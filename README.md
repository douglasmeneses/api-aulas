# 🏢 API de Gestão de Funcionários — Programação Web

![Java](https://img.shields.io/badge/Java-11-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-2.7-6DB33F?style=for-the-badge&logo=spring-boot&logoColor=white)
![Spring Data JPA](https://img.shields.io/badge/Spring_Data_JPA-6DB33F?style=for-the-badge&logo=spring&logoColor=white)
![H2 Database](https://img.shields.io/badge/H2-Database-003B57?style=for-the-badge)
![Gradle](https://img.shields.io/badge/Gradle-02303A?style=for-the-badge&logo=gradle&logoColor=white)

API RESTful desenvolvida para a disciplina de **Programação Avançada para Web**, com foco na implementação de arquitetura em camadas (Controller, Service, Repository), operações de CRUD completas para gestão de funcionários e persistência com **Spring Data JPA** e banco em memória **H2**.

---

## 📌 Funcionalidades

- 👔 **Gestão de Funcionários:** Cadastro, listagem geral, busca por identificador, atualização e remoção de colaboradores.
- 📐 **Arquitetura em Camadas:** Desacoplamento entre camada de exposição HTTP (`controller`), regras de negócio (`service`) e persistência relacional (`repository`).
- ⚡ **Banco de Dados In-Memory H2:** Configuração ágil sem necessidade de instalação de SGBD externo.

---

## 🏗️ Estrutura do Projeto

```text
src/main/java/com/api1/ap1/
├── controller/        # FuncionarioController (Endpoints REST)
├── model/             # Entidade JPA Funcionario
├── repository/        # FuncionarioRepository (Spring Data JPA)
├── service/           # FuncionarioService (Regras de negócio)
└── Ap1Application.java
```

---

## 🛠️ Tecnologias Utilizadas

- **Linguagem:** [Java 11](https://www.oracle.com/java/)
- **Framework:** [Spring Boot 2.7.16](https://spring.io/projects/spring-boot)
- **Acesso a Dados:** Spring Data JPA / Hibernate
- **Banco de Dados:** H2 Database (em memória)
- **Produtividade:** Project Lombok & Spring Boot DevTools
- **Build Tool:** Gradle

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
- [JDK 11](https://adoptium.net/) ou superior

### 1. Clonar o repositório
```bash
git clone https://github.com/douglasmeneses/api-aulas.git
cd api-aulas
```

### 2. Executar a aplicação
No Linux/macOS:
```bash
./gradlew bootRun
```
No Windows:
```cmd
gradlew.bat bootRun
```

A API estará rodando em `http://localhost:8080`.

---

## 📡 Endpoints da API

| Método | Rota | Descrição |
| :--- | :--- | :--- |
| `GET` | `/funcionarios` | Lista todos os funcionários |
| `GET` | `/funcionarios/{id}` | Busca funcionário por ID |
| `POST` | `/funcionarios` | Cadastra um novo funcionário |
| `PUT` | `/funcionarios/{id}` | Atualiza os dados de um funcionário |
| `DELETE` | `/funcionarios/{id}` | Remove um funcionário |

---

## 👨‍💻 Autor

Desenvolvido por **Douglas Meneses**.

- 💼 GitHub: [@douglasmeneses](https://github.com/douglasmeneses)
- ✉️ Email: [meneses.doug@gmail.com](mailto:meneses.doug@gmail.com)
