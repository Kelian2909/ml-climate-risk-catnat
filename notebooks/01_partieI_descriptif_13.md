# Partie I — Descriptif (Département 13)

**Contexte (rappel).** Le 13 présente une forte saisonnalité du SWI (creux JJA), influencée par le Mistral et des recharges automnales hétérogènes. La présence d’argiles accroît la vulnérabilité RGA. On cherche des cartes **μ̂(SWI)** et **incertitudes** à la maille **commune** pour éclairer CatNat.


A. Setup (imports, chemins, CRS=2154)
B. Chargement des données (communes 13, SWI mensuel, argiles)
C. QA & complétude (NA, histogrammes)
D. Cartes (médiane SWI, % argile)
E. Séries temporelles (département 13, focus JJA)
F. Corrélations simples (Spearman)  ← descriptif, pas de modèle
G. Baselines & métriques
   G1. Baseline 0 : Climatologie (médiane historique par commune×mois)
   G2. Baseline 1 : Drift seul (Ridge/ElasticNet) – RMSE/MAE
H. Exports figures & tableaux
