# 🗳️ Análise Eleitoral & Socioeconômica (SC 2022)
**(Excel + Power Pivot + DAX + Star Schema)**

> 🔗 **[CLIQUE AQUI PARA ACESSAR O DASHBOARD INTERATIVO](https://app.powerbi.com/view?r=eyJrIjoiMmMxNDk3ZGMtNjJlYS00NjM2LTg1NDUtNzRiY2VjZTllNTNkIiwidCI6ImYwYzhjMGRmLTQ5MWItNDMyYy1iZmNjLTM5ZjljNzZiYzI2YiJ9)**

Projeto de Business Intelligence que integra dados eleitorais do TSE (**2,1 milhões de registros**) com indicadores socioeconômicos do IBGE, com o objetivo de analisar a distribuição proporcional de votos em diferentes faixas de PIB e renda municipal.

---

### 📚 1. Objetivo do Projeto

O objetivo foi construir uma análise profunda e executiva sobre o cenário eleitoral de Santa Catarina em 2022, cruzando o Big Data das urnas com a realidade econômica do IBGE para identificar padrões de comportamento eleitoral baseados na riqueza municipal.

**Os dados são baseados em fontes oficiais públicas: [TSE (Resultados por Seção)](https://dadosabertos.tse.jus.br/), [IBGE (Censo 2022)](https://www.ibge.gov.br/) e [SIDRA](https://sidra.ibge.gov.br/).**

Toda a solução foi desenvolvida focando em:

✔ **Processamento de Big Data** (2.1M+ de linhas) via Power Pivot

✔ **Modelagem Star Schema** no Modelo de Dados do Excel

✔ **DAX Avançado** para classificação socioeconômica

✔ **Dashboard Executivo** com foco em inteligência de dados

---

### 🏗️ 2. Engenharia de Dados (O Motor do Projeto)

Nesta etapa, o foco foi garantir a performance analítica superando os limites tradicionais de planilhas:

* **Processamento em Memória:** Utilização do engine **xVelocity (Power Pivot)** para gerenciamento e análise eficiente de **2.178.931 registros** de votação sem perda de performance.
* **ETL e Padronização (Power Query):** * **Normalização de Chaves:** Ajuste de identificadores para garantir a integridade referencial entre as bases do TSE e IBGE.
    * **Tipagem de Dados:** Conversão de IDs para **Texto**, preservando zeros à esquerda e evitando erros de integridade.
    * **Higienização:** Remoção de ruídos estatísticos e colunas irrelevantes para otimizar o peso do modelo.

---

### 📊 3. Arquitetura do Modelo (Star Schema)

O modelo foi estruturado seguindo as melhores práticas de Business Intelligence para permitir cruzamentos multidimensionais rápidos:

* **Tabela Fato (`votacao_secao`):** Centraliza os votos transacionais.
* **Tabelas de Dimensão:**
    * **Dimensão IBGE:** Cadastro de cidades com dados de PIB/Renda.
    * **Dimensão Candidatos/Partidos:** Identificação de legendas e nomes.
    * **Dimensão Calendário:** Estrutura temporal para análises cronológicas.



---

### 📈 4. Análises Desenvolvidas com DAX

Fórmulas inteligentes que transformam dados brutos em insights estratégicos:

* **Classificação Socioeconômica Dinâmica:** Categorização automática dos municípios em: *Elite Econômica, PIB Alto, PIB Médio e PIB Baixo*.
* **Análise Proporcional (Market Share):** Cálculo de participação percentual por partido utilizando `% do Total da Linha`, permitindo comparação justa entre municípios de diferentes portes.
* **Análise de Extremos Econômicos:** Comparação direta entre os 5 municípios com maior PIB vs. os 5 com menor PIB.

> ⚠️ **Nota:** A análise considera indicadores médios municipais e não características individuais dos eleitores.

---

### 🎯 5. Entrega Analítica (Dashboard)

Interface desenhada para análise executiva e tomada de decisão:

* **Navegação Sincronizada:** Filtros de municípios que refletem instantaneamente em todos os indicadores.
* **Visualização Comparativa:** Gráficos estruturados para leitura rápida da dominância partidária por faixa de renda.
* **Estrutura Executiva:** Design limpo, focado em tabelas dinâmicas conectadas diretamente ao Modelo de Dados.

---

### 🧠 Competências Demonstradas
* **ETL:** Power Query
* **Modelagem:** Star Schema & xVelocity Engine
* **Linguagem:** DAX (Medidas e Colunas Calculadas)
* **Gestão de Dados:** Big Data no Excel (2.1M+ registros)
* **Repositório:** Organização estruturada no GitHub

---

### 🙋‍♂️  Sobre o Autor

**TIAGO SANTOS**
* Analista de Dados • Excel | SQL | Power BI
* Foco em análises de e-commerce, logística e performance comercial.

---

## ⚖️ Licença / Aviso Legal

Todo o conteúdo deste repositório foi desenvolvido para fins **educacionais e de portfólio pessoal**.
Você é livre para usar, modificar e compartilhar os arquivos, desde que mantenha os devidos créditos ao autor original.

---

## 🤝 Conecte-se comigo

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Tiago%20Magalhães%20Santos-blue?logo=linkedin)](https://www.linkedin.com/in/tiago-magalh%C3%A3es-santos-0b6ab0b6/)

---
