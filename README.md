# ia-setorizacao-patio

Este repositório contém a solução de Inteligência Artificial desenvolvida para o projeto da disciplina de IoT, com o objetivo de **prever automaticamente o setor ideal para motos serem estacionadas em um pátio**, com base em características como tipo da moto, tamanho e ocupação atual do setor.

---

##  Tema
**Setorização inteligente de pátio para entrada e saída de motos** com sugestão automática de alocação, utilizando **Machine Learning** para aprimorar a logística interna de estacionamentos operacionais.

---

##  Problema
Empresas de entrega como a Mottu possuem pátios com centenas de motos, o que torna a **organização manual ineficiente**. Atualmente, a alocação de vagas é feita de forma estática ou pelo próprio operador, o que **gera ocupações desbalanceadas** e **retrabalho operacional**.

---

##  Solução proposta
Desenvolvemos uma IA capaz de:
- Analisar o tipo e tamanho da moto
- Verificar a ocupação atual de cada setor do pátio
- Sugerir o **setor ideal automaticamente**, respeitando regras de negócio (por exemplo, motos pequenas em setores com menor ocupação)

---

##  Bibliotecas Utilizadas
- **Python 3.10+**
- **Pandas** – Para manipulação e simulação dos dados
- **Scikit-learn** – Para pré-processamento e criação do modelo de Machine Learning
- **DecisionTreeClassifier** – Algoritmo usado para classificar os setores ideais

---

##  Arquitetura da IA
### Algoritmo: **Árvore de Decisão**
A arquitetura consiste em:
1. **Geração da base de dados simulada**
2. **Codificação de dados com LabelEncoder**
3. **Treinamento do modelo com DecisionTreeClassifier**
4. **Avaliação com métrica de acurácia**
5. **Previsão para motos novas**

Escolhemos esse algoritmo por ser fácil de interpretar, rápido para treinar e muito adequado para decisões baseadas em regras claras, como no pátio.

---

##  Base de Dados
A base foi **simulada com 100 registros**, contendo:
- Tipo da moto (`Scooter`, `Trail`, `Naked`, `Custom`)
- Tamanho (`Pequena`, `Média`, `Grande`)
- Ocupação do setor (10–100%)
- Setor ideal (A, B ou C)

Gerada automaticamente no Colab.

---

##  Execução (via Google Colab)

 **Notebook utilizado:** `IA_Patio_Mottu.ipynb`


