# Exploitation de données électorales avec Python

Évaluation intermédiaire — *Python pour la data science*  
Auteur : SERVANT Lucas, GOUALOU Maxence, DELETANG Arthur  
Chargé de TD : BEROVA Raya

---

## Objectif

Explorer les données électorales du **premier tour de l'élection présidentielle française 2022** à l'échelle communale et départementale, en étudiant notamment la surreprésentation territoriale de chaque candidat.

---

## Structure du dépôt

```
.
├── dm_elections_2022.ipynb   # Notebook principal (analyses + visualisations)
├── utils.py                  # Fonctions utilitaires (formatage des nombres et scores)
├── requirements.txt          # Dépendances Python
└── README.md                 # Ce fichier
```

---

## Données

Les données proviennent du portail [data.gouv.fr](https://www.data.gouv.fr/fr/datasets/r/182268fc-2103-4bcb-a850-6cf90b02a9eb) et sont chargées directement depuis le notebook via une URL publique — aucun téléchargement manuel n'est nécessaire.

Le fond de carte des départements est récupéré automatiquement via la librairie `cartiflette`.

---

## Installation et utilisation

**1. Cloner le dépôt** — ouvrir un terminal et exécuter :

```bash
git clone https://github.com/Luservant/DM_python.git
```

**2. Ouvrir le dossier** `DM_python` qui vient d'être créé.

**3. Ouvrir un terminal dans ce dossier** et exécuter :

```bash
pip install -r requirements.txt
jupyter lab dm_elections_2022.ipynb
```

Le notebook est **entièrement reproductible** : un clic sur *Run All* suffit à reproduire l'ensemble des analyses et visualisations.

---

## Contenu du notebook

| Section | Description |
|---|---|
| **1. Explorations générales** | Nettoyage des données, construction du code commune, comptage des candidats, scores nationaux et départementaux |
| **2. Comparaison aux moyennes nationales** | Calcul de la surreprésentation départementale, visualisation en barres horizontales |
| **3. Cartographie** | Cartes choroplèthes de la surreprésentation par département pour chaque candidat |
