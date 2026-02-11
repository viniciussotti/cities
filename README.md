🇧🇷 Brazilian Cities & States Database
Este repositório contém uma base de dados abrangente de Estados e Cidades do Brasil, ideal para sistemas de e-commerce, formulários de cadastro, logística ou qualquer aplicação que utilize dados geográficos nacionais.

A base inclui informações essenciais como nomes, siglas de UF, códigos DDD, códigos ISO e coordenadas de geolocalização (latitude e longitude).

🚀 Formatos Disponíveis
Os dados estão organizados em dois formatos principais para facilitar a integração:

CSV: Para manipulação rápida em planilhas ou importação genérica.

SQL: Scripts prontos para execução em bancos de dados relacionais (MySQL/PostgreSQL/MariaDB).

📊 Estrutura dos Dados
Estados (estados.csv / states.sql)
ID: Identificador único.

Nome: Nome completo do estado.

UF: Sigla da Unidade Federativa.

Código ISO: Código de padronização internacional.

Cidades (cidades.csv / cities.sql)
ID: Identificador único da cidade.

Nome: Nome da cidade.

UF: Sigla do estado pertencente.

DDD: Código de discagem direta a distância.

Latitude: Coordenada geográfica vertical.

Longitude: Coordenada geográfica horizontal.

📝 Demonstração dos Dados
Abaixo, um exemplo de como os dados estão estruturados no arquivo CSV:

Cidades:

Snippet de código
id,nome,uf,ddd,latitude,longitude
1100015,Alta Floresta D'Oeste,RO,69,-11.9355,-61.9998
1100023,Ariquemes,RO,69,-9.90846,-63.0333
3550308,São Paulo,SP,11,-23.5489,-46.6388
3304557,Rio de Janeiro,RJ,21,-22.9035,-43.2096
Estados:

Snippet de código
id,nome,uf,iso
11,Rondônia,RO,BR-RO
35,São Paulo,SP,BR-SP
33,Rio de Janeiro,RJ,BR-RJ
🛠️ Como Utilizar
Importação SQL
Se você utiliza um banco de dados SQL, basta executar os scripts na ordem:

states.sql

cities.sql

Uso com Python/Pandas
Python
import pandas as pd

# Carregar as cidades
df_cidades = pd.read_csv('cidades.csv')

# Filtrar cidades de um estado específico com DDD
sp_cidades = df_cidades[df_cidades['uf'] == 'SP']
print(sp_cidades[['nome', 'ddd']])
📄 Licença
Este projeto está sob a licença MIT. Sinta-se à vontade para usar e contribuir.
