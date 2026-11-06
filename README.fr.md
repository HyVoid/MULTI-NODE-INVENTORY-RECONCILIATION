[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Modèle Excel de réconciliation des stocks Shopify & 3PL : écarts de stock d'entrepôt, variance de comptage cyclique & calculateur de coût de dépréciation
<img width="1102" height="790" alt="image" src="https://github.com/user-attachments/assets/3a637973-b460-4160-a098-eed931e2dc18" />



[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Web Browser + Microsoft Excel (.xlsx)](https://img.shields.io/badge/Platform-Web%20Browser%20%2B%20Microsoft%20Excel%20(.xlsx)-217346.svg)](#quick-start-tutorial-how-to-reconcile-shopify-wms--3pl-inventory-in-4-steps)
[![Tool Type: Plug-and-Play Ecommerce Inventory Spreadsheet](https://img.shields.io/badge/Tool%20Type-Plug--and--Play%20Inventory%20Spreadsheet-2251FF.svg)](#what-it-helps-you-track-ecommerce-inventory-pain-points-vs-solutions)

**Un modèle Excel (`.xlsx`) de réconciliation des stocks Shopify & 3PL prêt à l'emploi et un calculateur en ligne gratuit d'écarts de stock, conçus pour les marques e-commerce, les opérateurs DTC et les gestionnaires d'entrepôt qui doivent auditer leurs quantités en stock sans écrire la moindre formule.** Comparez **les quantités de la vitrine Shopify**, les **enregistrements internes du système de gestion d'entrepôt (WMS)** et **les comptages physiques de la logistique tierce (3PL)** côte à côte, calculez la **dépréciation des stocks pondérée par le COGS ($)**, stoppez la **survente due au stock fantôme** et générez des **réclamations de remboursement 3PL documentées** dans un seul tableur préconfiguré.

**Testez vos données SKU gratuitement dans votre navigateur dès maintenant, ou téléchargez le fichier Excel débloqué pour vos audits mensuels.**

Chaque règle d'appariement SKU, formule de nettoyage de texte et calcul d'écart en dollars est déjà intégré. Copiez-collez vos exports CSV bruts provenant de Shopify, de votre WMS et de votre 3PL pour visualiser vos écarts de stock exacts et votre exposition aux pertes financières en quelques secondes — avec une garantie de remboursement de 30 jours sans conditions.

> 🌐 **Essayez d'abord le calculateur de réconciliation en ligne**  
> [Lancez le calculateur web interactif gratuit de réconciliation des stocks Shopify & 3PL (démo navigateur, aucune configuration requise)](https://hyvoid.github.io/multi-node-inventory-reconciliation/)
> 
> 📥 **Téléchargez le modèle Excel prêt à l'emploi**  
> [Obtenez le modèle Excel débloqué de réconciliation multi-nœuds des stocks et d'audit des pertes (.xlsx avec formules à mise à jour automatique)](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)
>
> *Le calculateur navigateur gratuit et le classeur Microsoft Excel téléchargeable reposent sur exactement les mêmes tables préconfigurées d'appariement SKU à 3 voies et d'écarts de COGS.*

---

## Ce que cet outil vous permet de suivre : points de douleur des stocks e-commerce vs. solutions

Découvrir que vos chiffres de stock ne correspondent pas n'est que la moitié du problème — vous devez aussi savoir où sont passées les unités et quel montant est en jeu. Ce **tableur d'audit des stocks plug-and-play** résout les cinq angles morts les plus fréquents du contrôle des stocks pour les marques e-commerce multicanal :

| Sujet de recherche fréquent & objectif de suivi | Point de douleur quotidien des stocks e-commerce (là où l'argent fuit) | Comment ce modèle Excel préconfiguré le corrige et le suit |
| :--- | :--- | :--- |
| **Écarts de stock Shopify vs. 3PL vs. WMS (`Appariement des stocks à 3 voies`)** | Shopify affiche 120 unités, votre WMS en indique 100 et votre 3PL 85 — et vous ne savez pas quel système détient le vrai comptage de stock. | Aligne **les quantités Shopify, WMS et 3PL côte à côte** par SKU afin de séparer les retards de synchronisation IT des pertes physiques réelles en entrepôt. |
| **Coût de dépréciation des stocks & radiation COGS (`Impact en $` vs. nombre d'unités)** | Traiter un écart de 20 unités sur un insert d'emballage à 2 $ avec la même urgence qu'une perte de 20 unités sur un produit phare à 75 $. | Multiplie chaque écart d'unités par le **coût unitaire (COGS)** de chaque SKU pour calculer l'**exposition exacte aux pertes en dollars ($)** destinée aux radiations comptables. |
| **Stock perdu 3PL & réclamations de remboursement SLA (`Audit de l'allocation de perte`)** | Vous savez que votre centre de fulfillment perd de la marchandise, mais il vous manque la preuve des écarts au niveau SKU nécessaire pour déposer une réclamation contractuelle. | Suit les **taux d'écart (%) entre 3PL et entrepôt interne** par rapport à votre plafond contractuel de perte afin de construire un registre de remboursement factuel. |
| **Stock fantôme & survente en haute saison (`Prévention des ruptures de stock`)** | Shopify affiche plus d'unités disponibles qu'il n'y en a réellement sur les étagères du 3PL, ce qui pousse les publicités payantes à générer des commandes que vous devez annuler et rembourser. | Signale chaque SKU pour lequel **le stock numérique de la vitrine dépasse le stock physique 3PL** afin de corriger les niveaux d'inventaire avant la survente. |
| **Paralysie d'analyse du comptage cyclique (`Top 10 des SKU à valeur de perte`)** | Faire défiler des milliers de lignes après un comptage cyclique d'entrepôt en passant à côté des 5 SKU qui génèrent 80 % de votre perte financière. | Filtre automatiquement les lignes concordantes et classe les **10 SKU aux pertes en dollars les plus élevées** sur un tableau de bord récapitulatif pour une action immédiate. |

---

## Tutoriel de démarrage rapide : comment réconcilier les stocks Shopify, WMS & 3PL en 4 étapes

Vous n'avez pas besoin de compétences Excel avancées ni de formules `VLOOKUP` manuelles pour réaliser un audit d'entrepôt. Suivez ces quatre étapes pour transformer des exports CSV bruts en un **rapport d'écarts et de dépréciation des stocks** clair :

### Étape 1 : saisissez votre liste maîtresse de SKU, vos COGS unitaires & vos seuils d'alerte (`Config_Master`)
Ouvrez l'onglet `Config_Master` pour définir vos règles d'inventaire de référence :
- Collez votre **liste maîtresse de SKU** et votre **coût de revient unitaire (COGS)**.
- Définissez vos **seuils d'alerte d'écart personnalisés** (par exemple, signaler tout SKU présentant un écart supérieur à `5 unités` ou une valeur de stock manquant supérieure à `100 $`).

*Aperçu en direct :* découvrez dès maintenant le fonctionnement de la table de configuration maîtresse dans le [calculateur navigateur gratuit de réconciliation des stocks 3PL](https://hyvoid.github.io/multi-node-inventory-reconciliation/).

---

### Étape 2 : copiez-collez vos exports CSV bruts Shopify, WMS & 3PL
Épargnez-vous la mise en forme manuelle des colonnes et le nettoyage du texte. Collez vos exports d'inventaire bruts directement dans les trois onglets d'entrée :
- `Import_Shopify` : votre export CSV d'inventaire produits Shopify (niveaux de stock de la vitrine).
- `Import_WMS` : votre rapport de stock interne du système de gestion d'entrepôt ou de l'ERP.
- `Import_3PL` : le comptage cyclique physique ou le rapport d'inventaire final de votre partenaire de fulfillment (compatible avec les exports de ShipBob, ShipMonk, Flexport, Amazon MCF et des portails 3PL personnalisés).
- **Zéro glissement de formule manuel :** les tables préconfigurées nettoient les espaces superflus, alignent les codes SKU et s'étendent automatiquement lorsque vous collez de nouvelles lignes.

---

### Étape 3 : consultez votre tableau de bord de dépréciation & le Top 10 des SKU à valeur de perte (`Dashboard`)
Basculez sur l'onglet `Dashboard` pour afficher les résultats complets de votre audit :
- Consultez la **valeur totale de dépréciation des stocks ($)**, l'**écart net d'unités** et les **taux de précision inter-systèmes (%)** calculés automatiquement.
- Examinez la liste des **10 SKU à valeur de perte la plus élevée** pour identifier quels produits exacts nécessitent un recomptage physique en entrepôt ou un ajustement urgent du stock sur Shopify.

---

### Étape 4 : téléchargez le modèle Excel débloqué pour des audits mensuels en un clic
Utilisez dès aujourd'hui l'outil navigateur gratuit pour tester votre flux de travail et repérer immédiatement les écarts de stock. Pour enregistrer vos coûts SKU de référence en local, exécuter des clôtures comptables mensuelles récurrentes et constituer un historique de réclamations 3PL, téléchargez le tableur `.xlsx` débloqué.

> 💡 **Pourquoi les marques e-commerce en croissance utilisent ce modèle Excel plutôt que de tout construire de zéro :**  
> Nettoyer des chaînes SKU désordonnées issues de trois exports différents, aligner des lignes discordantes et pondérer les écarts de stock par le COGS unitaire relève d'une ingénierie de tableur fastidieuse. **Dans ce modèle Excel, chaque règle d'appariement à 3 voies, normalisateur de texte et formule à mise à jour automatique est déjà intégré pour vous.**  
> 
> Vous n'avez même pas besoin de double-cliquer sur les coins de cellules ni de faire glisser des formules vers le bas. Téléchargez le classeur sur votre ordinateur, collez vos exports Shopify et 3PL du mois par-dessus les données du mois précédent, et obtenez un audit financier actualisé des pertes en un clic. Même sans aucune expérience technique des tableurs, vous obtenez une visibilité instantanée sur la santé de vos stocks — vous libérant pour vous concentrer sur le marketing, le réapprovisionnement des best-sellers et la clôture des ventes pendant les pics du T4 et du Black Friday, pendant qu'un simple modèle de copier-coller gère la réconciliation des données.  
> 
> 👉 **[Téléchargez dès aujourd'hui le modèle Excel débloqué de réconciliation des stocks Shopify & 3PL (.xlsx) et automatisez vos audits de stock](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**

---

## La logique métier & la méthodologie : 4 angles morts des stocks que ce modèle Excel résout pour vous

La plupart des marques e-commerce perdent des milliers de dollars à cause de la dépréciation des stocks et de la survente, non pas parce qu'elles oublient de compter leur stock, mais parce que les vérifications standard à 2 voies et les tableurs d'unités basiques masquent l'endroit où surviennent les véritables dommages financiers. Voici, en termes simples, comment ce modèle protège vos stocks et votre trésorerie :

### 1. Comparer seulement deux systèmes masque l'existence d'un bug IT ou d'un vol en entrepôt (triangulation des stocks à 3 voies)
**Le fait objectif :** si vous comparez uniquement Shopify (100 unités) à votre 3PL (80 unités), vous savez que 20 unités manquent, mais vous ignorez *pourquoi*. Ces 20 unités peuvent se trouver dans des commandes non expédiées à cause d'un webhook API défaillant, ou 20 cartons physiques peuvent avoir quitté l'entrepôt par la porte arrière.  
**Votre bénéfice direct :** en alignant **Shopify (vitrine numérique) + WMS (registre interne) + 3PL (comptage physique des étagères)** côte à côte sur une même ligne, le modèle isole le point de rupture exact :
- Si `Shopify ≠ WMS`, mais `WMS = 3PL` : vous avez un retard de synchronisation de la vitrine ou des commandes non expédiées. Corrigez vos paramètres d'intégration.
- Si `Shopify = WMS`, mais `3PL < WMS` : le stock physique a été perdu, endommagé ou mal compté au centre de fulfillment. Déposez une réclamation 3PL.

### 2. Compter des unités manquantes au lieu de dollars manquants gaspille la main-d'œuvre d'entrepôt (classement des écarts pondéré par le COGS)
**Le fait objectif :** une feuille de comptage cyclique standard traite chaque unité de la même manière. Si votre équipe trie les écarts uniquement par nombre d'unités, elle passera des heures à recompter des fournitures d'emballage bon marché tout en ignorant les produits à coût élevé qui drainent silencieusement votre marge. Regardez comment les comptages bruts d'unités induisent les équipes d'entrepôt en erreur par rapport à la dépréciation pondérée par le COGS :

```text
SKU-A (Branded Poly-Mailer):   -50 Units Missing  ×  $0.20 Unit COGS  =   -$10.00 Financial Loss
SKU-B (Wireless Headphones):    -4 Units Missing  × $115.00 Unit COGS =  -$460.00 Financial Loss

```

Dans un tableur basique par nombre d'unités, `SKU-A` (-50 unités) semble être une urgence tandis que `SKU-B` (-4 unités) paraît être une simple erreur d'arrondi — alors que `SKU-B` coûte **46 fois plus d'argent** à votre entreprise.

**Votre bénéfice direct :** le modèle multiplie automatiquement chaque écart d'unités par son COGS unitaire et classe vos **10 SKU à valeur de perte la plus élevée par impact en dollars**. Votre équipe enquête d'abord sur la perte de 460 $ au lieu de courir après 10 $ de pochettes d'expédition.

### 3. Les contrats de fulfillment 3PL imposent des délais de réclamation stricts et des plafonds de perte (preuve de réclamation SLA documentée)

**Le fait objectif :** presque tous les contrats de logistique tierce (3PL) incluent une « allocation de perte » intégrée (généralement 0,5 % à 2,0 % du total des unités traitées) et exigent des commerçants qu'ils soumettent une preuve d'écart SKU par SKU dans les 15 à 30 jours suivant un comptage cyclique pour prétendre à un remboursement. Les plaintes envoyées par e-mail sans registre d'écarts structuré sont systématiquement rejetées par les responsables de comptes 3PL.

**Votre bénéfice direct :** le modèle calcule les **pourcentages d'écart exacts entre nœuds** et génère une table d'écarts propre au niveau SKU montrant le stock attendu, le comptage physique, le déficit d'unités et la valeur en COGS — vous donnant une documentation prête à envoyer pour récupérer de l'argent auprès de votre 3PL.

### 4. Le « stock fantôme » sur Shopify brûle le budget publicitaire payant et déclenche des rétrofacturations (détection de stock fantôme)

**Le fait objectif :** lorsque votre boutique Shopify croit que vous avez 50 unités en stock, vos publicités shopping Meta et Google continuent de dépenser de l'argent pour attirer du trafic sur cette page produit. Si votre 3PL n'a en réalité 0 unité sur l'étagère (« stock fantôme »), chaque nouvelle commande client entraîne un retard de fulfillment, une annulation manuelle, des frais de traitement de paiement perdus et des tickets de support clients furieux.

**Votre bénéfice direct :** le modèle met en évidence chaque SKU pour lequel la disponibilité en vitrine dépasse le stock physique en entrepôt, afin que vous puissiez ajuster les quantités d'inventaire Shopify avant la survente lors des événements de vente à fort trafic.

---

## Tableurs de stocks manuels (`VLOOKUP`) vs. ce modèle automatisé de réconciliation Shopify & 3PL

| Facteur de comparaison entrepôt & comptabilité | Feuilles Excel manuelles (`VLOOKUP` / `INDEX-MATCH` de zéro) | Modèle standardisé de réconciliation des stocks multi-nœuds (cet outil) |
| --- | --- | --- |
| **Alignement des stocks entre 3 systèmes (`Shopify` + `WMS` + `3PL`)** | Le personnel recolle manuellement trois fichiers CSV distincts chaque mois, avec le risque de références de cellules cassées et de SKU oubliés. | Le **moteur d'appariement à 3 voies** préconfiguré aligne automatiquement les quantités Shopify, WMS et 3PL dès que vous collez vos exports. |
| **Mise en forme CSV désordonnée & SKU non appariés** | Les espaces de fin, les zéros initiaux et les codes SKU en majuscules/minuscules déclenchent de fausses erreurs `#N/A` sur des milliers de lignes. | Une **couche de normalisation de texte** intégrée nettoie les espaces et standardise les chaînes SKU avant le calcul des différences de stock. |
| **Valorisation financière de la dépréciation (`radiation COGS`)** | Les rapports n'affichent que des quantités d'unités manquantes, obligeant les comptables à rechercher manuellement les coûts produits à la clôture mensuelle. | Une **matrice de coûts SKU** intégrée convertit chaque pénurie d'unités en **exposition exacte aux pertes en dollars ($)** pour les écritures comptables. |
| **Filtrage des exceptions (`SKU à pertes principales`)** | Les managers font défiler plus de 5 000 lignes concordantes pour repérer quels produits présentent des écarts de stock dangereux. | Le **tableau de bord d'exceptions automatisé** filtre les lignes normales et classe automatiquement les **10 SKU aux pertes en dollars les plus élevées**. |
| **Documentation des remboursements SLA 3PL** | Les unités manquantes en entrepôt se discutent informellement par e-mail, sans pourcentages de précision historiques ni totaux en dollars. | Produit un **registre des écarts et des taux d'écart 3PL** prêt pour l'audit afin d'étayer les demandes formelles de crédit et de remboursement SLA. |

---

## Pour qui c'est fait : rôles e-commerce, cas d'usage des stocks & flux de travail tableur

Cette boîte à outils comble le fossé entre les étagères physiques de l'entrepôt et les états financiers e-commerce. Elle est conçue pour **les marques DTC en croissance, les vendeurs Shopify multicanal, les utilisateurs de 3PL et les équipes financières e-commerce** qui veulent un contrôle fiable des stocks sans payer plus de 30 000 $ par an pour un ERP d'entreprise :

* **Propriétaires de boutiques Shopify & fondateurs de marques DTC (`Modèle Excel de réconciliation des stocks Shopify`) :** repérez le stock fantôme et l'inventaire d'entrepôt manquant en quelques minutes, sans embaucher un analyste de données ni apprendre des formules de tableur complexes.
* **Responsables des opérations & du fulfillment e-commerce (`Tableur d'audit des écarts de stock & SLA 3PL`) :** tenez les centres de fulfillment externes (tels que ShipBob, ShipMonk ou des 3PL régionaux) responsables en suivant les taux de dépréciation mensuels par rapport aux plafonds SLA contractuels.
* **Gestionnaires d'entrepôt & contrôleurs de stocks (`Calculateur plug-and-play de variance de comptage cyclique`) :** réconciliez les comptages physiques des emplacements avec les registres WMS après les comptages cycliques hebdomadaires ou mensuels, en priorisant les recomptages selon la valeur en dollars la plus élevée à risque.
* **Comptables e-commerce & CFO fractionnaires (`Modèle comptable de dépréciation des stocks & radiation COGS`) :** calculez les ajustements exacts de valorisation de l'inventaire final et les radiations de dépréciation COGS de fin de mois pour QuickBooks Online, Xero ou NetSuite.
* **Vendeurs multicanal Amazon, Walmart & Shopify (`Feuille de comparaison des stocks multi-entrepôts`) :** auditez la distribution du stock et les quantités SKU non liées entre entrepôts internes, nœuds 3PL et canaux de vente en ligne depuis un seul fichier.

*Remarque : ce classeur Excel ne remplace pas les scanners de codes-barres en temps réel, les applications de synchronisation d'inventaire par API en direct ni votre WMS. Il sert de **couche d'audit et de réconciliation indépendante** pour détecter les échecs de synchronisation et la dépréciation physique que les logiciels automatisés ne voient pas.*

---

## Scénarios concrets : comment résoudre les problèmes courants de stocks Shopify & 3PL

Si votre équipe opérationnelle ou financière rencontre l'un de ces maux de tête récurrents de gestion des stocks, ce tableur est structuré pour les résoudre dès la sortie de la boîte :

* **Comment prévenir la survente pendant le Black Friday / Cyber Monday (haute saison du T4) :** Shopify affiche 100 unités disponibles, mais votre 3PL n'en a que 20 sur l'étagère. Exécutez cette réconciliation chaque semaine pendant le T4 pour détecter le « stock fantôme » et synchroniser les comptages de votre vitrine avant que les clients n'achètent des articles en rupture de stock.
* **Comment prouver le stock perdu par le 3PL et réclamer des remboursements SLA :** votre partenaire de fulfillment perd des SKU à ticket élevé au-delà de son allocation contractuelle de perte de 1,5 %. Collez vos journaux d'expédition WMS et le comptage physique du 3PL dans le modèle pour générer un rapport de pertes en dollars détaillé à l'appui de votre réclamation.
* **Comment calculer la dépréciation des stocks de fin de mois pour la comptabilité e-commerce :** votre comptable a besoin d'un chiffre en dollars exact du stock perdu ou endommagé pour clôturer le compte de résultat mensuel. Utilisez le total pondéré par le COGS du tableau de bord pour enregistrer des écritures de radiation d'inventaire précises en quelques minutes.
* **Comment réconcilier des exports CSV d'entrepôt désordonnés sans formules `VLOOKUP` cassées :** différents systèmes exportent des codes SKU avec des espaces superflus ou un formatage incohérent. Déposez les exports bruts dans les onglets d'import et laissez le modèle aligner et comparer chaque SKU automatiquement.

---

## À propos de Theseus Workshop

**Theseus Workshop** conçoit des modèles Microsoft Excel plug-and-play et des outils de décision basés sur le navigateur pour les opérateurs qui ont besoin de chiffres clairs et fiables dès aujourd'hui — sans logiciels d'entreprise encombrants ni programmation complexe de tableurs.

Chaque outil est conçu autour d'une question pratique unique :

> **« Quels chiffres opérationnels et financiers exacts doivent figurer dans une table préconfigurée pour que votre prochaine décision métier prenne des secondes au lieu de plusieurs heures ? »**

Si vous voulez arrêter de vous battre avec des feuilles `VLOOKUP` cassées, des ruptures de stock surprises et des pertes d'inventaire 3PL non compensées, téléchargez le modèle Excel complet ci-dessous ou explorez notre bibliothèque complète de tableurs opérationnels :

* 📥 **Obtenez ce modèle de réconciliation des stocks :** [Téléchargez le modèle Excel débloqué de réconciliation des stocks Shopify & 3PL (.xlsx)](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)
* 🌐 **Testez le calculateur web gratuit :** [Ouvrez le simulateur navigateur interactif de réconciliation des stocks 3PL](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
* 🧰 **Explorez tous les modèles Excel prêts à l'emploi & les boîtes à outils métier :** [Visitez la boutique officielle Theseus Workshop sur TheseusWorkshop.com](https://www.google.com/search?q=https://www.theseusworkshop.com%3Futm_source%3Dgithub%26utm_medium%3DGitHub%2520README%26utm_campaign%3Dreadme%2520new%2520launch%26utm_content%3Dinventory-readme-store-link)

---


## Détails techniques

<details>
<summary>Pour les réviseurs techniques, les praticiens d'Excel et les collaborateurs</summary>

### Architecture du classeur

Le classeur est délibérément structuré comme un **moteur de nettoyage et de réconciliation des données + tableau de bord décisionnel des pertes financières**, et non comme une base de données d'inventaire permanente. Chaque cycle de réconciliation peut écraser le jeu d'imports précédent ou être enregistré comme un classeur séparé, gardant le fichier léger et évitant les dépendances inutiles aux bases de données ou aux macros.

L'architecture suit un schéma simple :

**Entrée → Normalisation → Réconciliation → Quantification → Signalement → Présentation**

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

| Feuille          | Couche        | Responsabilité                                                            | Utilisateur principal  |
| ---------------- | ------------- | ------------------------------------------------------------------------- | ---------------------- |
| `Dashboard`      | Décision      | Résumé des KPI, exposition aux pertes, comparaison des nœuds, Top 10 des exceptions            | Direction / Management       |
| `Config_Master`  | Configuration | Liste SKU standard, informations produit, coût unitaire, seuils d'écart | Opérations / Finance   |
| `Import_Shopify` | Entrée        | Export brut d'inventaire Shopify                                              | Opérations             |
| `Import_WMS`     | Entrée        | Export brut d'inventaire WMS interne                                         | Entrepôt / Opérations |
| `Import_3PL`     | Entrée        | Export brut d'inventaire physique 3PL                                         | 3PL / Opérations       |
| `Calc_Engine`    | Calcul        | Normalisation des données, appariement des SKU, calculs d'écarts, impact financier | Couche technique masquée |

Les trois feuilles d'import sont volontairement maintenues comme des **zones de collage**. La spécification source permet aux utilisateurs de coller directement les exports originaux, y compris la compatibilité avec les lignes vides initiales, au lieu de les forcer à remanier manuellement les fichiers avant la réconciliation.

### Flux de données et logique de réconciliation

La couche de calcul centrale utilise `Config_Master` comme point de référence pour les SKU standardisés.

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

La conception répond spécifiquement au problème des **données désordonnées**. L'architecture source prévoit `TRIM()` pour supprimer les espaces cachés ou accidentels et `UPPER()` pour normaliser la casse, suivis de `XLOOKUP` ou `INDEX + MATCH` pour une récupération croisée non invasive entre tables.

Cela compte parce qu'un SKU tel que :

```text
ABC-001
```

ne devrait pas devenir une fausse exception simplement parce qu'un autre export contient :

```text
 abc-001
```

Le moteur de réconciliation traite donc la normalisation comme un préalable à la comparaison, plutôt que d'essayer de résoudre les problèmes de qualité des données après que le rapport d'écarts a déjà été généré.

### Principe du point de coupure de la réconciliation

Les instantanés d'inventaire doivent représenter le **même instant de coupure métier**.

Par exemple :

```text
Shopify Snapshot     → Sunday 23:59:59
WMS Snapshot         → Sunday 23:59:59
3PL Physical Count   → Sunday 23:59:59
```

Si les instantanés sont pris à des moments sensiblement différents, les mouvements de stock, les retours ou les commandes en transit peuvent créer des différences apparentes qui ne constituent pas une réelle dépréciation.

L'architecture source identifie explicitement la cohérence de l'instant de coupure comme une contrainte opérationnelle centrale et avertit que des instantanés désalignés peuvent créer de « fausses différences ».

C'est donc une **exigence de contrôle métier**, et pas seulement une exigence de formule de tableur.

### Le SKU comme clé unique de réconciliation

Le SKU est traité comme l'identité standard reliant les trois systèmes sources.

La couche de configuration maintient :

* SKU standard
* Nom du produit
* Coût unitaire
* Seuil d'écart
* Seuil d'alerte

Le moteur de calcul utilise ensuite cette clé standard pour récupérer les quantités auprès de chaque source.

Cela évite que la réconciliation ne dépende de l'ordre des lignes des fichiers importés. Shopify peut lister les SKU dans une séquence, le WMS dans une autre et le 3PL dans une troisième ; le moteur de calcul compare toujours le même produit au même produit.

La spécification source souligne l'unicité et la cohérence des SKU comme une contrainte fondamentale : un produit physique ne devrait pas être représenté par plusieurs identifiants incohérents.

### Architecture du tableau de bord

Le Dashboard est délibérément conçu pour une **gestion par exception d'abord**, et non pour reproduire les tables sources brutes.

La couche KPI principale contient :

* Écart total de quantités
* Perte financière totale estimée
* Taux d'écart 3PL
* Taux d'écart de l'entrepôt interne

La couche visuelle fournit ensuite :

* Répartition de la valeur des pertes entre 3PL et entrepôt interne
* Top 10 des SKU classés par valeur de perte
* Identification des exceptions à haut risque

Ces sorties sont directement spécifiées dans l'architecture source.

La séquence de gestion prévue est :

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

C'est pourquoi ce classeur s'entend mieux comme une **couche d'aide à la décision** que comme un simple tableur de comparaison de stocks.

### Trois pièges qui surprennent même les opérateurs de stocks expérimentés

#### Piège 1 — Traiter chaque différence de quantité comme une dépréciation

**Décision :**
Un opérateur voit que Shopify déclare 1 000 unités tandis que le 3PL en déclare 970 et enregistre immédiatement 30 unités comme perdues.

**Chiffre erroné :**
La comparaison utilise des instantanés pris à des moments différents.

**Pourquoi la recommandation change :**
La différence de 30 unités peut représenter des expéditions, des retours, des ajustements ou d'autres mouvements survenus entre les deux instantanés.

**Approche correcte :**
D'abord établir un instant de coupure commun et comparer des instantanés d'inventaire comparables.

| Approche                 | Résultat                                             |
| ------------------------ | -------------------------------------------------- |
| Instants d'instantanés différents | Différence de 30 unités traitée comme une perte                 |
| Coupure commune           | Seul l'écart résiduel inexpliqué fait l'objet d'une enquête |

La source identifie spécifiquement l'incohérence de l'instant de coupure comme une cause de fausses différences.

La décision corrigée est donc **« enquêter sur l'écart résiduel »**, et non **« réclamer la totalité de l'écart comme dépréciation ».**

<details>
<summary>Logique de calcul</summary>

```text
Comparable Variance
= Quantity at Node A
- Quantity at Node B

Only when:
Snapshot_A_Time = Snapshot_B_Time
```

Un écart ne doit pas être interprété comme une perte financière tant que la base de comparaison elle-même n'est pas valide.

</details>

#### Piège 2 — Classer les problèmes par unités plutôt que par argent

**Décision :**
L'opérateur trie le rapport de réconciliation par le plus grand écart de quantité.

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

L'architecture source demande explicitement d'introduire une matrice de coûts SKU afin que les différences de quantité puissent être traduites en perte financière.

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

La deuxième exception présente la quantité la plus faible mais la conséquence financière la plus importante.

</details>

#### Piège 3 — Supposer qu'un appariement SKU propre signifie des données propres

**Décision :**
L'opérateur utilise une recherche directe entre les trois exports et suppose que les enregistrements non appariés représentent un inventaire manquant.

**Hypothèse erronée :**
Les chaînes SKU sont présumées identiques entre les systèmes.

**Pourquoi la recommandation change :**
Les données exportées peuvent contenir des espaces initiaux ou finaux, une casse incohérente, des caractères spéciaux, des lignes vides ou des conventions historiques de nommage des SKU. La source identifie spécifiquement ces éléments comme des problèmes pratiques de qualité des données.

Par exemple :

```text
Shopify → "sku-001"
WMS     → "SKU-001"
3PL     → " SKU-001 "
```

Un appariement exact naïf peut interpréter ces éléments comme des produits différents.

**Approche correcte :** normaliser l'identifiant avant la recherche inter-systèmes.

<details>
<summary>Logique de normalisation</summary>

```excel
=UPPER(TRIM([@SKU]))
```

Utilisez ensuite la clé normalisée pour la récupération inter-tables.

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

Cela réduit les fausses exceptions causées par le formatage plutôt que par un mouvement d'inventaire.

</details>

### Exemple de scénario

Supposons qu'une réconciliation hebdomadaire soit effectuée pour un seul SKU après que les trois systèmes ont été capturés au même instant de coupure.

Les instantanés importés déclarent :

| Source  | Quantité |
| ------- | -------: |
| Shopify |    1,000 |
| WMS     |      992 |
| 3PL     |      970 |

Le coût unitaire configuré du SKU est de **$18**.

Le premier geste analytique n'est pas de déclarer 30 unités perdues. Le système établit les différences entre chaque position d'inventaire déclarée :

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

Si l'écart de 22 unités côté 3PL reste inexpliqué après vérification du calendrier d'expédition, des retours, des ajustements et d'autres mouvements légitimes, l'exposition financière estimée au coût configuré est :

```text
22 × $18 = $396
```

L'implication managériale est donc différente d'une simple alerte générique de stock.

L'action suivante n'est pas d'inspecter chaque SKU de manière égale. L'opérateur doit enquêter **d'abord sur l'exception côté 3PL**, vérifier si l'écart représente une perte physique, un dommage, une question de calendrier ou un problème de reporting, puis déterminer si l'écart dépasse la tolérance contractuelle ou interne de l'entreprise.

Le tableau de bord est conçu pour rendre cette priorisation visible : la direction peut voir l'exposition financière totale, la répartition des pertes entre les nœuds et les exceptions de SKU de valeur la plus élevée sans parcourir manuellement les exports bruts.

L'outil prend donc en charge une séquence :

**réconciliation → isolement des exceptions → quantification financière → investigation opérationnelle → réclamation potentielle ou correction de processus.**

Il ne détermine pas lui-même si un écart est juridiquement recouvrable. Cela reste une décision managériale et contractuelle.

### Référence des formules

Les formules ci-dessous décrivent les schémas de calcul principaux spécifiés pour l'architecture de réconciliation. Elles visent à rendre le raisonnement du classeur auditable, et non à transformer le README en un catalogue générique de formules Excel.

<details>
<summary>Normalisation des SKU</summary>

**Objectif :** standardiser les chaînes SKU importées avant comparaison.

```excel
=UPPER(TRIM([@SKU]))
```

**Logique :**

* `TRIM()` supprime les espaces initiaux, finaux et redondants.
* `UPPER()` standardise la casse des lettres.
* La clé normalisée résultante devient apte à l'appariement inter-systèmes.

La source recommande spécifiquement `TRIM()` et `UPPER()` à cette fin.

</details>

<details>
<summary>Recherche inter-systèmes</summary>

**Objectif :** récupérer la quantité correspondante d'une table source après que le SKU a été standardisé.

```excel
=XLOOKUP(
    Normalized_SKU,
    Source_SKU_Column,
    Source_Quantity_Column,
    0
)
```

L'architecture autorise `XLOOKUP` ou `INDEX + MATCH` comme mécanisme de récupération inter-tables.

Le principe de conception important n'est pas la fonction de recherche spécifique. C'est que **l'identité SKU, plutôt que la position de ligne, contrôle la réconciliation**.

</details>

<details>
<summary>Calcul des écarts</summary>

**Objectif :** quantifier la différence entre des positions d'inventaire comparables.

```text
Absolute Variance
= Source Quantity - Reference Quantity
```

L'implémentation doit conserver le signe lorsque l'interprétation directionnelle est utile et utiliser des valeurs absolues pour classer l'ampleur de l'écart.

```text
Variance Magnitude
= ABS(Source Quantity - Reference Quantity)
```

Cela prend en charge à la fois :

* la réconciliation directionnelle ;
* le classement des exceptions.

</details>

<details>
<summary>Conversion en perte financière</summary>

**Objectif :** convertir un écart d'inventaire en une exposition financière estimée.

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

Le coût unitaire est maintenu dans `Config_Master`, ce qui permet de réutiliser le même moteur de réconciliation lorsque les coûts produits changent.

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

La conception source prévoit que `Config_Master` maintienne les seuils d'écart et que la mise en forme conditionnelle signale les lignes dont la quantité ou le taux d'écart franchit la limite configurée.

</details>

### Règles de validation

Le moteur de réconciliation dépend d'un petit nombre de contrôles qui doivent être respectés avant que la sortie puisse être considérée comme de niveau décisionnel.

| Champ / Contrôle                  | Règle                                                                                                           | Comportement en cas d'erreur                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **SKU**                          | Doit être standardisé et identifiable de manière cohérente entre les fichiers sources.                                        | Les enregistrements non appariés ou mal formés doivent être traités comme des exceptions de qualité de données plutôt que classés silencieusement comme dépréciation. |
| **Unicité des SKU**               | Un produit physique doit correspondre à une identité SKU standard unique.                                                  | Les identifiants en double ou conflictuels exigent une correction des données maîtresses avant toute réconciliation fiable.                       |
| **Coût unitaire**                    | Doit exister dans `Config_Master` pour la valorisation financière.                                                         | L'écart de quantité peut rester visible, mais l'exposition financière ne peut pas être valorisée de manière fiable sans coût.                    |
| **Coupure des instantanés**             | Les données Shopify, WMS et 3PL doivent représenter le même point temporel.                                               | Des horodatages différents peuvent créer de faux écarts et nécessitent une réexportation ou un ajustement.                                       |
| **Données sources importées**         | Les exports bruts doivent être collés de manière cohérente dans leurs zones d'import désignées.                                  | Les anomalies structurelles ou de format source doivent être corrigées avant d'interpréter les exceptions résultantes.                   |
| **Seuil d'écart**        | Les seuils de quantité/taux doivent être maintenus dans la configuration plutôt que codés en dur dans les sorties individuelles. | Les exceptions franchissant le seuil sont mises en évidence pour investigation.                                                      |
| **Tolérance 3PL / SLA**          | La tolérance contractuelle aux pertes doit être prise en compte pour décider si une exception justifie une réclamation.              | Le classeur fournit les preuves ; la direction détermine si une réclamation contractuelle doit être engagée.                    |
| **Calendrier des retours**               | Les retours enregistrés par un 3PL et les remboursements enregistrés dans Shopify peuvent survenir à des moments différents.                        | Les écarts à court terme ne doivent pas être automatiquement interprétés comme une dépréciation permanente.                                     |
| **Nommage historique des SKU**        | Les incohérences de nommage héritées doivent être normalisées ou mappées.                                                    | Les SKU historiques non mappés doivent rester visibles comme exceptions de qualité de données.                                                |
| **Délai de synchronisation des systèmes** | Les problèmes temporaires de synchronisation Shopify/3PL échappent à la logique de réconciliation du tableur.               | À traiter comme un problème d'intégration système plutôt que de forcer une solution de contournement VBA dans le tableur.                               |

La source distingue explicitement les problèmes qu'Excel peut résoudre de ceux nécessitant une intervention opérationnelle ou au niveau du système. La réconciliation standardisée, la valorisation des pertes et les tableaux de bord d'exceptions relèvent du classeur ; la discipline de comptage cyclique, la gestion des réclamations 3PL, la synchronisation des API et le suivi GPS n'en relèvent pas.



### Ce que ce classeur ne tente pas de résoudre

L'architecture maintient délibérément une frontière claire autour de la couche Excel.

**Problèmes de gestion opérationnelle :**

* procédures de comptage cyclique 3PL incohérentes ;
* fréquence insuffisante des comptages physiques d'inventaire ;
* absence d'engagement de réclamations lorsque les limites de pertes contractuelles sont dépassées.

Ces problèmes exigent une action managériale plutôt qu'une formule supplémentaire.

**Problèmes d'intégration système :**

* délais de synchronisation en temps réel Shopify ↔ 3PL ;
* communication API ;
* intégration ERP automatisée.

La source recommande spécifiquement de ne pas forcer ces problèmes dans un classeur Excel léger via VBA.

**Problèmes de visibilité du transport :**

* suivi GPS en temps réel des stocks en transit ;
* flux de travail de gestion des transports.

Ces problèmes exigent un TMS dédié plutôt qu'un tableur de réconciliation des stocks.

Cette frontière est intentionnelle. L'objectif du classeur est de fournir une **couche répétable de réconciliation et d'analyse des pertes financières**, et non de prétendre que chaque problème de contrôle des stocks est un problème Excel.

### Obtenir le classeur

L'outil est conçu pour une réconciliation récurrente plutôt que pour une analyse ponctuelle de tableur.

Le cycle opérationnel prévu est :

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

**Version Excel :** utilisez le classeur lorsque la réconciliation doit être actualisée avec les exports réels Shopify, WMS et 3PL.

L'outil est délibérément conçu pour qu'un utilisateur opérationnel ou financier non technique puisse réaliser la réconciliation récurrente sans reconstruire le modèle analytique à chaque fois. L'objectif source est d'environ **10 minutes** pour le nettoyage, la réconciliation et l'examen des exceptions.

### Limites

Ce classeur est une **couche de réconciliation et d'analyse des pertes**, et non une plateforme de contrôle des stocks.

Il ne peut pas :

* garantir la synchronisation en temps réel Shopify ↔ WMS ↔ 3PL ;
* empêcher un opérateur d'entrepôt d'expédier physiquement un article lorsque le stock est insuffisant ;
* remplacer un WMS, un ERP ou un système de gestion des stocks ;
* imposer les procédures de comptage cyclique 3PL ;
* déterminer automatiquement si un écart est contractuellement recouvrable ;
* fournir un suivi GPS en temps réel des stocks en transit ;
* résoudre des problèmes historiques de données maîtresses de SKU sans une décision de mappage appropriée.

Ces frontières sont explicites dans la conception source. La réconciliation standardisée, la valorisation des écarts, le classement des exceptions et le reporting du tableau de bord sont considérés comme des problèmes Excel appropriés. La discipline de comptage cyclique et la gestion des réclamations 3PL exigent des contrôles managériaux ; la synchronisation API en temps réel relève de l'intégration système ; le suivi physique des expéditions relève d'un TMS.

Il existe également d'importantes contraintes d'interprétation.

**Une différence de quantité n'est pas automatiquement une dépréciation.** Les retours peuvent être enregistrés par un 3PL à un moment différent du remboursement Shopify correspondant, et un calendrier d'instantanés incohérent peut créer des différences temporaires. L'opérateur doit valider le contexte métier avant de classer un écart comme perte permanente.

**Le chiffre de perte financière est une estimation, pas une écriture comptable.** Il dépend du coût unitaire SKU configuré et de l'interprétation de la différence de quantité sous-jacente.

**Un résultat de tableur propre ne garantit pas des données sources propres.** Les incohérences historiques de nommage des SKU, les exports incomplets, les enregistrements en double ou des comptages physiques incorrects peuvent encore produire des conclusions trompeuses.

Le classeur doit donc être utilisé comme un **mécanisme d'établissement des faits et de priorisation**, et non comme un moteur de jugement automatique.

</details>


## Autres outils de cette série

Une collection d'outils Excel légers d'aide à la décision couvrant le contrôle opérationnel, la réconciliation, la rentabilité, les stocks et l'analyse financière.

* **[inventory-planning-reorder-point-excel](https://github.com/HyVoid/inventory-planning-reorder-point-excel)** — Quelle décision d'achat faut-il prendre aujourd'hui, compte tenu des tendances de la demande, des délais et des contraintes de trésorerie ? — Prévoyez les besoins d'inventaire en combinant signaux de demande, risques de délai, recommandations d'achat et exposition du fonds de roulement.
* **[Retail-SKU-Concentration-Assortment-Diagnostic-Console](https://github.com/HyVoid/Retail-SKU-Concentration-Assortment-Diagnostic-Console)** — Quels produits dominent le risque d'inventaire ou diluent la qualité de l'assortiment ? — Identifiez le risque de concentration SKU et l'efficacité de l'assortiment dans les catalogues de produits de détail.
* **[Retail-and-Maquila-Inventory-Ledger](https://github.com/HyVoid/Retail-and-Maquila-Inventory-Ledger)** — Où l'inventaire circule-t-il entre les opérations de détail et de maquila ? — Suivez les mouvements d'inventaire, les pertes de traitement et l'exposition de stock entre usines, entrepôts et magasins.
* **[Universal-3D-Cargo-Loading-Optimization-Simulator](https://github.com/HyVoid/Universal-3D-Cargo-Loading-Optimization-Simulator)** — Comment charger le fret pour réduire l'espace gaspillé et les frictions opérationnelles ? — Simulez des configurations de chargement 3D pour maximiser la capacité des conteneurs et l'efficacité d'expédition.
* **[Cross-Border-DTC-Inventory-Governance-Console](https://github.com/HyVoid/Cross-Border-DTC-Inventory-Governance-Console)** — Quelle est la vraie demande d'achat après exclusion des engagements de précommande et des retours attendus ? — Reconstruisez les signaux de demande réels en isolant les obligations de précommande et le comportement de retour des données de ventes brutes.
* **[inventory-allocation-fulfillment-excel](https://github.com/HyVoid/inventory-allocation-fulfillment-excel)** — Chaque commande client peut-elle réellement être livrée à temps, compte tenu du stock physique, des réservations, des conteneurs en transit et des bons de commande ouverts sur l'ensemble de nos sites ? — Calculez les quantités disponibles à la promesse et les besoins nets d'approvisionnement en réconciliant le stock physique, les réservations de commandes, l'inventaire en transit et les bons de commande ouverts sur plusieurs sites.

## Licence

Ce projet est publié sous la **licence Apache 2.0**.

Vous pouvez utiliser, modifier, distribuer et adapter le projet conformément aux termes et conditions de la licence Apache 2.0.

Consultez le fichier de licence du dépôt pour le texte complet de la licence.

