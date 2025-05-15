<p align="center">
   <img src="https://www.asc-csa.gc.ca/images/satellites/planck/planck-animation.jpg" alt="Planck Space Telescope with stylized Cosmic Microwave Background colours over a space backdrop" height=300> 
   <br> Crédit d'image | Image credit: <a href=https://www.asc-csa.gc.ca/images/satellites/planck/planck-animation.jpg>ASC-CSA</a>
</p>

<p align="center">
 <a href="#stars">
  <img alt="Étoiles sur GitHub | GitHub Repo stars" src="https://img.shields.io/github/stars/asc-csa/Planck-Telescope-Data-Tutorial">
 </a>
 <a href="#watchers">
  <img alt="Spectateurs sur Github | GitHub watchers" src="https://img.shields.io/github/watchers/asc-csa/Planck-Telescope-Data-Tutorial">
 </a>
 <a href="https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/tree/main/commits/main">
  <img alt="Dernier commit sur GitHub | GitHub last commit" src="https://img.shields.io/github/last-commit/asc-csa/Planck-Telescope-Data-Tutorial">
 </a>
 <a href="https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/tree/main/graphs/contributors">
  <img alt="Contributeurs sur GitHub | GitHub contributors" src="https://img.shields.io/github/contributors/asc-csa/Planck-Telescope-Data-Tutorial">
 </a>
 <a href="https://twitter.com/intent/follow?screen_name=csa_asc">
  <img alt="Suivre sur Twitter | Twitter Follow" src="https://img.shields.io/twitter/follow/csa_asc?style=social">
 </a>
</p>

<h2 align="center">
  <a href="#titre-du-projet">Français</a> |
  <a href="#project-title">English (follows)</a>
</h2>

<a id="titre-du-projet"></a>
# Données du télescope spatial Planck - Tutoriel

> **Description brève :**
> Ce tutoriel rend les données du satellite Planck plus accessibles en montrant comment les importer, les visualiser et les analyser pour explorer les conditions de l’Univers primordial.

---

## À propos
La mission du satellite Planck est la première mission européenne vouée à l'étude de la naissance de l'Univers. Le télescope spatial Planck a été lancé conjointement avec l'Observatoire spatial Herschel à bord d'une fusée Ariane 5, le 14 mai 2009. Il s'agit du télescope spatial le plus sensible jamais conçu pour étudier le rayonnement cosmique de fond, c'est-à-dire les résidus du rayonnement issu du Big Bang qui se sont produits il y a 13,8 milliards d'années. Le télescope spatial Planck mesure la température du rayonnement fossile cosmologique et recherche les régions plus chaudes ou froides que la moyenne. Ces faibles fluctuations de température, nommées anisotropies, seraient à l'origine des galaxies qui existent aujourd'hui.

Le télescope spatial Planck fournira aux astronomes un aperçu des conditions qui régnaient au début de l'Univers. L'objectif de la mission est d'aider à répondre à certaines des grandes questions de la science moderne. Comment l'Univers s'est-il formé? Comment a-t-il évolué jusqu'à sa forme actuelle? Quelle forme prendra-t-il dans l'avenir? Les scientifiques espèrent ainsi établir quelle théorie explique le mieux l'origine de l'ensemble des structures cosmiques.

Le but de ce tutoriel est de faire connaître les données de la mission et d’améliorer leur accessibilité. Ce tutoriel vous enseigne sur la façon d’importer les fichiers FITS, d’accéder aux informations des entêtes, de manipuler les données HEALPix, de visualiser les données sur une carte du ciel et d’effectuer des analyses de base avec les données.

## Prérequis
- Assurez-vous d'installer les bibliothèques nécessaires à faire fonctionner le tutoriel.
  
## Démarrage rapide

1. 📦 **Cloner le dépôt**
   ```bash
   git clone https://github.com/asc-csa/Planck-Telescope-Data-Tutorial.git
   cd Planck-Telescope-Data-Tutorial/Code
   ```
2. 🐍 **Créer un environnement**
   ```bash
   # Avec virtualenv
   python -m venv env
   source env/bin/activate

   # Ou avec conda
   conda create -n jwst_env 
   conda activate jwst_env
   ```
3. 📥 **Installer les dépendances**
   ```bash
   pip install -r requirements.txt
   ```
4. 🚀 **Lancer le tutoriel**
   ```bash
   jupyter notebook Planck_Telescope_Data_Tutorial.ipynb.ipynb
   ```
> **Remarque :** Si les graphiques ou cartes ne s’affichent pas, redémarrez Jupyter Notebook ou ajoutez `%matplotlib inline` dans la première cellule.

## Fonctionnalités

