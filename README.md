# 💊 PharmaVida: Supply Chain & Logistics Analytics

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![SciPy](https://img.shields.io/badge/SciPy-8CAAE6?style=for-the-badge&logo=scipy&logoColor=white)
![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)

## 📌 1. Visão Geral do Projeto
O **PharmaVida** é um projeto de Ciência de Dados aplicado à cadeia de suprimentos (Supply Chain). O objetivo principal desta análise foi estruturar, limpar e modelar dados logísticos e de faturamento para identificar gargalos operacionais, otimizar rotas de entrega e extrair inteligência de negócios a partir do comportamento de compra e custos de frete.

A entrega final consiste em um pipeline de análise exploratória validado estatisticamente e um **Dashboard Executivo Interativo** que permite aos tomadores de decisão monitorar a saúde logística da empresa em tempo real.

## 🎯 2. O Problema de Negócio
No setor farmacêutico e de saúde, o tempo de entrega é um fator crítico. A operação da PharmaVida enfrentava o desafio de entender as variáveis que impactavam atrasos e custos de frete. As principais perguntas de negócios respondidas foram:
- *Existe uma correlação real entre o valor do pedido (Ticket) e o tempo de entrega?*
- *Quais regiões (Estados) apresentam maior ineficiência logística?*
- *Como está a distribuição de preços dos produtos mais movimentados pela logística?*

## 🛠️ 3. Tecnologias e Ferramentas Utilizadas
- **Linguagem:** Python
- **Manipulação e Limpeza:** Pandas, NumPy
- **Estatística e Testes de Hipóteses:** SciPy
- **Visualização de Dados e BI:** Power BI (DAX, Power Query)
- **Design de Dashboards:** Arquitetura de Layout em "Z", UI/UX em Dark Mode, Storytelling com Dados.

## ⚙️ 4. Metodologia e Desenvolvimento

O projeto foi dividido em 3 grandes fases:

### Fase 1: Engenharia e Limpeza de Dados (Python)
- **Data Cleaning:** Tratamento de valores nulos e correção de tipagem de dados.
- **Tratamento de Anomalias:** Identificação e remoção de *outliers* extremos (ex: erros de precisão flutuante que geravam notações científicas irreais como `2,697E+16`).
- **Merge de Dados:** Cruzamento de tabelas de clientes, produtos, pedidos e dados de logística para formar uma base analítica (Data Mart) unificada.

### Fase 2: Estatística Aplicada e EDA
- Realização de **Análise Exploratória de Dados (EDA)** para entender a distribuição temporal e geográfica das vendas.
- **Testes de Hipóteses:** Utilização de Correlação de Pearson para validar estatisticamente a relação entre produtos premium (`Preco_Unitario`) e a agilidade logística (`Tempo_Entrega_Dias`).

### Fase 3: Visualização e Inteligência de Negócios (Power BI)
- Importação da base limpa e resolução de conflitos de *Locale* (padrão US do Python vs. PT-BR do Power BI).
- Construção de um Dashboard focado em Supply Chain utilizando:
  - **KPIs (Cartões):** Faturamento Total, Preço Médio, Tempo Médio de Entrega e Custo Médio de Frete.
  - **Gráfico de Dispersão:** Para comprovar visualmente a correlação matemática entre Tempo e Preço.
  - **Matriz de Calor (Heatmap):** Evidenciando gargalos logísticos por Estado x Canal de Venda.
  - **Histograma:** Exibindo a distribuição de frequência dos pedidos.

## 🚀 5. Principais Insights Entregues
1. **Mapeamento de Gargalos:** O Heatmap regional permitiu identificar de forma instantânea quais estados estão operando fora do SLA de entrega.
2. **Correlação Operacional:** A dispersão comprovou os padrões de comportamento logístico de acordo com o ticket do produto.
3. **Integridade Financeira:** A limpeza rigorosa de *outliers* garantiu que os cálculos de faturamento total e ticket médio refletissem a realidade operacional, evitando distorções na tomada de decisão.

## 🧠 6. Aprendizados do Projeto
- **Tratamento de Tipagem Multi-Plataforma:** Lidar com os desafios de formatação de casas decimais (pontos vs. vírgulas) na transição de dados processados em Python para plataformas de visualização.
- **Design de Dashboards:** Aplicação do padrão de "Leitura em Z" para organizar informações de forma hierárquica, garantindo que o usuário consuma primeiro os KPIs gerais e, em seguida, desça para análises mais granulares.



---
**Desenvolvido por [Vitor Ferrari Mendes](https://www.linkedin.com/in/SEU-LINKEDIN-AQUI)**  
*Analista de Dados | Estudante de Ciência de Dados | Embaixador Google Students*
