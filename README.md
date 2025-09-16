# ProjetoUnifeob
Engenharia de Software
1) Objetivo
Sistema web minimalista para permitir que candidatos enviem seus dados e motivos para trabalhar em eventos da AbracadabraKids, com armazenamento local em SQLite e interface simples.

2) Tecnologias
- Python 3.11+
- Flask
- SQLite (arquivo abracadabrakids.db)

3) Estrutura do sistema
- Rota / : Formulário público para candidaturas e listagem das 10 candidaturas mais recentes.
- Rota /apply : POST que salva candidatura no banco.
- Rota /admin/list : listar todas as candidaturas em texto (para uso interno).

4) Banco de dados (schema)
Tabela: applicants
- id INTEGER PK
- first_name TEXT
- last_name TEXT
- phone TEXT
- email TEXT
- reason TEXT
- location TEXT
- created_at TEXT (ISO timestamp UTC)

5) Segurança e melhorias sugeridas
- Adicionar autenticação para /admin
- Filtrar e sanitizar entradas com validação adicional
- Enviar e-mails automáticos (SMTP) para confirmar candidaturas
- Migrar para banco centralizado (Postgres) se escalar
- Adicionar upload de currículo (arquivo)

