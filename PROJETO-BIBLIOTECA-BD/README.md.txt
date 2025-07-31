# 📚 Projeto MySQL - Sistema de Bibliotecas

Repositório com a modelagem e implementação de um sistema de gerenciamento de bibliotecas usando MySQL.

🔗 [GitHub - ErickVeronezi](https://github.com/ErickVeronezi)

---

## 🗂️ Estrutura do Projeto

- `create_tables.sql` → Criação das tabelas principais do sistema.
- `constraints.sql` → Adição das chaves estrangeiras (FKs) e regras de integridade.
- `inserts_exemplo.sql` → População das tabelas com dados de exemplo.
- `views.sql` → Criação de views para relatórios e consultas específicas.
- `procedures.sql` → Procedures para ações automatizadas como registrar multas e atualizar status.
- `modelo dbdiagram.png` → Diagrama lógico das entidades (gerado via [dbdiagram.io](https://dbdiagram.io/)).
- `modelo brmodelo.jpg` → Modelo conceitual de alto nível do sistema.

---

## 🧱 Entidades Principais

- **BIBLIOTECA**: Cadastro das bibliotecas.
- **ENDERECO**: Localização de cada biblioteca.
- **LIVRO**: Cadastro de livros.
- **EXEMPLAR**: Cópias físicas dos livros.
- **CLIENTE**: Usuários da biblioteca.
- **EMPRESTIMO**: Registro dos empréstimos realizados.
- **MULTA**: Controle de multas por atraso na devolução.
- **CATEGORIA**: Classificação dos livros.

---

## 🔍 Principais Views

- `V_TOTAL_LIVROS`: Livros por biblioteca e quantidades disponíveis.
- `V_EMPRESTIMO_ABERTO`: Empréstimos em aberto ou atrasados.
- `V_EMPRESTIMOS_ATRASADO`: Apenas empréstimos atrasados.
- `V_TOTAL_EMPRESTIMOS`: Empréstimos por cliente.
- `V_LIVROS_DISPONIVEIS`: Quantidade de exemplares disponíveis por livro.
- `V_TOTAL_MULTA`: Multas pendentes por cliente.

---

## ⚙️ Procedures Implementadas

- `P_EMPRESTIMOS_POR_CLIENTE`: Lista todos os empréstimos de um cliente pelo nome.
- `P_ATUALIZAR_STATUS_EMPRESTIMO`: Atualiza o status de um empréstimo.
- `P_REGISTRAR_MULTA`: Registra uma nova multa associada a um empréstimo.
- `P_CLIENTES_ATRASADOS`: Lista todos os clientes com empréstimos atrasados.
- `P_LISTAR_LIVROS_POR_CATEGORIA`: Mostra todos os livros filtrados por categoria.

---

## 🛠️ Requisitos Técnicos

- **Banco de Dados**: MySQL
- **Compatibilidade**: MySQL 8.0+

---

## ✅ Status do Projeto

> Projeto **concluído** com tabelas, dados de exemplo, views e procedures.

---

## 📌 Autor

**Erick Veronezi**  
GitHub: [@ErickVeronezi](https://github.com/ErickVeronezi)

---
