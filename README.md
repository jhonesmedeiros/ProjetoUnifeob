# ProjetoUnifeob
Engenharia de Software
1) Objetivo
Sistema web minimalista para permitir que candidatos enviem seus dados e motivos para trabalhar em eventos da AbracadabraKids, com armazenamento local em SQLite e interface simples.

2) Tecnologias
- Python 3.11+
- Flask
- SQLite (arquivo abracadabrakids.db)

3) Como rodar (passo-a-passo)
- Instalar Python 3.11+
- Criar e ativar virtualenv (recomendado): python -m venv venv; source venv/bin/activate (Linux/Mac) ou venv\Scripts\activate (Windows)
- Instalar dependências: pip install Flask
- Salvar este arquivo como app.py
- Executar: python app.py
- Acessar: http://127.0.0.1:5000

4) Estrutura do sistema
- Rota / : Formulário público para candidaturas e listagem das 10 candidaturas mais recentes.
- Rota /apply : POST que salva candidatura no banco.
- Rota /admin/list : listar todas as candidaturas em texto (para uso interno).

5) Banco de dados (schema)
Tabela: applicants
- id INTEGER PK
- first_name TEXT
- last_name TEXT
- phone TEXT
- email TEXT
- reason TEXT
- location TEXT
- created_at TEXT (ISO timestamp UTC)

6) Segurança e melhorias sugeridas
- Adicionar autenticação para /admin
- Filtrar e sanitizar entradas com validação adicional
- Enviar e-mails automáticos (SMTP) para confirmar candidaturas
- Migrar para banco centralizado (Postgres) se escalar
- Adicionar upload de currículo (arquivo)

7) Deploy para produção (resumo)
- Use Gunicorn + Nginx ou uma plataforma como Render / Heroku / Railway
- Armazenar DB em serviço gerenciado ou usar Postgres
- Configurar variáveis de ambiente para SECRET_KEY e CONTACT_EMAIL

8) Como publicar no GitHub
- Iniciar repositório local, criar .gitignore (venv, *.db)
- Commit e push para GitHub
- Incluir README.md e LICENCE (se desejar)
