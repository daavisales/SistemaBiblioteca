# Library Management System (Console)

A console app in plain Java for managing an academic library: books, students, professors and loans. College project focused on object-oriented design.

> 🇧🇷 Original Portuguese documentation: [README.pt-BR.md](./README.pt-BR.md) · GUI version: [SistemaBiblioteca2.0](https://github.com/daavisales/SistemaBiblioteca2.0)

![Java](https://img.shields.io/badge/Java-8%2B-orange?logo=openjdk&logoColor=white)

## Features

- Register books and users (students and professors)
- Borrow and return books; due date and loan limit depend on the user type
- List books, users and active loans

## OOP concepts applied

- **Abstraction and inheritance:** `Usuario` is abstract; `Aluno` and `Professor` extend it.
- **Polymorphism:** loan limit and loan period are overridden per user type.
- **Encapsulation:** private state behind getters and setters.
- **Layering:** `modelo` (domain), `servico` (business rules), `interfacee` (console UI), `principal` (entry point).

## Run locally

Requires JDK 8+.

```bash
javac -d out $(find . -name '*.java')
java -cp out principal.Main
```
