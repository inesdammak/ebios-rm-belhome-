# 🔐 Étude de sécurité EBIOS RM — Cas Belhome

Projet réalisé dans le cadre du **Master Data Analytics — OMNES**, portant
sur l'analyse de risque cyber selon la méthode **EBIOS Risk Manager**
(ANSSI).

## 🎯 Ce qui était demandé

L'exercice consistait à mener une **étude de risque cyber complète** sur un
cas d'entreprise fictif (Belhome, un bureau d'études techniques) en
appliquant rigoureusement la méthodologie **EBIOS RM de l'ANSSI**, à
travers ses différents ateliers/modules :

1. **Étude du contexte** — comprendre le métier, les enjeux et le
   périmètre de l'analyse
2. **Identification des biens essentiels et biens supports** — cartographier
   ce qui a de la valeur pour l'entreprise et ce qui l'héberge/le transporte
3. **Construction des événements redoutés** — identifier les scénarios
   d'impact métier à éviter
4. **Analyse des scénarios de menace** — détailler sources de menace,
   vulnérabilités, chaînes d'attaque et impacts
5. **Évaluation des risques** (gravité × vraisemblance) et priorisation
6. **Traitement du risque** — proposer des mesures concrètes (réduire,
   éviter, transférer, accepter) adaptées aux contraintes d'une TPE
7. **Analyse des risques résiduels** après traitement

Le livrable attendu comprenait un **rapport écrit détaillé** et une
**présentation de soutenance**, avec des recommandations opérationnelles
réalistes au regard des moyens limités d'une petite structure.

## 🏢 Le cas Belhome

Belhome est une TPE de 9 personnes (bureau d'études spécialisé dans les
structures pour architectes et promoteurs) qui vient de perdre deux appels
d'offres dans des circonstances inhabituelles. Le dirigeant soupçonne une
fuite d'information, sans preuve. La mission : objectiver la situation par
une analyse de risque structurée plutôt que de chercher un coupable.

## 🔑 Principaux constats

- **Le risque ne vient pas d'une cyberattaque sophistiquée**, mais des
  usages physiques quotidiens : clés USB, accès aux locaux, supports
  amovibles — le véritable point de bascule qui contourne l'isolement
  réseau (air-gap) de l'entreprise.
- **2 événements redoutés priorisés** :
  - **R2 (priorité 1, critique)** — compromission des études techniques
    (savoir-faire, responsabilité professionnelle des ingénieurs)
  - **R1 (priorité 2)** — fuite des données commerciales (prix, marges,
    réponses aux appels d'offres)
- **Mesures à fort effet et coût quasi nul** identifiées : politique
  stricte des supports amovibles (clés USB nominatives, chiffrées,
  journalisées), durcissement des accès physiques, chiffrement au repos.
- Même après traitement, un **risque résiduel non nul subsiste**
  (facteur humain, nécessité opérationnelle d'accès aux données) : il est
  géré par une surveillance continue plutôt que recherché à zéro.

## 📂 Contenu du dépôt

```
ebios-rm-belhome/
├── README.md
├── .gitignore
└── docs/
    ├── Rapport_EBIOS_Belhome.pdf
    └── Soutenance_EBIOS_Belhome.pptx
```

## 🛠️ Méthodologie & référence

- **EBIOS Risk Manager** — méthode de gestion des risques numériques de
  l'[ANSSI](https://cyber.gouv.fr/la-methode-ebios-risk-manager)
- Grille de cotation Gravité × Vraisemblance (échelle 1 à 4)
- 4 leviers de traitement du risque : réduire, éviter, transférer, accepter

## ✍️ Auteur

Master Data Analytics — OMNES.
