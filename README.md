<div align="center">

# Divide.ai API

API REST para gerenciamento financeiro pessoal e compartilhado, com integração de inteligência artificial para auxiliar na análise das finanças do usuário.

<p>
  <img src="https://img.shields.io/badge/Java%2017-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java 17"/>
  <img src="https://img.shields.io/badge/Spring%20Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI"/>
</p>

</div>

## Sobre

O **Divide.ai** é uma API para gerenciamento de finanças pessoais e compartilhamento de despesas entre grupos.

A aplicação permite organizar transações, categorias e grupos, dividir despesas entre participantes e acompanhar as dívidas geradas.

Também possui integração com a **OpenAI**, utilizando informações financeiras do usuário como contexto para oferecer um assistente financeiro personalizado.

## Funcionalidades

* Cadastro e autenticação de usuários com JWT
* Gerenciamento de transações e categorias
* Criação e gerenciamento de grupos
* Divisão de despesas entre participantes
* Gerenciamento de dívidas
* Assistente financeiro integrado à OpenAI
* Histórico de interações
* Envio de e-mails
* Validação e tratamento de erros

## Tecnologias

<p>
  <img src="https://img.shields.io/badge/Java%2017-ED8B00?style=flat-square&logo=openjdk&logoColor=white" alt="Java"/>
  <img src="https://img.shields.io/badge/Spring%20Boot%203-6DB33F?style=flat-square&logo=springboot&logoColor=white" alt="Spring Boot"/>
  <img src="https://img.shields.io/badge/Spring%20Security-6DB33F?style=flat-square&logo=springsecurity&logoColor=white" alt="Spring Security"/>
  <img src="https://img.shields.io/badge/Hibernate-59666C?style=flat-square&logo=hibernate&logoColor=white" alt="Hibernate"/>
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/JWT-000000?style=flat-square&logo=jsonwebtokens&logoColor=white" alt="JWT"/>
  <img src="https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white" alt="OpenAI"/>
  <img src="https://img.shields.io/badge/Maven-C71A36?style=flat-square&logo=apachemaven&logoColor=white" alt="Maven"/>
</p>

Também são utilizados **Spring Data JPA, MapStruct, Jakarta Validation e Spring Mail**.

## Executando

### Pré-requisitos

* Java 17+
* PostgreSQL
* Chave da OpenAI

Clone o repositório:

```bash
git clone https://github.com/wislaargolo/divide.ai-api.git
cd divide.ai-api
```

Configure as variáveis de ambiente:

```env
DATABASE_URL=jdbc:postgresql://localhost:5432/divide_ai
DATABASE_USER=postgres
DATABASE_PASSWORD=sua_senha

OPENAI_KEY=sua_chave

USERNAME_EMAIL=seu_email
PASSWORD_EMAIL=sua_senha
```

Execute:

```bash
./mvnw spring-boot:run
```

A aplicação ficará disponível em:

```text
http://localhost:8080
```

## Repositórios relacionados

### [divide.ai-framework](https://github.com/wislaargolo/divide.ai-framework)

Evolução do Divide.ai focada em reutilização e extensibilidade, extraindo funcionalidades comuns para um núcleo compartilhado e permitindo diferentes especializações de domínio.
