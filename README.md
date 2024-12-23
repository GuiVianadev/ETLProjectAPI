# ETL com Python e Requests

Este é um projeto de ETL (Extract, Transform, Load) desenvolvido em Python, que utiliza a biblioteca `requests` para consumir dados de APIs. O objetivo do projeto é extrair dados, transformá-los conforme as necessidades do negócio e carregá-los em uma base de dados ou outro formato estruturado.

## Tecnologias Utilizadas

- **Python**: Linguagem principal para o desenvolvimento do projeto.
- **Requests**: Para realizar requisições HTTP e consumir APIs.
- **Pandas**: Para manipulação e transformação dos dados.
- **SQLite**: Banco de dados local para armazenar os dados carregados (opcional).
- **Jupyter Notebook** (opcional): Para prototipação e análise dos dados.

## Estrutura do Projeto

etl-project/ │ ├── data/ # Diretório para armazenamento de dados transformados │ ├── raw/ # Dados brutos extraídos │ └── processed/ # Dados processados e prontos para carregamento │ ├── scripts/ # Scripts principais do projeto │ ├── extract.py # Lógica de extração de dados │ ├── transform.py # Lógica de transformação de dados │ └── load.py # Lógica de carregamento de dados │ ├── requirements.txt # Dependências do projeto └── README.md # Documentação do projeto

markdown
Copy code

## Funcionalidades

1. **Extração (Extract)**:
   - Consumo de dados de APIs REST utilizando a biblioteca `requests`.

2. **Transformação (Transform)**:
   - Limpeza e transformação de dados usando a biblioteca `pandas`.

3. **Carregamento (Load)**:
   - Salvamento dos dados em formato `.csv` ou banco de dados SQLite.

## Pré-requisitos

Certifique-se de que você tem o Python 3.8 ou superior instalado. As dependências do projeto estão listadas no arquivo `requirements.txt`.

## Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/etl-project.git
   cd etl-project
Crie um ambiente virtual (recomendado):

bash
Copy code
python -m venv venv
source venv/bin/activate  # No Windows, use `venv\Scripts\activate`
Instale as dependências:

bash
Copy code
pip install -r requirements.txt
Como Executar
Execute o script de extração:

bash
Copy code
python scripts/extract.py
Execute o script de transformação:

bash
Copy code
python scripts/transform.py
Execute o script de carregamento:

bash
Copy code
python scripts/load.py
Melhorias Futuras
Adicionar testes unitários para validar o pipeline.
Implementar suporte a múltiplas fontes de dados (APIs adicionais, arquivos CSV, etc.).
Automatizar o pipeline com agendamento (ex.: cron jobs ou apscheduler).
Contribuições
Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests.