[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Rapprochement des stocks multi-nœuds et analyse des pertes | Modèle Excel Shopify et 3PL
<img width="1920" height="790" alt="image" src="https://github.com/user-attachments/assets/6689bffe-1aac-43d7-9f63-6e85a14470f0" />


[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Browser + Excel](https://img.shields.io/badge/Platform-Browser%20%2B%20Excel-217346.svg)](#quick-start-tutorial-how-to-automate-your-inventory-reconciliation)
[![Tool Type: Decision Support](https://img.shields.io/badge/Tool%20Type-Decision%20Support-2251FF.svg)](#what-it-helps-you-track-inventory-pain-points-vs-solutions)

**Un tableur de rapprochement des stocks automatisé et un modèle d'analyse des pertes conçus pour les marques de commerce électronique multicanal. Comparez instantanément les niveaux de stock Shopify, les enregistrements internes du système de gestion d'entrepôt (WMS) et les comptages physiques de la logistique tierce (3PL) pour localiser les écarts et traduire les pertes d'unités en impact financier direct — sans écrire de formules VLOOKUP ni reconstruire des rapports chaque mois.**

**Sans inscription. Sans installation. Gratuit dans votre navigateur.**

Testez vos données opérationnelles dans la version navigateur gratuite en un instant. Pour les clôtures mensuelles récurrentes et la sécurité des données hors ligne, passez au modèle Excel entièrement débloqué avec une garantie de remboursement de 30 jours sans question.

> 🌐 **Ouvrir le tableau de bord interactif**  
> [Essayer le simulateur de rapprochement des stocks 3PL gratuit dans le navigateur](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
> 
> 📥 **Obtenir le tableur réutilisable**  
> [Télécharger le modèle Excel d'analyse des pertes et d'audit des stocks](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)

---

## Ce qu'il permet de suivre : points de douleur des stocks vs. solutions

Au lieu de se contenter d'identifier que « les chiffres ne correspondent pas », cette boîte à outils traduit les différences de stock brutes en un plan d'action financier.

| Point de douleur des stocks e-commerce (le « pourquoi ») | Solution de rapprochement (le « comment ») |
| :--- | :--- |
| **Angles morts inter-systèmes :** vous ignorez quel système (Shopify vs. 3PL vs. WMS) détient la vérité terrain pour le stock disponible. | **Triangulation multi-nœuds :** aligne côte à côte les quantités déclarées par les systèmes pour localiser précisément où les synchronisations de données échouent. |
| **Perte financière non quantifiée :** traiter un écart de 20 unités sur un article à 5 $ de la même manière qu'un article à 50 $. | **Analyse des écarts pondérée par le coût des marchandises vendues (COGS) :** multiplie les écarts d'unités par le coût du SKU pour révéler la véritable exposition à la dépréciation financière. |
| **Fuite logistique tierce (3PL) :** vous soupçonnez vos partenaires d'exécution de perdre du stock, mais sans preuve concrète pour les réclamations SLA. | **Suivi du taux d'écart :** isole les taux d'écart entre la 3PL et l'entrepôt interne pour construire une base factuelle de réclamations contractuelles de perte. |
| **Paralysie analytique face aux données brutes :** faire défiler des milliers de lignes de feuilles de comptage cyclique pour trouver des erreurs. | **Tableaux de bord par exception :** classe automatiquement les « 10 premiers SKU par valeur de perte » pour prioriser les investigations du management. |

---

## Tutoriel de démarrage rapide : comment automatiser votre rapprochement des stocks

Transformez des exports multi-sources désordonnés en un audit des stocks de niveau direction en quatre étapes structurées.

### Étape 1 : configurez vos données de référence SKU (configuration unique)
Accédez à la feuille `Config_Master`. Définissez votre nomenclature SKU standard, le coût unitaire (COGS) et les seuils d'alerte spécifiques à votre activité (par ex., signaler tout écart > 5 unités ou > 100 $ de valeur). Cette référence garantit que toutes les données entrantes sont mesurées par rapport à une source de vérité unique.

### Étape 2 : importez les exports WMS, 3PL et Shopify
Contournez la normalisation manuelle des données. Collez vos exports CSV bruts directement dans leurs onglets désignés :
*   `Import_Shopify` (la disponibilité de votre vitrine)
*   `Import_WMS` (vos enregistrements d'entrepôt internes)
*   `Import_3PL` (vos comptages physiques d'exécution externe)
*Remarque : le système est conçu pour ingérer directement les exports bruts — aucune suppression manuelle de colonnes ni reconstruction requise.*

### Étape 3 : générez le tableau de bord des pertes et examinez les exceptions
Accédez à la sortie `Dashboard`. Le moteur de rapprochement automatisé nettoie instantanément la mise en forme, aligne les SKU et calcule les écarts. Examinez vos écarts de stock de plus forte valeur, la valeur totale des pertes et les taux de précision nœud à nœud sans calculer manuellement une seule cellule.

### Étape 4 : établissez une routine et téléchargez pour un usage répété
Pour votre premier audit, utilisez la version navigateur pour identifier immédiatement les problèmes de stock. Pour établir une cadence robuste de contrôle des stocks mensuel, exportez le système pour un usage à long terme.

👉 **Action requise :** une fois votre flux de travail validé, **[téléchargez ici le modèle Excel de rapprochement des stocks réutilisable](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**. Le mois prochain, collez simplement le nouvel instantané des stocks par-dessus les anciennes données — toute l'analyse des écarts se rafraîchira automatiquement.

---

## La logique métier et la méthodologie

Cette boîte à outils est conçue autour de principes professionnels d'audit, déplaçant l'accent de l'agrégation des données vers la protection proactive des actifs. Voici la méthodologie opérationnelle qui alimente le classeur :

### 1. Méthodologie : le rapprochement des stocks à trois voies
*   **La méthode :** à la manière des audits financiers des comptes fournisseurs, ce cadre emploie un **principe de rapprochement à trois voies** entre les ventes numériques (Shopify), le suivi interne (WMS) et le stockage physique (3PL). 
*   **L'impact métier :** cela met fin au « jeu du reproche ». En triangulant les données, les responsables des opérations peuvent déterminer si un problème est une erreur de synchronisation de la vitrine (décalage d'API) ou une perte physique d'exécution (perte), réduisant considérablement le temps de résolution.

### 2. Méthodologie : priorisation par valeur financière à risque (VaR)
*   **La méthode :** les écarts sont intrinsèquement pondérés par le coût des marchandises vendues (COGS). La couche de calcul transforme l'`Écart d'unités` en `Exposition à la dépréciation financière`.
*   **L'impact métier :** cela optimise l'allocation de la main-d'œuvre. Au lieu que le personnel d'entrepôt consacre 4 heures à enquêter sur un écart de 50 unités de pochettes matelassées, il est redirigé par le tableau de bord vers un écart de 3 unités sur de l'électronique à marge élevée.

### 3. Méthodologie : rapports par exception
*   **La méthode :** la boîte à outils filtre des milliers de SKU concordants en une liste condensée d'exceptions opérationnelles basée sur des seuils de tolérance définis par l'utilisateur (par ex., perte acceptable < 0,5 %).
*   **L'impact métier :** cela crée un **raisonnement industrialisé**. Le directeur de la chaîne d'approvisionnement ne regarde pas un dump de données ; il regarde une liste d'actions concrètes pour la correction des processus internes ou le dépôt de réclamation 3PL.

---

## Scénarios concrets : quand utiliser ce modèle d'audit des stocks

Ce système est spécialement conçu pour les points d'inflection critiques de la chaîne d'approvisionnement où la précision du stock physique dicte la santé financière.

*   **Scénario A : clôture financière de fin de mois.** Les équipes financières ont besoin d'un chiffre exact de dépréciation COGS pour la comptabilité. Utilisez ce modèle pour calculer la valeur exacte en dollars des stocks perdus dans tous les entrepôts le dernier jour du mois.
*   **Scénario B : litiges contractuels SLA 3PL.** Vous soupçonnez votre partenaire d'exécution de perdre de la marchandise au-delà de l'allocation de perte de 1,5 %. Utilisez la comparaison multi-nœuds pour générer un rapport de réclamation documenté pour les SKU manquants de forte valeur.
*   **Scénario C : prévention des ruptures en haute saison (T4/Black Friday).** Shopify affiche 100 unités, mais la 3PL n'en a que 20. Exécutez ce rapprochement chaque semaine pendant le T4 pour détecter le « stock fantôme » avant que les clients n'achètent du stock que vous ne détenez pas physiquement, évitant ainsi des taux de remboursement massifs et des tickets de support client.

---

## Problèmes courants des opérations de stock que cela résout

| Problème des opérations de stock | Processus manuel sur tableur | Solution du modèle automatisé |
| :--- | :--- | :--- |
| **Trois systèmes disparates en désaccord** | Les opérateurs exécutent manuellement `INDEX/MATCH` sur les fichiers Shopify, WMS et 3PL, augmentant les risques de références cassées. | Une couche de rapprochement standardisée aligne automatiquement toutes les unités de gestion des stocks (SKU). |
| **Mise en forme désordonnée des données exportées** | Les lignes vides, les espaces de fin et les SKU sensibles à la casse créent de fausses erreurs de non-concordance. | La couche de calcul normalise les chaînes et les types de données avant la vérification des écarts. |
| **La perte n'est mesurée qu'en unités** | Le management voit un déficit d'unités mais ne peut pas estimer précisément l'impact COGS. | La matrice de coûts SKU intégrée convertit les déficits de quantité en dépréciations financières estimées. |
| **Les grandes exceptions sont noyées dans le détail** | Les contrôleurs parcourent des milliers de lignes et manquent des écarts de stock commercialement fatals. | Le tableau de bord direction met en évidence les taux d'erreur 3PL, le stock mort et les 10 premiers articles par valeur de perte. |
| **Les pertes 3PL sont difficiles à étayer** | Le stock manquant reste une réclamation informelle d'entrepôt sans documentation. | Génère un grand livre d'écarts factuel pour appuyer les réclamations SLA 3PL formelles et les remboursements. |

---

## À qui cela s'adresse : rôles et cas d'usage

Cet outil comble le fossé entre l'entreposage physique et le reporting financier. Il est délibérément conçu pour :

*   les **responsables des opérations e-commerce** ayant besoin d'un *modèle de rapprochement des stocks Shopify* pour synchroniser les vitrines numériques avec les centres d'exécution physiques.
*   les **directeurs de la chaîne d'approvisionnement** recherchant une *alternative au logiciel d'audit 3PL* pour tenir les partenaires externes responsables des taux de perte contractuels.
*   les **contrôleurs de stocks et gestionnaires d'entrepôt** effectuant des *rapprochements de comptage cyclique* mensuels sur plusieurs nœuds internes.
*   les **CFO fractionnels et directeurs financiers** ayant besoin d'une méthode précise pour calculer la *perte de stocks et l'impact COGS* pour les clôtures comptables de fin de mois.
*   les **fondateurs DTC** qui ont besoin d'une vue d'ensemble de la santé des stocks de niveau direction sans investir dans des intégrations ERP complexes à six chiffres.

*Remarque : cette boîte à outils n'est **pas** conçue pour remplacer les API temps réel, les systèmes ERP ou la numérisation de codes-barres WMS en direct. C'est un cadre d'aide à la décision périodique utilisé pour auditer ces systèmes.*

---

## À propos du créateur

Je conçois des outils de suivi opérationnel et d'aide à la décision légers pour les situations où il y a trop de pièces mobiles à garder en tête, mais pas assez de complexité pour justifier un autre système d'entreprise.

La question centrale est simple : **quelles informations doivent être réunies en un seul endroit centralisé avant que la prochaine décision stratégique de chaîne d'approvisionnement puisse être prise avec confiance ?**

Ce classeur de rapprochement des stocks multi-nœuds est un exemple de cette approche : transformer des comparaisons de stocks inter-systèmes récurrentes en un flux analytique standardisé qui relie les écarts opérationnels aux conséquences financières.


## Détails techniques

<details>
<summary>Pour les réviseurs techniques, les praticiens d'Excel et les collaborateurs</summary>

### Architecture du classeur

Le classeur est délibérément structuré comme un **moteur de nettoyage des données et de rapprochement + tableau de bord décisionnel de perte financière**, plutôt que comme une base de données de stocks permanente. Chaque cycle de rapprochement peut écraser le jeu d'imports précédent ou être enregistré comme un classeur séparé, gardant le fichier léger et évitant les dépendances inutiles en bases de données ou macros.

L'architecture suit un principe simple :

**Entrée → Normalisation → Rapprochement → Quantification → Signalement → Présentation**

```text
                    ┌──────────────────────┐
                    │    Config_Master      │
                    │ SKU / Cost / Rules    │
                    └──────────┬───────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
     Import_Shopify       Import_WMS       Import_3PL
     System snapshot      WMS snapshot     Physical stock
             │                 │                 │
             └─────────────────┼─────────────────┘
                               ▼
                    ┌──────────────────────┐
                    │     Calc_Engine      │
                    │ Normalize + Match    │
                    │ Variance Calculation  │
                    │ Loss Valuation        │
                    │ Exception Flagging    │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │      Dashboard       │
                    │ KPI + Loss Analysis  │
                    │ Risk Ranking         │
                    └──────────────────────┘
```

Le classeur est divisé en six feuilles fonctionnelles :

| Feuille            | Couche        | Responsabilité                                                            | Utilisateur principal   |
| ---------------- | ------------- | ------------------------------------------------------------------------- | ---------------------- |
| `Dashboard`      | Décision      | Résumé des KPI, exposition aux pertes, comparaison des nœuds, 10 premières exceptions            | Direction / Management       |
| `Config_Master`  | Configuration | Liste SKU standard, informations produit, coût unitaire, seuils d'écart | Opérations / Finance   |
| `Import_Shopify` | Entrée         | Export brut des stocks Shopify                                              | Opérations             |
| `Import_WMS`     | Entrée         | Export brut des stocks WMS internes                                         | Entrepôt / Opérations |
| `Import_3PL`     | Entrée         | Export brut des stocks physiques 3PL                                         | 3PL / Opérations       |
| `Calc_Engine`    | Calcul   | Normalisation des données, appariement des SKU, calculs d'écart, impact financier | Couche technique masquée |

Les trois feuilles d'import sont volontairement maintenues comme des **zones de collage**. La spécification source permet aux utilisateurs de coller directement les exports originaux, y compris la compatibilité avec les lignes vides de tête, au lieu de les forcer à remanier manuellement les fichiers avant le rapprochement.

### Flux de données et logique de rapprochement

La couche de calcul principale utilise `Config_Master` comme point de référence pour les SKU standardisés.

```text
Raw Export
   ↓
Trim / Normalize
   ↓
Standard SKU Key
   ↓
Cross-System Lookup
   ↓
Shopify Quantity
WMS Quantity
3PL Quantity
   ↓
Absolute Variance
   ↓
Relative Variance
   ↓
Unit Cost
   ↓
Estimated Financial Loss
   ↓
Warning / Exception Status
   ↓
Dashboard
```

La conception répond spécifiquement au problème des **données désordonnées**. L'architecture source prescrit `TRIM()` pour supprimer les espaces cachés ou accidentels et `UPPER()` pour normaliser la capitalisation, suivis de `XLOOKUP` ou `INDEX + MATCH` pour une récupération inter-tables non invasive.

Cela compte parce qu'un SKU tel que :

```text
ABC-001
```

ne devrait pas devenir une fausse exception simplement parce qu'un autre export contient :

```text
 abc-001
```

Le moteur de rapprochement traite donc la normalisation comme un préalable à la comparaison, plutôt que d'essayer de résoudre les problèmes de qualité des données après que le rapport d'écarts a déjà été généré.

### Principe de la date de coupure du rapprochement

Les instantanés des stocks doivent représenter le **même instant de coupure métier**.

Par exemple :

```text
Shopify Snapshot     → Sunday 23:59:59
WMS Snapshot         → Sunday 23:59:59
3PL Physical Count   → Sunday 23:59:59
```

Si les instantanés sont pris à des moments sensiblement différents, les mouvements de stock, les retours ou les commandes en transit peuvent créer des différences apparentes qui ne sont pas une perte réelle.

L'architecture source identifie explicitement la cohérence de l'instant de coupure comme une contrainte opérationnelle fondamentale et avertit que des instantanés décalés peuvent créer de « fausses différences ».

C'est donc une **exigence de contrôle métier**, et pas seulement une exigence de formule de tableur.

### Le SKU comme clé unique de rapprochement

Le SKU est traité comme l'identité standard reliant les trois systèmes sources.

La couche de configuration maintient :

* SKU standard
* Nom du produit
* Coût unitaire
* Seuil d'écart
* Seuil d'alerte

Le moteur de calcul utilise ensuite cette clé standard pour récupérer les quantités auprès de chaque source.

Cela évite que le rapprochement ne dépende de l'ordre des lignes des fichiers importés. Shopify peut lister les SKU dans une séquence, le WMS dans une autre et la 3PL dans une troisième ; le moteur de calcul compare toujours le même produit au même produit.

La spécification source souligne l'unicité et la cohérence des SKU comme une contrainte fondamentale : un produit physique ne devrait pas être représenté par plusieurs identifiants incohérents.

### Architecture du tableau de bord

Le Dashboard est délibérément conçu pour une **gestion par l'exception d'abord**, et non pour reproduire les tables sources brutes.

La couche KPI principale contient :

* Écart total de quantité
* Perte financière totale estimée
* Taux d'écart 3PL
* Taux d'écart de l'entrepôt interne

La couche visuelle fournit ensuite :

* Répartition de la valeur de perte entre la 3PL et l'entrepôt interne
* 10 premiers SKU classés par valeur de perte
* Identification des exceptions à haut risque

Ces sorties sont explicitement spécifiées dans l'architecture source.

La séquence de gestion envisagée est :

```text
How much is different?
        ↓
How much money is exposed?
        ↓
Where is the exposure concentrated?
        ↓
Which SKUs matter most?
        ↓
Which exceptions should be investigated?
        ↓
Is a process correction or 3PL claim required?
```

C'est pourquoi le classeur est mieux compris comme une **couche d'aide à la décision** que comme un simple tableur de comparaison des stocks.

### Trois pièges qui surprennent même les opérateurs de stocks expérimentés

#### Piège 1 — traiter chaque différence de quantité comme une perte

**Décision :**
Un opérateur voit que Shopify déclare 1 000 unités tandis que la 3PL en déclare 970 et enregistre immédiatement 30 unités comme perdues.

**Chiffre erroné :**
La comparaison utilise des instantanés pris à des moments différents.

**Pourquoi la recommandation change :**
L'écart de 30 unités peut représenter des expéditions, des retours, des ajustements ou d'autres mouvements survenus entre les deux instantanés.

**Approche correcte :**
Établir d'abord un instant de coupure commun et comparer des instantanés de stocks comparables.

| Approche                 | Résultat                                             |
| ------------------------ | -------------------------------------------------- |
| Instants d'instantané différents | Écart de 30 unités traité comme une perte                 |
| Coupure commune           | Seul l'écart résiduel inexpliqué fait l'objet d'une enquête |

La source identifie spécifiquement l'incohérence de la date de coupure comme une cause de faux écarts.

La décision corrigée est donc **« enquêter sur l'écart résiduel »**, et non **« réclamer la totalité de l'écart comme perte ».**

<details>
<summary>Logique de calcul</summary>

```text
Comparable Variance
= Quantity at Node A
- Quantity at Node B

Only when:
Snapshot_A_Time = Snapshot_B_Time
```

Un écart ne devrait pas être interprété comme une perte financière tant que la base de comparaison elle-même n'est pas valide.

</details>

#### Piège 2 — classer les problèmes par unités plutôt que par argent

**Décision :**
L'opérateur trie le rapport de rapprochement par le plus grand écart de quantité.

**Métrique erronée :**
Un écart de 50 unités est classé au-dessus d'un écart de 10 unités simplement parce que `50 > 10`.

**Pourquoi la recommandation est incomplète :**
La quantité ne représente pas la signification économique.

Supposons :

| SKU   | Écart | Coût unitaire | Exposition estimée |
| ----- | -------: | --------: | -----------------: |
| SKU-A |       50 |        $2 |               $100 |
| SKU-B |       10 |       $40 |               $400 |

Un classement fondé uniquement sur la quantité enquêterait d'abord sur SKU-A. Un classement fondé sur la perte financière enquêterait d'abord sur SKU-B.

L'architecture source prescrit explicitement l'introduction d'une matrice de coûts SKU afin que les différences de quantité puissent être traduites en perte financière.

**Décision correcte :** prioriser les exceptions en utilisant à la fois **l'écart de quantité et l'exposition financière**, plutôt que la quantité seule.

<details>
<summary>Logique de calcul</summary>

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

Pour l'exemple :

```text
SKU-A = 50 × $2  = $100
SKU-B = 10 × $40 = $400
```

La deuxième exception a la quantité la plus faible mais la conséquence financière la plus importante.

</details>

#### Piège 3 — supposer qu'un appariement SKU propre signifie des données propres

**Décision :**
L'opérateur utilise une recherche directe entre les trois exports et suppose que les enregistrements non appariés représentent du stock manquant.

**Hypothèse erronée :**
Les chaînes SKU sont présumées identiques entre les systèmes.

**Pourquoi la recommandation change :**
Les données exportées peuvent contenir des espaces de tête ou de fin, une capitalisation incohérente, des caractères spéciaux, des lignes vides ou des conventions historiques de nommage des SKU. La source identifie spécifiquement ces éléments comme des problèmes pratiques de qualité des données.

Par exemple :

```text
Shopify → "sku-001"
WMS     → "SKU-001"
3PL     → " SKU-001 "
```

Une correspondance exacte naïve peut interpréter ces éléments comme des produits différents.

**Approche correcte :** normaliser l'identifiant avant la recherche inter-systèmes.

<details>
<summary>Logique de normalisation</summary>

```excel
=UPPER(TRIM([@SKU]))
```

Utiliser ensuite la clé normalisée pour la récupération inter-tables.

Conceptuellement :

```text
Raw SKU
   ↓
TRIM()
   ↓
UPPER()
   ↓
Standardized SKU Key
   ↓
XLOOKUP / INDEX + MATCH
```

Cela réduit les fausses exceptions causées par la mise en forme plutôt que par un mouvement de stock.

</details>

### Scénario d'exemple

Supposons qu'un rapprochement hebdomadaire soit effectué pour un seul SKU après que les trois systèmes ont été capturés au même instant de coupure.

Les instantanés importés déclarent :

| Source  | Quantité |
| ------- | -------: |
| Shopify |    1 000 |
| WMS     |      992 |
| 3PL     |      970 |

Le coût unitaire configuré du SKU est de **18 $**.

La première étape analytique n'est pas de déclarer 30 unités perdues. Le système établit les différences entre chaque position de stock déclarée :

```text
Shopify vs. WMS
= 1,000 - 992
= 8 units

WMS vs. 3PL
= 992 - 970
= 22 units
```

Cela fournit immédiatement une question opérationnelle plus utile.

L'écart total n'est pas simplement « 30 unités manquantes ». Les données suggèrent que le plus grand écart inexpliqué est concentré entre les nœuds WMS et 3PL.

Si l'écart 3PL de 22 unités reste inexpliqué après vérification du calendrier d'expédition, des retours, des ajustements et d'autres mouvements légitimes, l'exposition financière estimée au coût configuré est :

```text
22 × $18 = $396
```

L'implication pour le management est donc différente d'une alerte de stock générique.

L'action suivante n'est pas d'inspecter chaque SKU de manière égale. L'opérateur devrait enquêter d'abord sur **l'exception côté 3PL**, vérifier si l'écart représente une perte physique, un dommage, un problème de calendrier ou un problème de reporting, puis déterminer si l'écart dépasse la tolérance contractuelle ou interne de l'entreprise.

Le tableau de bord est conçu pour rendre cette priorisation visible : le management peut voir l'exposition financière totale, la répartition des pertes entre les nœuds et les exceptions de SKU de plus forte valeur sans parcourir manuellement les exports bruts.

L'outil prend donc en charge une séquence de :

**rapprochement → isolement des exceptions → quantification financière → enquête opérationnelle → réclamation ou correction de processus potentielle.**

Il ne détermine pas lui-même si un écart est juridiquement recouvrable. Cela reste une décision de management et contractuelle.

### Référence des formules

Les formules ci-dessous décrivent les schémas de calcul principaux spécifiés pour l'architecture de rapprochement. Elles visent à rendre le raisonnement du classeur auditable plutôt qu'à transformer le README en un catalogue générique de formules Excel.

<details>
<summary>Normalisation des SKU</summary>

**Objectif :** standardiser les chaînes SKU importées avant comparaison.

```excel
=UPPER(TRIM([@SKU]))
```

**Logique :**

* `TRIM()` supprime les espaces de tête, de fin et redondants.
* `UPPER()` standardise la capitalisation des lettres.
* La clé normalisée qui en résulte devient adaptée à l'appariement inter-systèmes.

La source recommande spécifiquement `TRIM()` et `UPPER()` à cette fin.

</details>

<details>
<summary>Recherche inter-systèmes</summary>

**Objectif :** récupérer la quantité correspondante dans une table source après que le SKU a été standardisé.

```excel
=XLOOKUP(
    Normalized_SKU,
    Source_SKU_Column,
    Source_Quantity_Column,
    0
)
```

L'architecture autorise `XLOOKUP` ou `INDEX + MATCH` comme mécanisme de récupération inter-tables.

Le principe de conception important n'est pas la fonction de recherche spécifique. C'est que **l'identité SKU, plutôt que la position de ligne, contrôle le rapprochement**.

</details>

<details>
<summary>Calcul des écarts</summary>

**Objectif :** quantifier la différence entre des positions de stock comparables.

```text
Absolute Variance
= Source Quantity - Reference Quantity
```

L'implémentation devrait préserver le signe lorsque l'interprétation directionnelle est utile et utiliser des valeurs absolues lors du classement de l'ampleur de l'écart.

```text
Variance Magnitude
= ABS(Source Quantity - Reference Quantity)
```

Cela prend en charge à la fois :

* le rapprochement directionnel ;
* le classement des exceptions.

</details>

<details>
<summary>Conversion en perte financière</summary>

**Objectif :** convertir l'écart de stock en une exposition financière estimée.

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

Le coût unitaire est maintenu dans `Config_Master`, permettant de réutiliser le même moteur de rapprochement lorsque les coûts des produits changent.

La source définit explicitement la matrice de coûts comme le mécanisme de traduction des écarts de stock en perte financière.

</details>

<details>
<summary>Écart relatif et seuil de risque</summary>

**Objectif :** distinguer une petite différence numérique d'une exception opérationnelle significative.

Conceptuellement :

```text
Discrepancy Rate
= Absolute Variance ÷ Reference Inventory
```

Le taux résultant peut être comparé au seuil d'alerte ou de tolérance configuré.

La conception source prescrit que `Config_Master` maintienne les seuils d'écart et que la mise en forme conditionnelle signale les lignes dont la quantité ou le taux d'écart franchit la limite configurée.

</details>

### Règles de validation

Le moteur de rapprochement dépend d'un petit nombre de contrôles qui doivent être respectés avant que la sortie puisse être traitée comme de qualité décisionnelle.

| Champ / Contrôle                  | Règle                                                                                                           | Comportement en cas d'erreur                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **SKU**                          | Doit être standardisé et identifiable de manière cohérente entre les fichiers sources.                                        | Les enregistrements non appariés ou mal formés devraient être traités comme des exceptions de qualité des données plutôt que silencieusement classés comme perte. |
| **Unicité des SKU**               | Un produit physique devrait correspondre à une identité SKU standard.                                                  | Les identifiants en double ou en conflit nécessitent une correction des données de référence avant tout rapprochement fiable.                       |
| **Coût unitaire**                    | Doit exister dans `Config_Master` pour la valorisation financière.                                                         | L'écart de quantité peut rester visible, mais l'exposition financière ne peut pas être valorisée de manière fiable sans coût.                    |
| **Coupure des instantanés**             | Les données Shopify, WMS et 3PL devraient représenter le même instant.                                               | Des horodatages différents peuvent créer de faux écarts et nécessiter une ré-exportation ou un ajustement.                                       |
| **Données sources importées**         | Les exports bruts devraient être collés de manière cohérente dans leurs zones d'import désignées.                                  | Les anomalies structurelles ou de format source devraient être corrigées avant d'interpréter les exceptions résultantes.                   |
| **Seuil d'écart**        | Les seuils de quantité/taux devraient être maintenus dans la configuration plutôt que codés en dur dans les sorties individuelles. | Les exceptions franchissant le seuil sont mises en évidence pour enquête.                                                      |
| **Tolérance 3PL / SLA**          | La tolérance de perte contractuelle doit être prise en compte pour décider si une exception mérite une réclamation.              | Le classeur fournit des preuves ; le management détermine si une réclamation contractuelle devrait être engagée.                    |
| **Calendrier des retours**               | Les retours enregistrés par une 3PL et les remboursements enregistrés dans Shopify peuvent survenir à des moments différents.                        | Les décalages à court terme ne devraient pas être automatiquement interprétés comme une perte permanente.                                     |
| **Nommage historique des SKU**        | Les incohérences de nommage historiques doivent être normalisées ou mappées.                                                    | Les SKU historiques non mappés devraient rester visibles comme des exceptions de qualité des données.                                                |
| **Délai de synchronisation des systèmes** | Les problèmes temporaires de synchronisation Shopify/3PL échappent à la logique de rapprochement du tableur.               | À traiter comme un problème d'intégration système plutôt qu'en forçant une solution de contournement de tableur basée sur VBA.                               |

La source distingue explicitement les problèmes qu'Excel peut résoudre des problèmes nécessitant une intervention opérationnelle ou au niveau du système. Le rapprochement standardisé, la valorisation des pertes et les tableaux de bord d'exceptions relèvent du classeur ; la discipline de comptage cyclique, la gestion des réclamations 3PL, la synchronisation des API et le suivi GPS n'en relèvent pas.



### Ce que ce classeur ne tente pas de résoudre

L'architecture maintient délibérément une frontière claire autour de la couche Excel.

**Problèmes de gestion opérationnelle :**

* procédures de comptage cyclique 3PL incohérentes ;
* fréquence insuffisante des comptages physiques des stocks ;
* absence d'engagement de réclamations lorsque les limites de perte contractuelles sont dépassées.

Ceux-ci nécessitent une action du management plutôt qu'une autre formule.

**Problèmes d'intégration système :**

* délais de synchronisation en temps réel Shopify ↔ 3PL ;
* communication API ;
* intégration ERP automatisée.

La source recommande spécifiquement de ne pas forcer ces problèmes dans un classeur Excel léger via VBA.

**Problèmes de visibilité du transport :**

* suivi GPS en temps réel des stocks en transit ;
* flux de travail de gestion du transport.

Ceux-ci nécessitent un TMS dédié plutôt qu'un tableur de rapprochement des stocks.

Cette frontière est intentionnelle. L'objectif du classeur est de fournir une **couche d'analyse répétable du rapprochement et des pertes financières**, et non de faire semblant que tout problème de contrôle des stocks est un problème Excel.

### Obtenir le classeur

L'outil est conçu pour un rapprochement récurrent plutôt que pour une analyse de tableur ponctuelle.

Le cycle opérationnel envisagé est :

```text
Export Shopify inventory
        ↓
Export WMS inventory
        ↓
Export 3PL physical inventory
        ↓
Paste the three snapshots
        ↓
Refresh the reconciliation
        ↓
Review financial loss + exception ranking
        ↓
Investigate / correct / claim
```

Le plan source spécifie une cadence hebdomadaire ou mensuelle, les utilisateurs collant les trois exports sources dans leurs feuilles d'entrée respectives et maintenant à jour les coûts SKU et les seuils d'alerte dans `Config_Master`.

**Version navigateur :** utilisez la version HTML pour un examen opérationnel rapide.

**Version Excel :** utilisez le classeur lorsque le rapprochement doit être rafraîchi avec les exports Shopify, WMS et 3PL réels.

L'outil est délibérément conçu pour qu'un utilisateur opérationnel ou financier non technique puisse effectuer le rapprochement récurrent sans reconstruire le modèle analytique à chaque fois. L'objectif source est d'environ **10 minutes** pour le nettoyage, le rapprochement et l'examen des exceptions.

### Limites

Ce classeur est une **couche de rapprochement et d'analyse des pertes**, et non une plateforme de contrôle des stocks.

Il ne peut pas :

* garantir la synchronisation en temps réel Shopify ↔ WMS ↔ 3PL ;
* empêcher un opérateur d'entrepôt d'expédier physiquement un article lorsque le stock est insuffisant ;
* remplacer un WMS, un ERP ou un système de gestion des stocks ;
* imposer les procédures de comptage cyclique 3PL ;
* déterminer automatiquement si un écart est contractuellement recouvrable ;
* fournir un suivi GPS en temps réel des stocks en transit ;
* résoudre les problèmes de données de référence historiques des SKU sans une décision de mappage appropriée.

Ces frontières sont explicites dans la conception source. Le rapprochement standardisé, la valorisation des écarts, le classement des exceptions et les rapports de tableau de bord sont considérés comme des problèmes Excel appropriés. La discipline de comptage cyclique et la gestion des réclamations 3PL nécessitent des contrôles de management ; la synchronisation API en temps réel relève de l'intégration système ; le suivi physique des expéditions relève d'un TMS.

Il existe également d'importantes contraintes d'interprétation.

**Une différence de quantité n'est pas automatiquement une perte.** Les retours peuvent être enregistrés par une 3PL à un moment différent du remboursement Shopify correspondant, et un calendrier d'instantanés incohérent peut créer des différences temporaires. L'opérateur doit valider le contexte métier avant de classer un écart comme une perte permanente.

**Le chiffre de perte financière est une estimation, et non une écriture comptable.** Il dépend du coût unitaire SKU configuré et de l'interprétation de la différence de quantité sous-jacente.

**Un résultat de tableur propre ne garantit pas des données sources propres.** Les incohérences historiques de nommage des SKU, les exports incomplets, les enregistrements en double ou les comptages physiques incorrects peuvent encore produire des conclusions trompeuses.

Le classeur devrait donc être utilisé comme un **mécanisme de constatation et de priorisation**, et non comme un moteur de jugement automatique.

</details>


## Autres outils de cette série

Une collection d'outils Excel légers d'aide à la décision couvrant le contrôle opérationnel, le rapprochement, la rentabilité, les stocks et l'analyse financière.

* **Contrôle des stocks et réapprovisionnement** — demande, réapprovisionnement, exposition des stocks et décisions d'achat.
* **Moteur de rentabilité au niveau de la commande** — revenus, coûts variables, répartition des frais d'expédition et rentabilité au niveau de la commande.
* **Contrôle de construction par projet** — budget du projet, engagements, coûts de chantier et rentabilité du projet.
* **Système de gestion des opérations et de la rentabilité pour entrepreneurs** — flux de travail Lead → Estimate → Job → Labor & Materials → Job Cost → Profit → Customer History.

## Licence

Ce projet est publié sous la **licence Apache 2.0**.

Vous pouvez utiliser, modifier, distribuer et adapter le projet sous réserve des termes et conditions de la licence Apache 2.0.

Consultez le fichier de licence du dépôt pour le texte complet de la licence.


