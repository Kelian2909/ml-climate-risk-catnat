# Contexte climatique — Bouches-du-Rhône (13)

## Positionnement
Le département des Bouches-du-Rhône (13) est caractérisé par un climat méditerranéen : étés chauds et secs, hivers doux, forte variabilité inter-annuelle. Cette configuration entraîne des tensions hydriques régulières durant la saison chaude (Juin–Août), période où le Soil Wetness Index (SWI) atteint ses minima.

## Saison et circulation
- **Saisonnalité marquée** : pluies concentrées à l’automne et en fin d’hiver ; déficit estival net.
- **Mistral** (flux nord/nord-ouest) : assèchement de l’air, évapotranspiration accrue, amplification des épisodes secs et des contrastes locaux.
- **Épisodes méditerranéens** (automne) : recharges rapides mais hétérogènes → forte dispersion spatiale des cumuls et des recharges de sol.

## Sols et vulnérabilité
- Présence d’**argiles** dans plusieurs secteurs du 13 → sensibilité au **retrait-gonflement des argiles (RGA)**.
- En contexte de sécheresse prolongée, la baisse du SWI accroît le retrait volumique des sols argileux et peut générer des désordres sur le bâti (fissurations, affaissements différentiels).

## Indicateur hydrique : SWI
- **SWI daily (Safran)** : humidité de surface/jusqu’au premier horizon, sensible aux pluies récentes et à l’évapotranspiration.
- **Comportement typique dans le 13** : baisse continue au printemps, **creux en JJA**, remontée avec les épisodes automnaux (si présents).
- Pour l’analyse, le passage **daily → mensuel** permet de suivre les régimes et de stabiliser les cartes à la maille **commune**.

## Enjeux assurantiels (CatNat)
- Les reconnaissances CatNat liées à la sécheresse (souvent associées au RGA) dépendent de **seuils d’intensité/durée** et de la **spatialisation** de l’événement.
- Besoin opérationnel : **cartes prédictives** du SWI et de l’**incertitude** à maille communale, pour éclairer :
  - la **prévention** (ciblage, priorisation),
  - la **souscription/tarification** (différenciation territoriale),
  - la **gestion de portefeuille** (agrégation du risque, scénarios).

## Conséquence méthodologique
- Les contrastes locaux (relief, Mistral, orages d’automne) imposent une **modélisation géostatistique** :
  - **Drift parcimonieux** (variables climatiques + % argiles + polynômes spatiaux x,y),
  - **Variogramme** des résidus (anisotropie possible N–S / E–O),
  - **Krigage universel** pour la prédiction et la **variance de krigeage** σ²_K.
- Les sorties incluent : **μ̂(SWI)**, **σ²_K**, et la **probabilité d’épisode sec** (seuil type q10), afin de traduire le signal en **risque**.

## Hypothèses/limites (à documenter)
- Qualité des interpolations d’entrée (réseau Safran) et des masques communaux (Admin Express).
- Sensibilité aux seuils (q10 vs. seuils “métier”) ; dépendance à la période de référence.
- Incertitudes plus fortes sur zones littorales/relief ou sous influence mistralienne marquée.
