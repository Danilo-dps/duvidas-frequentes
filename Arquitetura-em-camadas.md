# Arquitetura em Camadas

## Arquitetura em camadas ou Arquitetura em camadas/layers, as camadas correspondentes são:

### Camadas Principais:
1. **Controller**:
   - **Responsabilidade**: Gerenciar as requisições HTTP, processar as entradas do usuário e retornar respostas.

2. **Service**:
   - **Responsabilidade**: Contém a lógica de negócios da aplicação. Processa as requisições e coordena ações entre as outras camadas.

3. **Repository**:
   - **Responsabilidade**: Abstrai a camada de persistência, gerenciando as operações de banco de dados.

4. **Data Transfer Object (DTO) / Resources**:
   - **Responsabilidade**: Transferir dados entre as camadas da aplicação de forma segura e organizada.

### Camadas Adicionais (opcionais):
5. **Business Logic Layer (BLL)**:
   - **Responsabilidade**: Centralizar a lógica de negócios que pode ser reutilizada entre diferentes serviços.

6. **View Models**:
   - **Responsabilidade**: Encapsular dados para a apresentação, especialmente em arquiteturas MVVM (Model-View-ViewModel).

Essas camadas ajudam a manter a aplicação organizada, modular e escalável.
