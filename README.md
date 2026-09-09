# Introduction à Python

## Structure du projet

```text
introduction-python/
├── data/
│   └── names/
├── notebooks/
│   └── 1_usa_names.ipynb
├── Initiation à Python 2026.pdf
├── poetry.lock
├── pyproject.toml
└── README.md
```

* `data/` : jeux de données utilisés dans les exercices.
* `notebooks/` : notebooks Jupyter contenant les exercices et exemples.
* `Initiation à Python 2026.pdf` : support de cours.
* `pyproject.toml` : configuration du projet et déclaration des dépendances.
* `poetry.lock` : versions exactes des dépendances installées.

## Prérequis

Avant de commencer, il est nécessaire d'avoir installé :

* **Git**
* **Python 3.11**
* **Poetry**

Le projet utilise Python 3.11 et Poetry pour gérer son environnement virtuel et ses dépendances.

## Installation

### Cloner le dépôt avec git

Depuis un terminal :

```bash
git clone https://github.com/lydiavi/introduction-python.git
cd introduction-python
```
Quelques commandes git utiles : 
```bash
git status
git add .
git commit -m "Description des changements"
git push

git checkout -b "mabranch"
```
### Initialiser le projet avec Poetry

Si le projet est déjà fourni avec un `pyproject.toml`, il n'est pas nécessaire de lancer `poetry init`.

La commande `poetry init` est utile lorsque l'on souhaite **créer un nouveau projet Poetry** à partir de zéro.

```bash
poetry init
```

Elle permet de créer le fichier `pyproject.toml` et de définir les informations du projet ainsi que ses dépendances.

> Dans ce dépôt, le fichier `pyproject.toml` existe déjà. Après avoir cloné le projet, passez directement à `poetry install`.

### Installer les dépendances

Pour installer les dépendances du projet à partir de `pyproject.toml` et du fichier `poetry.lock` :

```bash
poetry install
```

Cette commande crée également l'environnement virtuel Poetry si nécessaire.


## Gestion des dépendances avec Poetry

### Installer une nouvelle dépendance

Par exemple, pour installer `numpy` :

```bash
poetry add numpy
```

Poetry ajoute alors la dépendance dans `pyproject.toml` et met à jour `poetry.lock`.

Pour une dépendance utilisée uniquement pendant le développement :

```bash
poetry add --group dev pytest
```

### Mettre à jour les dépendances

Pour rechercher et installer des versions plus récentes des dépendances autorisées par les contraintes définies dans `pyproject.toml` :

```bash
poetry update
```

Cette commande met également à jour `poetry.lock`.


## Ressources

* [Dépôt GitHub](https://github.com/lydiavi/introduction-python)
* [Documentation Python](https://docs.python.org/3/)
* [Documentation Poetry](https://python-poetry.org/docs/)


Projet d'introduction à Python – 2026.
