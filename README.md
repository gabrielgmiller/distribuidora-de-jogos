# 🎮 Distribuidora de Jogos

Aplicação web desenvolvida com **Python**, **Flask** e **PostgreSQL**, que permite o gerenciamento de jogos, pessoas associadas e receitas obtidas. Ideal para controle de uma distribuidora digital de jogos independentes.

## 🔧 Tecnologias Utilizadas

- Python 3
- Flask
- SQLAlchemy
- PostgreSQL
- Babel (traduções e formatação de datas)
- HTML + Jinja2 (templates)
- Werkzeug (autenticação de senha segura)

## 📁 Funcionalidades

- Cadastro e login de usuários com CNPJ
- Cadastro de jogos e pessoas associadas
- Controle de ganhos financeiros mensais
- Relatório de ganhos por mês e acumulado
- Interface web amigável com templates HTML

## 🗂 Estrutura Principal

- `app.py`: Aplicação Flask com as rotas e lógica do sistema
- `models/`: Modelos de banco de dados (usuário, jogo, pessoa, ganho)
- `templates/`: Páginas HTML renderizadas
- `database.ini`: Configurações de conexão com PostgreSQL

## 🔐 Requisitos

- Python 3.8+
- PostgreSQL
- Bibliotecas Python (instaláveis via `requirements.txt`)

## 🚀 Como Rodar Localmente

1. **Clone o repositório**
   ```bash
   git clone https://github.com/gabrielgmiller/distribuidora-de-jogos.git
   cd distribuidora-de-jogos
   ```

2. **Crie e ative um ambiente virtual (opcional, mas recomendado)**
   ```bash
   python -m venv venv
   source venv/bin/activate  # ou venv\Scripts\activate no Windows
   ```

3. **Instale as dependências**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure o arquivo `database.ini`**
   ```ini
   [postgresql]
   host=localhost
   database=seu_banco
   user=seu_usuario
   password=sua_senha
   port=5432
   ```

5. **Execute a aplicação**
   ```bash
   python app.py
   ```

6. Acesse em: [http://localhost:5000](http://localhost:5000)

## 📌 Observações

- A aplicação já cria as tabelas automaticamente com `db.create_all()` no primeiro run.
- Inclui mensagens de feedback via `flash()` para ações importantes.

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.