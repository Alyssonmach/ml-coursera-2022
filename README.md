# Exercícios de Machine Learning em Python

Adaptação em Python e Jupyter Notebook de oito exercícios de programação do curso original de Machine Learning de Andrew Ng na Coursera. Os notebooks acompanham uma versão anterior do curso e servem como material de estudo dos algoritmos implementados neles.

> **Escopo:** este repositório não corresponde à especialização atual completa de Machine Learning. A especialização foi atualizada e expandida para três cursos. Este projeto reúne exercícios da versão anterior e cobre apenas parte dos temas e práticas da versão atual. Por exemplo, não inclui árvores de decisão e ensembles, recomendação baseada em conteúdo ou aprendizado por reforço. Consulte a [página oficial da especialização na Coursera](https://www.coursera.org/specializations/machine-learning-introduction) para ver o currículo vigente.

O histórico deste repositório registra a última atualização em **2 de janeiro de 2022**. Portanto, considere os notebooks e as instruções como material legado, não como uma reprodução atualizada do curso.

## Conteúdo

| Pasta | Exercício |
| --- | --- |
| `exercise1/` | Regressão linear |
| `exercise2/` | Regressão logística |
| `exercise3/` | Classificação multiclasse e redes neurais |
| `exercise4/` | Treinamento de redes neurais e backpropagation |
| `exercise5/` | Regressão linear regularizada e viés versus variância |
| `exercise6/` | Máquinas de vetores de suporte (SVM) e classificação de spam |
| `exercise7/` | K-means e análise de componentes principais (PCA) |
| `exercise8/` | Detecção de anomalias e filtragem colaborativa |

Cada pasta de exercício contém o notebook, o módulo `utils.py` com funções auxiliares e, quando necessário, as pastas `Data/` e `Figures/`.

## Estrutura

```text
.
├── exercise1/ … exercise8/
│   ├── Data/                 # dados usados no exercício
│   ├── Figures/              # imagens e gráficos de apoio
│   ├── exerciseN.ipynb       # enunciado e atividades
│   └── utils.py              # funções auxiliares
├── requirements.txt          # dependências Python
└── submission.py             # integração legada com o avaliador Coursera
```

## Como executar

Use Python 3 e instale as dependências em um ambiente virtual:

```bash
python3 -m venv .venv
source .venv/bin/activate
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
jupyter lab
```

No Windows, ative o ambiente com:

```powershell
.venv\Scripts\Activate.ps1
```

No JupyterLab, abra o notebook do exercício desejado, por exemplo `exercise1/exercise1.ipynb`, e execute as células em ordem. Os notebooks contêm instruções e código de estudo; a execução local não exige uma conta Coursera.

## Envio para avaliação

O arquivo `submission.py` implementa a integração usada pelos avaliadores dos exercícios originais. Ela pode depender de endpoints, tokens e regras da plataforma que mudaram desde a criação do curso; por isso, não é necessária para estudar ou executar os notebooks localmente.

O código de envio salva credenciais em um arquivo `token.pkl` no diretório de execução. Mantenha esse arquivo privado e não compartilhe tokens. Se você já enviou um token válido para um repositório remoto, revogue-o na plataforma, se possível.

## Referência do curso atual

A [especialização atual de Machine Learning](https://www.coursera.org/specializations/machine-learning-introduction), criada pela DeepLearning.AI e Stanford Online, é uma versão atualizada e expandida do curso pioneiro. O currículo e os materiais oficiais podem mudar; consulte a página da especialização para obter a descrição mais recente.
