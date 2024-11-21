# kaggle-titanic

## Sobre o Projeto
Este projeto de estudo aborda a competição "Titanic - Machine Learning from Disaster" do Kaggle. O objetivo é prever quais passageiros sobreviveram ao naufrágio do Titanic com base em informações como idade, sexo, classe, entre outras.

O projeto foi desenvolvido utilizando Python e bibliotecas populares de aprendizado de máquina e análise de dados.

---

## Estrutura do Projeto
O projeto está dividido em 4 etapas principais:

1. **Instalação das Dependências**: Configuração do ambiente com as bibliotecas necessárias.
2. **Análise Exploratória dos Dados (EDA)**: Análise dos dados para entender padrões e identificar relações entre variáveis.
3. **Pré-processamento dos Dados**: Limpeza, codificação e transformação dos dados para uso em modelos de aprendizado de máquina.
4. **Criação do Modelo**: Implementação de uma Rede Neural Multicamadas (MLP) para prever a sobrevivência dos passageiros.
5. **Análises Finais e Submissão**: Avaliação do modelo e criação do arquivo para submissão no Kaggle.

---

## Instalação
As bibliotecas utilizadas incluem:

- **Análise de Dados**: `pandas`, `numpy`, `matplotlib`, `seaborn`
- **Machine Learning**: `scikit-learn`, `tensorflow`, `keras`

Execute o comando abaixo para instalar as dependências:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn keras tensorflow
```

---

## Como Rodar o Projeto
1. **Clonar o repositório** ou acessar o arquivo do Colab diretamente pelo link fornecido.
2. Certifique-se de ter as bibliotecas instaladas no ambiente de execução.
3. Execute as células do notebook passo a passo, desde a análise exploratória até a geração do arquivo de submissão.

---

## Análise Exploratória dos Dados
Alguns insights obtidos durante a análise dos dados incluem:
- Passageiros da 1ª classe têm maior probabilidade de sobrevivência.
- Mulheres têm maior taxa de sobrevivência em relação aos homens.
- Passageiros que pagaram tarifas mais altas têm maior chance de sobreviver.

---

## Pré-processamento dos Dados
O pipeline de pré-processamento inclui:
- **Imputação**: Tratamento de valores ausentes na coluna `Age` usando a média.
- **Codificação**: Conversão de variáveis categóricas (`Sex` e `Embarked`) para valores numéricos.
- **Remoção de Colunas**: Exclusão de variáveis irrelevantes como `Name`, `Ticket` e `Cabin`.

Os dados transformados foram salvos em arquivos `.csv` e `.pkl` para uso posterior.

---

## Modelo de Machine Learning
- **Arquitetura**: Rede Neural Multicamadas (MLP) com camadas densas e ativação ReLU.
- **Compilação**: Otimizador `Adam`, função de perda `binary_crossentropy` e métrica de acurácia.
- **Treinamento**: Dados de treino divididos em 80% para treinamento e 20% para validação.

---

## Resultados
- **Curvas de Erro e Acurácia**: Demonstram o desempenho do modelo ao longo das épocas.
- **Matriz de Confusão**: Avaliação final no conjunto de validação.