Veuillez noter que le code de ce didacticiel repose sur la bibliothèque Python [Healpy](https://healpy.readthedocs.io/en/latest/index.html), qui ne prend pas en charge Windows en mode natif. Il est recommandé d'exécuter ce tutoriel dans un environnement Linux. Si vous souhaitez exécuter le code sur Windows, veuillez utiliser [l'émulateur Linux de Windows](https://learn.microsoft.com/en-us/windows/wsl/install) et vous assurez que WSL est actif sur votre ordinateur.

Si vous souhaitez interagir directement avec le notebook:

1. Télécharger le fichier du tutoriel [Planck_Telescope_Data_Tutorial.ipynb](https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/blob/main/Code/Planck_Telescope_Data_Tutorial.ipynb).
2. Si vous n’avez pas encore utilisé Jupyter Notebooks, installez-le avec:<br>
``` pip install notebook ```
3. Entrez la commande suivante pour lancer un serveur Jupyter Notebook local:<br>
``` jupyter notebook ```
4. Ouvrez le lien web qu’il fournit dans votre navigateur et lancez le didacticiel.

Vous pouvez aussit utiliser le code directement dans vos propres scripts Python.

## Licence

Ce projet est  sous une licence MIT modifiée – voir le fichier [LICENSE](https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/blob/main/LICENSE.txt) pour plus de détails.

---

<h2 align="center">
  <a href="#project-title">English </a> |
  <a href="#titre-du-projet">Français (précède)</a>
</h2>

<a id="project-title"></a>
# Planck Space Telescope Data Tutorial

> **Brief description:**
> This tutorial improves access to Planck satellite data by showing how to import, visualize, and analyze it to explore conditions in the early Universe.

---

## About
Planck is ESA's first mission to study the birth of the Universe. Planck was launched jointly with the Herschel Space Observatory aboard an Ariane 5 rocket, on May 14, 2009. The satellite is the most sensitive telescope ever designed to study the cosmic microwave background--the remnants of radiation from the Big Bang 13.8 billion years ago. Planck's detectors measure the temperature of this light, searching for regions that are slightly warmer or colder than the average. These small fluctuations in temperature, called anisotropies, provided the seeds for the formation of galaxies that exist today.

The Planck satellite is giving astronomers a glimpse of conditions near the beginning of the Universe. The mission's objective is to help answer some fundamental questions of modern science: How was the Universe formed? How has it evolved to its present form? And what shape will it take in the future? Scientists thereby hope to establish which theory best explains the origin of all cosmic structures.

The purpose of this tutorial is to raise awareness of this data and enhance its accessibility. In this tutorial, you are provided examples of how to import FITS files, access header information, manipulate the HEALPix data, visualize skymaps, and conduct basic analyses of the data in Python. 

## Prerequisites
- Make sure to install the requirements for the tutorial.

## Quick Start

1. 📦 **Clone the repo**
   ```bash
   git clone https://github.com/asc-csa/Planck-Telescope-Data-Tutorial.git
   cd Planck-Telescope-Data-Tutorial
   ```
2. 🐍 **Create environment**
   ```bash
   # Using virtualenv
   python -m venv env
   source env/bin/activate

   # Or using conda
   conda create -n jwst_env 
   conda activate jwst_env
   ```
3. 📥 **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```
4. 🚀 **Run the tutorial**
   ```bash
   jupyter notebook Planck_Telescope_Data_Tutorial.ipynb.ipynb
   ```
> **Note:** If plots or maps do not display, restart Jupyter Notebook or run `%matplotlib inline` in the first cell.

## Functionality
Please note that the code in this tutorial relies on the [Healpy](https://healpy.readthedocs.io/en/latest/index.html) Python library, which does not support Windows natively. Linux is recommended to run this tutorial. If you wish to run the code on Windows, please use the [Windows Subsystem for Linux](https://learn.microsoft.com/en-us/windows/wsl/install) and make sure to enable WSL on your computer.

If you wish to interact with the notebook directly:

1. Download the tutorial file [Planck_Telescope_Data_Tutorial.ipynb](https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/blob/main/Code/Planck_Telescope_Data_Tutorial.ipynb).
2. If you have not previously used Jupyter Notebooks, install it with:<br>
``` pip install notebook ```
3. Enter the following command to launch a local Jupyter Notebook server:<br>
``` jupyter notebook ```
4. Open the URL it provides in your browser, and experiment with the tutorial.

Otherwise, you may simply use the code directly in your own Python scripts.

## License

This project is licensed under a modified MIT license - see the [LICENSE](https://github.com/asc-csa/Planck-Telescope-Data-Tutorial/blob/main/LICENSE.txt) file for details.

---

