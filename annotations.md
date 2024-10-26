# Annotations no Spring Boot

- Quanto as anotações, no desenvolvimento no spring boot, cada classe e cada método exige algum tipo de anotação quando a demanda for pelo protocolo HTTP

# Anotações na classe

`@RestController`: Indica que a classe vai tratar de requisições HTTP e que os métodos retornam dados diretamente. 

**@RestController**
```java
public class MyController {
    // Métodos aqui...
}
```

`@RequestMapping`: Usada na classe para definir o ponto de entrada base da URL. 

**@RestController**   
**@RequestMapping("/api")**
```java
public class MyController {
    // Métodos aqui...
}
```

# Anotações em Métodos
`@GetMapping`: Mapeia requisições HTTP GET para métodos específicos.

**@GetMapping("/users")**
```java
public List<User> getAllUsers() {
    return userService.getAllUsers();
}
```

`@PostMapping`: Mapeia requisições HTTP POST.

**@PostMapping("/users")**
```java
public User createUser(@RequestBody User user) {
    return userService.saveUser(user);
}
```

`@PutMapping`: Mapeia requisições HTTP PUT.

**@PutMapping("/users/{id}")**
```java
public User updateUser(@PathVariable Long id, @RequestBody User user) {
    return userService.updateUser(id, user);
}
```

`@DeleteMapping`: Mapeia requisições HTTP DELETE.

**@DeleteMapping("/users/{id}")**
```java
public void deleteUser(@PathVariable Long id) {
    userService.deleteUser(id);
}
```

### Essas são só algumas das anotações principais que você verá com mais frequência. Cada uma desempenha um papel vital na forma como a aplicação interage com as requisições HTTP.

# Todas as anotações serão relacionadas ao CRUD?

- Não necessariamente. Muitas anotações no Spring Boot estão relacionadas ao CRUD (Create, Read, Update, Delete), mas há um conjunto vasto de anotações que servem para outros propósitos além do CRUD. Aqui estão algumas delas:

## Segurança
`@Secured`: Define quais roles têm acesso a um método ou classe.

**@Secured("ROLE_USER")**
```java
public void secureMethod() {}
```

`@PreAuthorize`: Verifica se a expressão SpEL fornecida é verdadeira antes de permitir o acesso.

**@PreAuthorize("hasRole('ROLE_ADMIN')")**
```java
public void preAuthorizeMethod() {}
```

## Configuração
`@Configuration`: Indica que uma classe contém definições de beans Spring.

**@Configuration**
```java
public class AppConfig {}
```

`@Bean`: Define um bean que será gerido pelo Spring Container.

**@Bean**
```java
public DataSource dataSource() {
    return new DataSource();
}
```

## Agendamento
`@Scheduled`: Usada para agendar a execução de um método em intervalos regulares.

**@Scheduled(fixedRate = 5000)**
```java
public void scheduledTask() {}
```

## Cache
`@Cacheable`: Indica que o resultado de um método pode ser armazenado em cache.

**@Cacheable("books")**
```java
public Book findBook(Long id) {
    return bookRepository.findById(id);
}
```

`@CacheEvict`: Indica que uma ou mais entradas de cache devem ser removidas.

**@CacheEvict(value = "books", allEntries = true)**
```java
public void clearCache() {}
```

## Eventos
`@EventListener`: Define um método como listener para eventos específicos.

**@EventListener**
```java
public void handleEvent(ApplicationEvent event) {
    // Lógica do evento
}
```

### Essas são apenas algumas das anotações não relacionadas ao CRUD. O Spring Boot usa anotações para uma ampla gama de funcionalidades, tornando o desenvolvimento mais modular e simplificado

# Quando há a configuração do maven, ele baixa todas as dependencias, é daí que são usadas as anotações

- Quando você configura o Maven com o arquivo pom.xml, ele baixa todas as dependências especificadas. Essas dependências incluem bibliotecas e frameworks que contêm as anotações e outras funcionalidades que você usa no seu código.

- Por exemplo, se você incluir o **spring-boot-starter-web** no seu **pom.xml**, o **Maven** baixa todas as dependências necessárias do **Spring Boot**, incluindo as classes que contêm anotações como **@RestController**, **@GetMapping**, **@PostMapping**, etc.
Essas dependências são então disponibilizadas no classpath do seu projeto, permitindo que você use essas anotações diretamente nas suas classes e métodos.
Assim, o **Maven** gerencia as versões e resolve as dependências para que você possa se concentrar em desenvolver seu aplicativo sem se preocupar em manualmente baixar e configurar todas as bibliotecas.

# As anotações são recursos que são abstraidos da minha aplicação?

### Essa é a essência! As anotações funcionam como uma camada de abstração que simplifica e automatiza várias tarefas dentro da sua aplicação.

- Quando você usa uma anotação, está dizendo ao framework ou biblioteca para fazer algo específico. Por exemplo, ao usar **@Autowired**, você não precisa se preocupar com os detalhes de como a injeção de dependência é feita - o Spring cuida disso para você. Da mesma forma, **@GetMapping** configura automaticamente o método para responder a requisições **HTTP GET**, sem que você precise escrever manualmente o código para isso.

- Portanto, essas anotações ajudam a tornar o seu código mais conciso, limpo e fácil de manter, permitindo que você se concentre mais na lógica de negócios da sua aplicação, enquanto os detalhes complexos são tratados pelo framework.















































































