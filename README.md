# Global Suicide Analysis Project

## Description

Ce projet analyse les taux de suicide dans le monde en fonction de divers facteurs socio-économiques et démographiques comme l'espérance de vie, la mortalité infantile, la consommation d'alcool, et le niveau d'éducation.

Nous utilisons un dataset mondial pour explorer les corrélations, visualiser les tendances historiques, et comprendre les facteurs qui influencent les taux de suicide.

## Objectif

A partir d’un jeu de données libre, réaliser une visualisation de votre choix.

---

## <u>Table de matière :</u>

- [Introduction](#introduction)
- [Fonctionnalités principales](#fonctionnalités)
- [Installation](#installation)
- [Structure du projet](#project-structure)
- [Visualisation des données](#data_visualisation)
- [Usage](#usage)
- [Crédits](#credits)
- [Conclusion](#conclusion)

---

## <a id="introduction"><u>Introduction: </u></a>

Ce dataset porte sur le taux de suicide dans le monde.
Dans le cadre de ce projet, j'ai choisi de travailler avec un dataset venant de kaggle :

- **Source :** [Kaggle - Global Suicide Rates Dataset](https://www.kaggle.com/code/youssefabdelghfar/global-suicide-rates/input)
- **Colonnes principales :**
  - `Country`
  - `Year`
  - `Suicides_number`
  - `Life_expectancy`
  - `Adult_mortality`
  - `Infant_deaths`
  - `Alcohol`
  - `GDP`
  - `Population`
  - `Schooling`
  - ...

---

## <a id="fonctionnalités"><u>Fonctionnalités principales: </u></a>

- Extraction des données 
- Analyse exploratoire (EDA)
- Nettoyage des données
- Transformation et enrichissement des données
- Visualisations interactives :
  - Carte mondiale du taux de suicide
  - Diagramme Coxcomb (Rose Chart)
  - Heatmaps de corrélation
  - Bar charts des pays avec le plus grand nombre de suicides
  - Scatter plots colorés suicide par niveau d'éducation
- Dashboard interactif avec Metabase (optionnel)

Avant tout cela, il est important de noter que ce projet contient un fichier requirements contenant 
toutes les librairies nécessaires pour la réalisation du projet.

Pour installer le projet il est utile de suivre les étapes suivantes :

---

## <a id="installation"><u>Installation:</u></a>

Lorsque vous initialisez le projet, il faut installer toutes les librairies avec la commande suivante :

1. Clonez le repository :

```bash
  git clone https://github.com/BRENHINES/Visualisation_TD.git
  cd Visualisation_TD
```

2. Créez un environnement virtuel et installez les dépendances :

```bash
  python -m venv venv
  source venv/bin/activate  # (Linux/macOS)
  venv\Scripts\activate     # (Windows)
    
  pip install -r requirements.txt
```

---

## <a id="project-structure"><u>Structure du projet:</u></a>

La structure du projet est comme suit :

```bash
📂 Visualisation_TD (project-root)
│── 📂 content                    # Raw data folder
│──── 📂 sample_data              # raw data folder
│────── 📜 Dataset_Final.csv      # Raw data files
│── 📜 Visualisation TD.ipynb     # Python scripts for automation in Jupyter Notebook
│── 📜 requirements.txt           # Dependencies
│── 📜 README.md                  # Documentation (this file)
```

---

## <a id="data_visualisation"><u>Visualisation des données:</u></a>

Dans le cadre de ce projet, plusieurs visualisations ont été créées pour mieux comprendre et analyser les données sur le taux de suicide dans le monde :

- Line plot
- Diagrammes Coxcomb pour l'éducation et le suicide 
- Heatmaps des corrélations entre facteurs 
- Scatter plots éducation vs suicides 
- Treemap pays et taux de suicide

Ces visualisations permettent de :
- Mieux comprendre l'évolution historique du phénomène.
- Comparer les pays et régions les plus touchées.
- Analyser les corrélations possibles entre facteurs sociaux (éducation, consommation d'alcool, espérance de vie) et les taux de suicide.

---

### 1. Line Plot : Évolution du taux de suicides dans le monde au fil du temps

Ce graphique en courbe montre l'évolution du nombre total de suicides dans le monde au fil des années 
pour identifier les tendances mondiales sur la durée (hausse ou baisse des suicides au fil du temps).

---

### 2. Bar Plot : Classement des pays avec le plus de suicides

Ce diagramme en barres présente les pays ayant enregistré le plus grand nombre de suicides. 
Il permet d'identifier les tendances mondiales sur la durée (hausse ou baisse des suicides au fil du temps).

---

### 3. Carte géographique : Taux de suicides par pays (par 100 000 habitants)

Cette carte colore les pays en fonction de leur taux de suicides (nombre de suicides rapporté à 100 000 habitants).
Permet de visualiser géographiquement les régions du monde les plus affectées.

---

### 4. Graphique de régression linéaire : Corrélation entre deux variables

Ce graphique montre la relation entre la consommation d'alcool et le nombre de suicides par pays.
Ce diagramme permet de détecter s’il existe une corrélation linéaire entre deux facteurs.

---

### 5. Histogramme : Distribution d'une variable

L'histogramme présente la distribution de l'espérance de vie (Life_expectancy) dans les données.
on peut ainsi comprendre la répartition de l'espérance de vie dans les différents pays/années.

---

### 6. Scatter Plot coloré par groupe de scolarisation

Ce nuage de points présente la relation entre le niveau moyen de scolarisation et le nombre de suicides, colorée par groupe d'années d'études (Faible, Moyenne, Élevée, Très Élevée).
Il nous permet d'observer comment l'éducation pourrait influencer le taux de suicide.

---

## <a id="usage"><u>Usage:</u></a>

Pour utiliser le projet, il faut exécuter le script principal :

Dans le fichier `Visualisation TD.ipynb`, il suffit de taper les touches `Shift + Enter` pour exécuter chaque cellule.

Vous pouvez également exécuter le script Python directement :

```bash
  python Visualisation_TD.py
  python main.py
```

---

## <a id="credits"><u>Crédits:</u></a>

- Dataset original : [Kaggle - Global Suicide Rates Dataset](https://www.kaggle.com/code/youssefabdelghfar/global-suicide-rates/input)
- Outils et librairies : Python, Pandas, Matplotlib, Seaborn, Plotly

---

## <a id="conclusion"><u>Conclusion:</u></a>

Ce projet d'analyse des taux de suicide dans le monde nous a permis de mieux comprendre un phénomène complexe aux implications sociales, économiques et sanitaires profondes.

À travers une série d'étapes méthodiques — du nettoyage des données jusqu'à la visualisation — nous avons :

- Préparé et enrichi un jeu de données mondial brut,
- Analysé les principales tendances temporelles et géographiques,
- Exploré les corrélations potentielles entre des facteurs tels que l'éducation, l'espérance de vie, la consommation d'alcool et les taux de suicide,
- Construit des visualisations variées (cartes, courbes, diagrammes de corrélation, scatter plots) pour rendre l'information accessible et compréhensible.

Ces analyses visuelles ont permis de dégager plusieurs enseignements clés :
- Certaines régions du monde présentent des taux de suicide significativement plus élevés,
- Le niveau d'éducation et certains facteurs socio-économiques semblent être liés aux variations de ces taux,
- L’évolution temporelle montre des dynamiques qui peuvent être corrélées à des contextes socio-économiques globaux.

Enfin, ce projet illustre l'importance de la visualisation de données dans l'analyse exploratoire : rendre les données visibles permet de mieux comprendre et communiquer des réalités souvent complexes.