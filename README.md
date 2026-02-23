# 🗳️ Inteligência Eleitoral & Análise Socioeconômica
**(Excel + Power Pivot + DAX – Santa Catarina 2022)**

Projeto completo de análise de dados utilizando **Excel (Power Pivot)** e **Linguagem DAX** para investigar o comportamento eleitoral em Santa Catarina, com foco em:
* **Desempenho por Candidato e Partido**
* **Correlação entre PIB per Capita e Votos**
* **Perfil de Rendimento Domiciliar (Censo 2022)**
* **Categorização socioeconômica municipal**
* **Insights estratégicos para análise de gabinete**

---

### 📚 1. Objetivo do Projeto

O objetivo foi construir uma análise profunda e executiva sobre o cenário eleitoral de Santa Catarina em 2022, cruzando o Big Data das urnas com a realidade econômica do IBGE para identificar: Como a riqueza municipal influencia a preferência partidária e quais regiões apresentam os maiores contrastes entre renda e voto.

**Os dados são baseados em fontes oficiais públicas: [TSE (Resultados por Seção)](https://dadosabertos.tse.jus.br/), [IBGE (Censo 2022)](https://www.ibge.gov.br/) e [SIDRA (Banco de Tabelas e Estatísticas)](https://dadosabertos.tse.jus.br/).**

Toda a solução foi feita do zero:

✔ **Limpeza e ETL massivo** no Excel (Power Query)

✔ **Gestão de Big Data** (2.1M+ de linhas) via Power Pivot

✔ **Modelagem Star Schema** no Modelo de Dados do Excel

✔ **DAX avançado** para classificação de faixas de PIB e Renda

✔ **Dashboard executivo** com navegação sincronizada

✔ **Insights socioeconômicos**

---

### 🏗️ 2. Engenharia de Dados (O Motor do Projeto)

Nesta etapa, o foco foi garantir que o Excel processasse um volume de dados 2x maior que seu limite padrão:

* **Processamento de Big Data:** Utilização do motor **xVelocity (Power Pivot)** para gerenciar **2.178.931 registros** de votação sem perda de performance ou travamentos.
* **Data Cleaning (Higienização):** * **Base IBGE:** Remoção de ruídos estatísticos e exclusão de colunas irrelevantes para manter o foco total em PIB e Renda.
    * **Base Candidatos:** Refinação do dicionário em conformidade com a **LGPD**, eliminando dados sensíveis e focando em chaves analíticas.
* **Tipagem de Dados:** Conversão rigorosa de identificadores para **Texto**, garantindo a integridade de códigos com zeros à esquerda e evitando somas acidentais de IDs.

---

### 📊 3. Arquitetura do Modelo (Star Schema)

O modelo foi estruturado seguindo as melhores práticas de Business Intelligence para permitir cruzamentos rápidos:

* **Tabela Fato (`votacao_secao`):** Centraliza os votos transacionais de SC.
* **Tabelas de Dimensão:**
    * **Dimensão IBGE:** Cadastro de cidades com dados de PIB/Renda.
    * **Dimensão Candidatos:** Identificação de nomes, números e legendas.
* **Relacionamentos:** Conexões robustas via chaves únicas, garantindo que o filtro de um município reflita instantaneamente em todos os indicadores socioeconômicos.

---

### 📈 4. Dashboard Interativo & BI

Interface desenhada para análise executiva e tomada de decisão:

* **Segmentação Executiva:** Filtro de municípios posicionado estrategicamente na Coluna B com design em **Cinza Neutro**.
* **Análise Multidimensional:** Sincronização completa entre tabelas de votos, tabelas socioeconômicas e gráficos de desempenho.
* **Categorização por DAX:** Fórmulas inteligentes que classificam automaticamente os municípios em: *Elite Econômica, PIB Alto, PIB Médio e PIB Baixo*.

---

### 🔗 5. Fontes de Dados
* **TSE:** Resultados de votação por seção eleitoral (SC - 2022).
* **IBGE:** Indicadores de Rendimento e PIB Municipal (Censo 2022).
