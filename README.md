# ☣️ Toxic Gas Detection Challenge - Bertin Technologies

## 🧪 Contexte

Ce dépôt correspond à notre participation au challenge **"Identification des gaz toxiques"** proposé par **Bertin Technologies** sur la plateforme [Challenge Data](https://challengedata.ens.fr/challenges/156).

L'objectif est d'améliorer la **détection et l'identification des gaz toxiques** à l'aide de **modèles de machine learning**, afin de renforcer la sécurité dans des contextes industriels ou en situation de conflit.

---

## 🎯 Objectif

Développer un modèle capable de **prédire les niveaux d'alarme** pour **23 classes de gaz** toxiques, à partir des mesures de capteurs intégrés dans un **dispositif portable de détection de gaz**.

---

## 📊 Description du jeu de données

Le dataset fourni contient environ **330 000 échantillons**, répartis équitablement entre **train** et **test**. Chaque échantillon comprend :

- `ID` : identifiant unique
- `M4` à `M7` et `M12` à `M15` : mesures de deux groupes de capteurs physiquement proches
- `S1`, `S2`, `S3` et `R` : mesures de quatre capteurs complémentaires
- `Humidity` : humidité absolue (unités arbitraires)

### 🎯 Labels (train uniquement)
- 23 colonnes correspondant aux **classes de gaz**, chacune représentant un **niveau d’alarme** compris entre 0 et 1.

> **Remarque :** Les conditions physiques comme l’humidité et la concentration des gaz dans l’ensemble de **test** diffèrent souvent de celles de l’ensemble d’entraînement, ce qui rend le problème plus réaliste et complexe.

---

## 🧠 Type de problème

- **Problème de régression supervisée multi-sorties**
- Objectif : prédire 23 valeurs continues (entre 0 et 1) par échantillon

---
