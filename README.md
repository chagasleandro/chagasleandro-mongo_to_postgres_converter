# 🛠️ MongoDB to PostgreSQL Converter

Ferramenta em Python para migrar dados de uma coleção MongoDB para uma tabela PostgreSQL com **criação automática de schema**.

Este projeto foi criado com o objetivo de **automatizar tarefas comuns de suporte técnico e integração de dados**, demonstrando habilidades práticas com bancos de dados, Python e automação de processos.

---

## 📌 Funcionalidades

- 🔄 Migração de dados MongoDB → PostgreSQL
- 🔍 Detecção automática do schema baseado nos documentos
- 🧱 Criação da tabela no PostgreSQL
- 📥 Inserção em lote dos dados
- 🛡️ Separação de credenciais via `.env`

---

## ⚙️ Tecnologias Utilizadas

- Python 3.10+
- [PyMongo](https://pymongo.readthedocs.io/)
- [Psycopg2](https://www.psycopg.org/)
- PostgreSQL
- MongoDB
- Dotenv

---

## 🚀 Como Usar

### 1. Clone o repositório

```bash
git clone https://github.com/chagasleandro/mongo_to_postgres_converter.git
cd mongo_to_postgres_converter

2. Instale as dependências
pip install -r requirements.txt

3. Configure o arquivo .env
Crie um arquivo .env com base no .env.example:
MONGO_URI=mongodb://localhost:27017
MONGO_DB=meubanco
MONGO_COLLECTION=clientes

PG_HOST=localhost
PG_DB=meubanco_postgres
PG_USER=postgres
PG_PASSWORD=123456
PG_PORT=5432

4. Execute a migração
python main.py

🧪 Exemplo de Documento no MongoDB
{
  "nome": "Maria",
  "idade": 28,
  "email": "maria@email.com",
  "ativo": true
}

Resultado no PostgreSQL:
CREATE TABLE clientes (
  nome TEXT,
  idade INTEGER,
  email TEXT,
  ativo BOOLEAN
);

🤝 Contribuições

📫 Contato

Desenvolvido por Leandro Chagas
📧 leandrosrs2012@gmail.com
🔗 GitHub
📄 Licença

Este projeto está licenciado sob a MIT License.

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.



