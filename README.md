# Gotta Predict 'Em All! 🐾

## Overview
This project leverages data modeling techniques to predict the conditions and locations where rare Pokémon can be encountered in **Pokémon Go**. Inspired by the game's integration of real-world elements, the project uses real-world datasets to provide insights that help players find rare Pokémon efficiently.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Data Sources](#data-sources)
3. [Data Preparation](#data-preparation)
4. [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
5. [Modeling Techniques](#modeling-techniques)
6. [Results](#results)
7. [How to Use](#how-to-use)
8. [Contributors](#contributors)
9. [References](#references)

---

## Introduction
Pokémon Go incorporates augmented reality and real-world mapping to create an engaging experience for players. Rare Pokémon appearances depend on various environmental and locational factors like weather, time of day, and proximity to landmarks. This project uses **classification** and **clustering models** to:
- Predict if rare Pokémon will appear under specific conditions.
- Group rare Pokémon based on their environmental and locational characteristics.

---

## Data Sources
1. **Pokémon Go Spawns (2016 Dataset)**: Includes details such as Pokémon ID, location, time, and weather.
2. **Pokémon Metadata**: Provides additional Pokémon information (e.g., name, type).
3. **Pokémon Rarity Levels**: Specifies the rarity classification of Pokémon.

Datasets were sourced from:
- [Predict 'Em All Dataset](https://www.kaggle.com/datasets/semioniy/predictemall)
- [Pokémon Metadata](https://www.kaggle.com/datasets/maca11/all-pokemon-dataset)
- [Pokémon Rarity Levels](https://web.archive.org/web/20240203201627/https://www.pokego.org/rare-pokemon-list/)

---

## Data Preparation
- **Data Cleaning**: Removed duplicates, handled missing values, and converted data types.
- **Feature Engineering**: Added new features like Pokémon rarity and normalized environmental variables.
- **Integration**: Merged multiple datasets for comprehensive analysis.

---

## Exploratory Data Analysis (EDA)
Key insights:
- Rare Pokémon are more likely to spawn near **PokéStops** and in urban areas.
- Weather significantly influences Pokémon types, with specific types (e.g., Water, Bug) more common in certain conditions.
- Rarity is highest in regions with moderate **population density** and near landmarks.

---

## Modeling Techniques
1. **Classification**: Decision Trees predict whether a Pokémon is rare (`True`) or not (`False`) based on environmental and locational factors.
2. **Clustering**: K-means clustering identifies patterns among rare Pokémon, grouping them by shared conditions (e.g., proximity to landmarks, weather).

---

## Results
- **Classification**:
  - Accuracy: ~61%
  - Precision (Rare Pokémon): ~77%
  - Recall (Rare Pokémon): ~63%
- **Clustering**:
  - Identified 9 distinct clusters of rare Pokémon based on conditions.

---

## How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/gotta-predict-em-all.git
