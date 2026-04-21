# Imagerie Micro-onde Temps Réel — RIS & Problème Inverse

**Université de Rennes, Campus de Beaulieu — Depuis novembre 2025**

## Description
Mise en œuvre d'un système d'imagerie micro-ondes basé sur une 
métasurface reconfigurable (RIS) et une antenne unique. 
Reconstruction d'image par résolution d'un problème inverse.

## Système expérimental
- Surface RIS Greenerwave 8×8 = 64 éléments reconfigurables
- Antenne cornet à 4,1 GHz (λ ≈ 7,3 cm)
- VNA (Vector Network Analyzer) pour mesure du coefficient S11
- Objet cible : cylindre aluminium à ~55 cm de la RIS

## Principe
- 5000 configurations aléatoires de la RIS générées
- Mesure différentielle : ΔΨ = S_obj − S_cal
- Construction de la matrice de mesure H (5000 × 4096)
- Inversion régularisée de Tikhonov (λ = 10⁻³)
- Reconstruction d'image par rétroprojection sur grille 80×80

## Compétences mises en œuvre
- Python : NumPy, SciPy, Matplotlib
- Traitement du signal et imagerie (problème inverse)
- Décomposition en valeurs singulières (SVD)
- Modélisation par matrices de Green et couplages mutuels

## Résultats
- Localisation de l'objet métallique validée à ~(-20cm, -20cm)
- Analyse SVD confirmant la faisabilité de l'approche
- Chaîne de traitement complète opérationnelle

## Contenu du dépôt
- `rapport_imagerie_microonde.pdf` — Rapport complet

## Contact
**Macaire OLUI** — oluimacaire@gmail.com
