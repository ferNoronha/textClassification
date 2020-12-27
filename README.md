# Classificação de texto com alguns tópicos do reddit

Projeto de classificação de texto com tópicos do reddit.
Foi utilizado a API do reddit para extrair alguns posts com assuntos variados como ['datascience', 'machinelearning', 'physics', 'astrology', 'conspiracy'] e treinamos as seguintes redes de classificação: Random Forest, Logistc Regression e KNN.

## Installation

Use the package manager [pip](https://pip.pypa.io/en/stable/) to install dependencies.

```bash
pip install numpy
pip install matplotlib
pip install -U scikit-learn
pip install seaborn
pip install config
pip install praw
```

## Usage

Para utilizar você deve inserir suas credenciais da API do reddit.
```python
api_reddit = praw.Reddit(client_id="id",
                     client_secret="secret",
                     password="password",
                     user_agent="testscript by u/fakebot3",
                     username="username")
```

Para rodar o código basta digitar no cmd:

```bash
python Projeto1.py
```
(Lembre-se de estar na mesma pasta do script)

## Result

KNN: 78% de acurácia;

Random Forest: 82% de acurácia;

Logistic Regression: 87% de acurácia;

Obs.: Ainda não foi realizado a engenharia de atributos para melhorar os métodos de classificação.
