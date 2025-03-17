# Entregavel 01

## Descrição do Projeto

Este projeto tem o objetivo de realizar análises de dados relacionados à produção agrícola. Primeiro o foco na análise exploratória de dados e na modelagem preditiva para prever o rendimento de culturas com base em variáveis climáticas. O segundo foco tem o objetivo de realizar uma análise de tendências, clusters e outliers nos dados de produção agrícola.

## Estrutura do Projeto

### 1. Parte 01

#### Objetivo
O objetivo é realizar uma análise exploratória dos dados de produção agrícola e construir modelos de machine learning para prever o rendimento das culturas com base em variáveis climáticas.

#### Passos Principais
1. **Importação de Bibliotecas e Carregamento dos Dados**:
   - Importação das bibliotecas necessárias (pandas, numpy, matplotlib, seaborn, etc.).
   - Carregamento do dataset `crop_yield.csv`.

2. **Exploração e Pré-processamento dos Dados**:
   - Verificação de valores ausentes.
   - Estatísticas descritivas dos dados.
   - Codificação da variável categórica 'Crop'.
   - Normalização das variáveis preditoras.
   - Divisão dos dados em conjuntos de treino e teste.

3. **Treinamento e Avaliação dos Modelos**:
   - Definição de vários modelos de regressão (Linear Regression, Random Forest, Gradient Boosting, KNN, MLP Regressor).
   - Treinamento e avaliação dos modelos usando métricas como R² e RMSE.
   - Comparação dos resultados dos modelos.

4. **Visualização da Performance**:
   - Gráficos comparando o desempenho dos modelos em termos de R² e RMSE.

5. **Conclusão**:
   - O modelo Random Forest apresentou o melhor desempenho, com um R² de 0,994401 e o menor erro (RMSE).

### 2. PARTE 02

#### Objetivo
O objetivo  e identificar outliers nos dados de produção agrícola e realizar uma análise de tendências e clusters.

#### Passos Principais
1. **Importação de Bibliotecas e Carregamento dos Dados**:
   - Importação das bibliotecas necessárias (pandas, numpy, matplotlib, seaborn, etc.).
   - Carregamento do dataset `crop_yield.csv`.

2. **Identificação de Outliers**:
   - Uso de métodos como Z-score e IQR para identificar outliers.
   - Visualização dos outliers usando boxplots.
   - Análise detalhada dos outliers identificados.

3. **Análise de Tendências e Clusters**:
   - Uso de técnicas de redução de dimensionalidade (PCA) para visualização espacial dos dados.
   - Identificação de clusters usando KMeans e DBSCAN.

4. **Conclusão**:
   - Identificação de outliers e análise de tendências nos dados de produção agrícola.

### Link youtube:
https://youtu.be/avImwD7Iq9o


# Entregavel 02

## 1. Estimativa de Preços da AWS

## Resumo da Estimativa

| Custo inicial | Custo mensal | Custo total de 12 meses |
|---------------|--------------|-------------------------|
| 0,00 USD      | 27,51 USD    | 330,12 USD              |
|               |              | Inclui um custo inicial |

## Estimativa Detalhada

### Amazon EC2 - US East (N. Virginia)

- **Grupo:** Nenhum grupo aplicado
- **Região:** US East (N. Virginia)
- **Custo inicial:** 0,00 USD
- **Custo mensal:** 10,13 USD

**Status:** -  
**Descrição:** -  

**Resumo da configuração:**  
- Locação: Instâncias compartilhadas  
- Sistema operacional: Linux  
- Carga de trabalho: Consistent  
- Número de instâncias: 1  
- Instância do EC2 avançada: t4g.micro  
- Estratégia de preços: On-Demand Utilization: 100% Utilized/Month  
- Habilitar monitoramento: Desabilitada  
- EBS Quantidade de armazenamento: 50 GB  
- DT Entrada: Not selected (0 TB por mês)  
- DT Saída: Not selected (0 TB por mês)  
- DT Intrarregião: 0 TB por mês  

