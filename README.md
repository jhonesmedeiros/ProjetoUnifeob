# README.md - Sistema RH AbracadabraKids

# Sistema RH AbracadabraKids

Este projeto é um **sistema web de Recursos Humanos** para a empresa AbracadabraKids, desenvolvido em **Python 3.11+ com Flask**. Ele permite o cadastro de candidatos, upload de currículos e administração segura via login de administrador.

## Funcionalidades
- Formulário de candidatura com campos de nome, sobrenome, telefone, email e motivo.
- Upload opcional de currículo (PDF, DOC, DOCX ou TXT).
- Banco de dados SQLite integrado para armazenamento seguro.
- Área de administração com login protegido e senha criptografada.
- Configuração opcional de envio de emails (Flask-Mail).

## Tecnologias Utilizadas
- Python 3.11+
- Flask, Flask-WTF, Flask-Login, Flask-Mail, Flask-SQLAlchemy
- Passlib para hashing seguro de senhas
- WTForms para validação de formulários

## Estrutura do Projeto
- `app.py`: arquivo principal com todas as rotas e lógica.
- `uploads/`: diretório onde os currículos enviados são armazenados.
- Banco de dados SQLite (`abracadabrakids.db`) criado automaticamente.

## Como Rodar
1. Clonar o repositório:
   ```bash
   git clone <seu-repositorio>
   cd <seu-repositorio>
   ```
2. Criar e ativar ambiente virtual:
   ```bash
   python -m venv venv
   source venv/bin/activate  # Linux/Mac
   venv\Scripts\activate     # Windows
   ```
3. Instalar dependências:
   ```bash
   pip install -r requirements.txt
   ```
4. Rodar a aplicação:
   ```bash
   python app.py
   ```
5. Acessar no navegador:
   ```
   http://127.0.0.1:5000
   ```

## Credenciais de Admin Padrão
- Usuário: `admin`
- Senha: `admin`
> **Atenção:** altere as credenciais em produção.

## Personalização
- Variáveis de configuração podem ser definidas via `.env`:
  - `SECRET_KEY`, `MAIL_SERVER`, `MAIL_PORT`, `MAIL_USERNAME`, `MAIL_PASSWORD` e outros.

Este README fornece uma visão geral clara e didática do sistema, permitindo que qualquer pessoa configure, teste e publique o projeto facilmente.
