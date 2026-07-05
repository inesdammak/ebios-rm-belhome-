# 🔐 Étude de sécurité EBIOS RM — Cas Belhome

Projet réalisé dans le cadre du **Master Data Analytics — OMNES** :
analyse de risque cyber selon la méthode **EBIOS Risk Manager (ANSSI)**.

## Contexte

Belhome, une TPE de bureau d'études techniques, vient de perdre deux
appels d'offres dans des circonstances suspectes. Le dirigeant soupçonne
une fuite d'information. Objectif de l'étude : objectiver la situation par
une analyse de risque structurée (contexte métier → biens essentiels →
événements redoutés → scénarios de menace → évaluation → traitement →
risques résiduels), plutôt que de chercher un coupable.

## Principaux constats

- Le risque vient surtout des **usages physiques quotidiens** (clés USB,
  accès aux locaux) plutôt que d'une cyberattaque sophistiquée.
- 2 risques prioritaires : **compromission des études techniques**
  (priorité 1, critique) et **fuite des données commerciales**
  (priorité 2).
- Mesures à fort effet / coût quasi nul : politique stricte des supports
  amovibles (USB nominatives, chiffrées), durcissement des accès
  physiques, chiffrement au repos.
- Un risque résiduel subsiste après traitement (facteur humain) : géré
  par surveillance continue plutôt qu'éliminé.

## Contenu du dépôt

```
ebios-rm-belhome/
├── README.md
├── .gitignore
└── docs/
    ├── Soutenance_EBIOS_Belhome.pdf
```

## Méthodologie

[EBIOS Risk Manager](https://cyber.gouv.fr/la-methode-ebios-risk-manager)
(ANSSI) — grille Gravité × Vraisemblance, 4 leviers de traitement
(réduire, éviter, transférer, accepter).

## Auteur

Master Data Analytics — OMNES.