### Amazon EC2 - South America (Sao Paulo)

- **Grupo:** Nenhum grupo aplicado
- **Região:** South America (Sao Paulo)
- **Custo inicial:** 0,00 USD
- **Custo mensal:** 17,38 USD

**Status:** -  
**Descrição:** -  

**Resumo da configuração:**  
- Locação: Instâncias compartilhadas  
- Sistema operacional: Linux  
- Carga de trabalho: Consistent  
- Número de instâncias: 1  
- Instância do EC2 avançada: t4g.micro  
- Estratégia de preços: On-Demand Utilization: 100% Utilized/Month  
- Habilitar monitoramento: Desabilitada  
- EBS Quantidade de armazenamento: 50 GB  
- DT Entrada: Not selected (0 TB por mês)  
- DT Saída: Not selected (0 TB por mês)  
- DT Intrarregião: 0 TB por mês  

## Confirmação

A Calculadora de Preços da AWS fornece apenas uma estimativa de suas taxas da AWS e não inclui nenhuma taxa. Suas taxas reais dependem de vários fatores, inclusive de seu uso real dos serviços da AWS. Saiba mais 😊

---

**Data de exportação:** 15/03/2025  
**Idioma:** Português  
**Estimar URL:** [https://calculator.aws/#/estimate?id=b34093a1e178bd19389fedcd74e37ccab03d29f3](https://calculator.aws/#/estimate?id=b34093a1e178bd19389fedcd74e37ccab03d29f3)



# 2. Escolha da Região AWS para Armazenamento de Dados de Sensores considerando Restrições Legais

Dadas as restrições legais para armazenamento no exterior e a necessidade de acessar rapidamente os dados dos sensores, a melhor opção é utilizar a **região AWS South America (São Paulo)**.

## Justificativa

### 1. Conformidade Legal
- A região **South America (São Paulo)** está localizada fisicamente no Brasil, garantindo conformidade com as leis locais de proteção de dados, como a **Lei Geral de Proteção de Dados (LGPD)**.
- Isso evita problemas legais relacionados ao armazenamento de dados em servidores localizados no exterior, que podem não estar em conformidade com as regulamentações brasileiras.

### 2. Latência Reduzida
- Armazenar os dados dos sensores em uma região próxima (como São Paulo) reduz significativamente a latência, o que é crucial para aplicações que dependem de respostas em tempo real ou de baixa latência, como monitoramento de sensores IoT ou sistemas de automação.

### 3. Disponibilidade e Desempenho
- A AWS oferece alta disponibilidade e desempenho em todas as suas regiões, incluindo a região de São Paulo. Isso garante que os dados dos sensores estejam sempre acessíveis e que o sistema funcione de maneira eficiente.

### 4. Integração com Serviços AWS
- Ao escolher a região de São Paulo, é possível integrar facilmente outros serviços da AWS, como:
  - **Amazon S3** para armazenamento de dados.
  - **Amazon DynamoDB** para banco de dados NoSQL.
  - **Amazon Kinesis** para processamento de fluxo de dados em tempo real.
- Todos esses serviços podem ser utilizados dentro da mesma região, simplificando a arquitetura e melhorando a eficiência.

### 5. Custos Otimizados
- Embora os custos possam variar entre as regiões, a escolha de uma região local pode reduzir custos associados à transferência de dados (data transfer) entre regiões, especialmente se os dados precisarem ser acessados frequentemente.

## Conclusão
A escolha da região **South America (São Paulo)** é a mais adequada para atender às necessidades de acesso rápido aos dados dos sensores e garantir a conformidade com as restrições legais de armazenamento no Brasil. Além disso, essa escolha oferece:
- Baixa latência.
- Alta disponibilidade.
- Integração perfeita com outros serviços da AWS.

## link youtube:
https://youtu.be/5vHStLiXbRc
