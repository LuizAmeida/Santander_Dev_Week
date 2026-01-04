# 🏦 Santander Dev Week - Pipeline ETL com Python

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Data Science](https://img.shields.io/badge/Data%20Science-ETL-green?style=for-the-badge)

## 🎯 Objetivo do Projeto
Este projeto foi desenvolvido como parte do desafio da **Santander Dev Week** pela DIO. O foco principal é demonstrar o domínio do fluxo **ETL (Extract, Transform, Load)** utilizando Python e a biblioteca Pandas para processamento de dados bancários simulados.

> **Nota:** Devido à indisponibilidade da API original do evento, este projeto utiliza a **Alternativa 2**, onde geramos uma base de dados sintética robusta com 100 registros para simular o motor de decisão de crédito e marketing do Santander.

---

## 🛠️ O Pipeline ETL

O projeto está dividido em etapas modulares para garantir a clareza e manutenção do código:

### 1. Preparação (Geração de Dados)
Como analista de dados, utilizei **Análise Combinatória** entre listas de nomes e sobrenomes para gerar **100 perfis únicos**. Cada perfil conta com:
* **Saldo Bancário:** Gerado aleatoriamente.
* **Score de Crédito:** Simulando o risco financeiro (100 a 1000).
* **Perfil de Investidor:** Conservador, Moderado ou Arrojado.

### 2. Extração (Extract)
Leitura da base de dados bruta em formato `.csv` utilizando o método `pd.read_csv()`, garantindo que os dados estejam prontos para processamento em memória.

### 3. Transformação (Transform)
Aqui reside a inteligência do projeto. Criamos um **Motor de Regras** que:
* **Calcula Limites:** Aumenta o limite do cartão proporcionalmente ao Score de Crédito do cliente.
* **Personaliza Ofertas:** Gera uma mensagem de marketing específica para cada perfil de investidor, simulando o comportamento de uma IA Generativa.



### 4. Carregamento (Load)
Os dados enriquecidos e transformados são exportados para um novo arquivo final (`santander_final_data.csv`), pronto para ser consumido por outras camadas da aplicação ou dashboards.

---

## 📁 Estrutura de Arquivos
* `main.ipynb` (ou `.py`): Contém todas as células do pipeline ETL.
* `santander_users.csv`: Base gerada inicialmente (Entrada).
* `santander_final_data.csv`: Base processada e enriquecida (Saída).

## 🚀 Como Executar
1. Clone este repositório:
   ```bash
   git clone [https://github.com/SEU-USUARIO/santander-dev-week-2023.git](https://github.com/SEU-USUARIO/santander-dev-week-2023.git)
   ````

## 2. Instale as dependências:
  ````bash
   pip install pandas
  ````

## 3. Execute o script principal para ver a mágica do ETL acontecer!

## 👨‍💻 Desenvolvedor
## Luiz - Cientista de Dados em Formação



---
*Projeto realizado para a **[Santander Dev Week](https://github.com/santanderdevweek)** - **[Digital Innovation One](https://www.dio.me/)**.*


