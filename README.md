# projeto-drosophila
# 🧠 Conectômica e Simulação Neural com NeuPrint

Este projeto realiza a extração, análise gráfica e simulação dinâmica de uma rede neural biológica real baseada no conectoma do cérebro da mosca-das-frutas (*Drosophila melanogaster*). Utilizando os dados públicos fornecidos pelo consórcio **Janelia FlyEM (NeuPrint)**, mapeamos a rede de conexões sinápticas e implementamos uma dinâmica básica inspirada no conceito de **Reservoir Computing** (Computação por Reservatório).

## 🛠️ Tecnologias Utilizadas

* **Python 3**
* **NeuPrint-Python (API)**: Para consulta e extração dos dados reais de sinapses.
* **NetworkX**: Para modelagem e análise da arquitetura do grafo neural.
* **Matplotlib**: Para visualização gráfica personalizada da rede em estilo *dark mode*.
* **NumPy**: Para manipulação algébrica das matrizes de adjacência e dinâmica temporal.

## 📋 Funcionalidades

1. **Extração de Dados Biológicos**: Conexão com o servidor NeuPrint para obter dados estruturais de neurônios e pesos sinápticos.
2. **Modelagem por Grafos**: Conversão das conexões sinápticas em um grafo direcionado (`nx.DiGraph`).
3. **Visualização Avançada**: Renderização personalizada dos 100 neurônios com maior grau de conectividade, mapeados por intensidade de conexões (colormap `plasma`).
4. **Simulação Dinâmica (Reservoir Computing)**: Simulação matemática usando função de ativação não linear (tangente hiperbólica) e propagação do estado de ativação dos neurônios ao longo de passos temporais discretos.

## 🚀 Como Rodar o Projeto

### Pré-requisitos

Antes de executar o notebook, você precisa obter uma chave de acesso (Token) em [Neuprint Janelia](https://neuprint.janelia.org/) e configurá-la nos Segredos do seu Google Colab com o nome de `NEUPRINT_TOKEN`.

### Instalação

```bash
pip install neuprint-python
```

### Estrutura do Repositório

* `Drosophila_Brain_Reservoir.ipynb`: Notebook com todo o fluxo de análise e simulação.
* `README.md`: Documentação explicativa do projeto.

---
Desenvolvido com fins de estudo e portfólio em Inteligência Artificial Biológica e Neurociência Computacional. 🚀
"""
