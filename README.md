# Análise Exploratória de Dados: Titanic 🚢

Este repositório contém uma análise detalhada sobre o conjunto de dados do Titanic, explorando os fatores que influenciaram a sobrevivência dos passageiros. O projeto utiliza Python e bibliotecas de ciência de dados para transformar dados brutos em insights significativos.

## 🛠️ Limpeza e Tratamento de Dados

A etapa de limpeza foi fundamental para garantir a integridade das análises. Os principais passos incluíram:
- **Tratamento de Dados Ausentes:** Identificação de valores nulos nas colunas `Age`, `Cabin` e `Embarked`.
- **Imputação:** A coluna de idade (`Age`) foi preenchida utilizando a mediana ou baseando-se em títulos (ex: Mr., Miss), enquanto a coluna `Cabin` foi tratada devido ao alto volume de dados faltantes.
- **Conversão de Tipos:** Ajuste de formatos categóricos e numéricos para otimizar o processamento e visualização.

---

## 📊 Insights Principais

### 1. Análise Geral de Gênero
A disparidade entre as taxas de sobrevivência de homens e mulheres é um dos pontos mais marcantes do desastre.
- **Insight:** Mulheres tiveram uma probabilidade de sobrevivência significativamente maior (aproximadamente 74%) em comparação aos homens (cerca de 18%). Isso reflete a política de "mulheres e crianças primeiro" aplicada durante o naufrágio.

![Distribuição de Sobrevivência por Género](/images/distribuicao-de-sobrevivencia-por-genero.png)

### 2. Matriz de Correlação (Heatmap)
A matriz de calor permitiu identificar quais variáveis estavam mais ligadas à sobrevivência (`Survived`).
- **Insight:** Observou-se uma forte correlação negativa entre a Classe (`Pclass`) e a Sobrevivência, indicando que passageiros de classes superiores tinham mais chances de sobreviver. Também notou-se correlação entre o Valor da Passagem (`Fare`) e a Sobrevivência.

![Matriz de Correlação Titanic](/images/matriz-de-correlacao-titanic.png)

### 3. Análise por Faixa Etária
Ao segmentar os passageiros por idade, novos padrões surgiram:
- **Insight:** Crianças (0-12 anos) tiveram uma das maiores taxas de sobrevivência em todas as classes. Por outro lado, adultos na faixa de 18 a 35 anos compunham a maior parte das vítimas, especialmente os do sexo masculino em classes econômicas inferiores.
* **Crianças:**
    ![Correlação Crianças](/images/correlacao-criancas.png)
* **Adultos (Geral):**
    ![Correlação Adultos](/images/correlacao-adultos.png)
![Distribuição de Sobrevivência por Idade](/images/distribuicao-de-sobrevivencia-por-idade.png)

#### Aprofundamento em Correlações por Idade e Classe:
Para entender melhor o impacto em diferentes grupos, analisamos as matrizes de correlação específicas para crianças e adultos, separando também por classes sociais.


* **Adultos (1ª e 2ª Classe):**
    ![Matriz de Correlação Adultos 1 e 2 Classe](/images/matriz-de-correlacao-adultos-1-e-2-classe.png)
* **Adultos (3ª Classe):**
    ![Matriz de Correlação Adultos 3 Classe](/images/matriz-de-correlacao-adultos-3-classe.png)

### 4. Comparação por Classe Social (Socioeconômica)
A classe do passageiro foi um determinante crucial para o destino final.
- **Insight:** - **1ª Classe:** Teve a maior taxa de sobrevivência (acima de 60%).
    - **3ª Classe:** Apesar de ser a mais numerosa, teve a menor taxa de sobrevivência, evidenciando o impacto do status socioeconômico no acesso aos botes salva-vidas.

![Sobrevivência por Classe Social](/images/sobrevivencia-por-classe-social.png)

---

## 📁 Estrutura do Projeto

O projeto está organizado da seguinte forma:
- `data/`: Contém o dataset original (`titanic_train.csv`).
- `notebooks/`: Arquivo principal da análise (`EDA_Titanic.ipynb`).
- `images/`: Pasta contendo todos os gráficos gerados e apresentados acima.

---

**Autores:** Isabelle Euclides & Shaini Dittberner  
**Instituição:** bytes4futures
