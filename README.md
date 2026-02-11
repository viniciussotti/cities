# 🇧🇷 Brazilian Cities & States Database

Este repositório contém uma base de dados completa e higienizada de **Estados e Cidades do Brasil**. É uma ferramenta essencial para desenvolvedores que precisam implementar seletores de localidade, sistemas de logística, calculadoras de frete ou qualquer aplicação que dependa de dados geográficos nacionais precisos.

A base inclui informações estratégicas como nomes oficiais, siglas de UF, códigos DDD, códigos ISO e coordenadas de geolocalização (latitude e longitude).

---

## 🚀 Formatos Disponíveis

Os dados estão organizados para facilitar a integração em diferentes stacks:

* **CSV:** Ideal para manipulação rápida em scripts Python, Excel ou importações genéricas.
* **SQL:** Scripts prontos para execução em bancos de dados relacionais (MySQL, PostgreSQL, MariaDB, SQLite).

---

## 📊 Estrutura dos Dados

### Estados (`estados.csv` / `states.sql`)
| Campo | Descrição |
| :--- | :--- |
| `id` | Código IBGE do estado |
| `nome` | Nome completo da Unidade Federativa |
| `uf` | Sigla do estado (ex: SP, RJ, PR) |
| `iso` | Código de padronização internacional (ex: BR-SP) |

### Cidades (`cidades.csv` / `cities.sql`)
| Campo | Descrição |
| :--- | :--- |
| `id` | Código IBGE da cidade |
| `nome` | Nome oficial do município |
| `uf` | Sigla do estado ao qual a cidade pertence |
| `ddd` | Código de discagem direta a distância |
| `latitude` | Coordenada geográfica (Eixo Y) |
| `longitude` | Coordenada geográfica (Eixo X) |

---

## 📝 Demonstração dos Dados

Exemplo de visualização dos dados estruturados:

### Cidades (CSV)
```csv
id,nome,uf,ddd,latitude,longitude
1100015,Alta Floresta D'Oeste,RO,69,-11.9355,-61.9998
1100023,Ariquemes,RO,69,-9.90846,-63.0333
3550308,São Paulo,SP,11,-23.5489,-46.6388
3304557,Rio de Janeiro,RJ,21,-22.9035,-43.2096
4105805,Colorado,PR,44,-22.8375,-51.9731
