Par Maxence Briquet, Matthieu Delafon, Abdelkarim Khalid, Marceau Macquignon, Marie Poff.

Voici les résultats de notre étude sur la bse de données "DPE logements existants depuis juillet 2021", disponible à l'adresse suivante : https://data.ademe.fr/datasets/dpe-v2-logements-existants

## Introduction

Dans le contexte actuel de crise de l’énergie concomitant au retour de la guerre en Europe, la sobriété énergétique est un sujet gagnant en popularité. Le gouvernement a donné sa consigne de maintien des thermostats à 19°C, afin de s’assurer l’évitement de coupures de courant lors de l’hiver. Il est aujourd’hui de plus en plus stratégique de n’avoir besoin de consommer que peu. L’isolation thermique est à ce jour l’un des meilleurs moyens pour ce faire, et est encouragée depuis plusieurs années par l’Etat, via notamment la politique du DPE : le diagnostic de performance énergétique. Il convient donc de s’attarder quelques temps sur cet indicateur mis en place par l’administration, dont les modalités ont récemment été modifiées. 

Comme le disait déjà le physicien Kelvin au XIXème siècle, « If you cannot measure it, you cannot improve it ». Il est de même dans la conduite d’une politique publique, qui se doit d’être constamment éprouvée par des chiffres qui en témoignent de l’efficacité, sans quoi sa poursuite ne saurait être justifiée. 

Pour évaluer la pertinence du DPE, nous chercherons principalement à établir la qualité – théorique – de l’indicateur en soi (est-il un véritable reflet de ce qu’il cherche à mesurer ?), la qualité en pratique de cet indicateur, sa fiabilité dans la récolte des données (est-on en pratique capables d’obtenir un indicateur fiable et pertinent, avec des données homogènes sur le territoire ?), et sur la mise en lumière des usages de l’indicateur (permet-il dans les faits aux pouvoirs publics d’avoir une vue sur ce qu’ils cherchent à savoir et peuvent-ils se baser sur ce système ?) ; et ainsi mettre en valeur les critiques et contre-critiques qui pourraient être faites au DPE.

Nous étudierons donc dans un premier temps la construction de cet indicateur (i), pour ensuite en comprendre les limites (ii). Enfin, nous développerons les divers usages de l'indicateur et de la base de données, pour en finaliser l'analyse (iii). 

## I. La construction d'un indicateur pour quantifier la performance énergétique

### Choix des informations sur le logement et les équipements qui permettent le calcul de l’indicateur
Le Diagnostic de Performance Énergétique (DPE) renseigne sur la performance énergétique et environnementale d’un logement ou d’un bâtiment, en évaluant sa consommation d’énergie et son impact en matière d’émissions de gaz à effet de serre. Il s’inscrit dans le cadre de la politique énergétique définie au niveau européen afin de réduire la consommation d’énergie des bâtiments et de limiter les émissions de gaz à effet de serre.

Le contenu et les modalités d’établissement du DPE sont réglementés. Le DPE contient des informations sur les caractéristiques du bâtiment ou du logement (surface, orientation, murs, fenêtres, matériaux, etc.) ainsi que sur ses équipements (de chauffage, de production d’eau chaude sanitaire, de ventilation, etc.) 

## II. Les limites de cet indicateur

### La méthode calcul
A l’aune de la réforme du DPE intervenue en juillet 2021, sa méthode de calcul a évolué. Appelée “3CL” pour “calcul conventionnel des consommations dans les logements” elle a été simplifiée par arrêté ministériel le 8 octobre 2021 afin de prendre en compte 2 critères : l’énergie primaire consommée par le logement (exprimé en kWh.ép/m².shab/an) et les émissions de gaz à effet de serre du logement (exprimées en kg eq CO2/m²/an).

5 critères sont pris en compte dans cette nouvelle méthode de calcul. Tout d’abord, les déperditions de l’enveloppe, issues du manque d'isolation des murs, des combles et du sol du logement. La nouvelle méthode a notamment fait évoluer la valeur du coefficient thermique qui permet de quantifier les déperditions de chaleur d’un matériau isolant afin de mieux tenir compte de l’amélioration des techniques de construction. 

Sont ensuite prises en compte les déperditions incombant aux flux d’air dans le logement. Elles peuvent être de 2 natures, soit par l’ouverture des fenêtres soit par la perméabilité à l’air du bâtiment ou du logement. Viennent également les consommations issues des auxiliaires de ventilation, et du chauffage de l’eau chaude sanitaire jusque-là non prises en compte dans la précédente méthode de calcul. Autre critère essentiel, l’évaluation des coûts annuels en énergie par logements. La méthode de cet indicateur a été revue par le décret du 8 octobre car trop éloignée de la réalité des coûts de l’électricité et du gaz. 

La méthode de calcul par tranches successives cumulées a donc été modifiée pour prendre en compte les tranches successives non-cumulées ce qui permet un lissage des estimations du prix des énergies, tout en garantissant l’absence d’effet de seuils, objectif premier de cette méthode. Enfin, le dernier indicateur pris en compte est le confort d’été relatif à la qualité de vie dans le logement face à la chaleur.

![Image4](https://user-images.githubusercontent.com/118830345/203367696-3134c832-896c-4ce5-a1ca-0d106a8be1da.png)

Source : Institut national de la consommation, 2021

### Les effets de seuil
Si les effets de seuil ont été lissés dans les différentes méthodes de calcul, il n’en est pas de même pour les classifications au sein du DPE. Sur le graphique ci-contre issu des bases de données de l’Ademe, on remarque un effet de seuil important avant chaque nouveau pallier amenant un changement de classification. Ce fait statistique n’est censé exister sur la représentation de cet indicateur qui se veut objectif car répondant à des critères pré-établis étant les mêmes pour tous les logements. 

Au-delà d’un questionnement sur la méthode de calcul en elle-même, c’est davantage d’erreur humaine qui serait à pointer du doigt selon de nombreuses organisations. Ces effets de seuil peuvent en effet s’expliquer par l’importance croissante du DPE dans la vente et l’acquisition d’un bien immobilier, il est donc de plus en plus nécessaire et avantageux pour les vendeur et les bailleurs d’obtenir les meilleurs notations possibles, au risque de ne plus pouvoir louer leur bien à court ou moyen terme. Cet effet de seuil se retrouve d’ailleurs uniquement au niveau des catégories les plus basses E, F et G, celles qui représentent le plus gros enjeu de rénovation thermique.

![Image3](https://user-images.githubusercontent.com/118830345/203368078-4abb7d4b-33f3-4ffb-b09d-a4820de702c0.png)

### Les critiques émises par les associations et les professionnels
Cet indicateur est donc très critiqué. Fin septembre, l’association de consommateur UFC que choisir a rendu publique une enquête réalisée sur le DPE. Ils ont fait évaluer plusieurs maisons 4 ou 5 fois par des diagnostiqueurs différents à chaque fois et le résultat a été assez surprenant. Pour certaines maisons, il y avait jusqu’à 3 classes d’écart (de B à E) ce qui démontre une faiblesse importante dans la méthodologie et la réalisation de ces diagnostics. 

S’en sont ressenti des écarts très importants dans les estimations de la consommation énergétique des bâtiments allant parfois du simple au triple. L’un des principaux problèmes mis en lumière est également la mauvaise concurrence entre les diagnostiqueurs. En effet, ces entreprises privées sont libres de fixer les tarifs qu’elles veulent pour ces diagnostics, ce qui peut avoir des conséquences sur la qualité de la note attribuée via des prestations “low cost”. Cette concurrence n’est pas non plus saine dans la prise en compte de l’importance des différents facteurs qui construisent le DPE. 

Ainsi, dans le même logement, un diagnostiqueur a indiqué que les murs représentent près de 50% des déperditions de chaleur, contre moins de 20% pour un autre diagnostiqueur, ce qui amène de facto des résultats très disparates. Les limites sont donc méthodologiques à cause d’une méthode de calcul considérée comme imparfaite par certains acteurs, économiques du fait de prestations soumis à la concurrence avec des homologations parfois indues et humaines, une limite difficile à estimer et à combler à causes des nombreux biais qu’induit l’intervention humaine.


## III. Les usages de cet indicateur

###2006-2021 : Un indicateur informatif

Transposé en droit Français en 2006, la Directive pour la performance énergétique des bâtiments (2002/91/EG) s’inscrit dans le cadre des initiatives de la communauté européenne visant à comprendre à une échelle plus individuelle l’importance/ la substantialité de nos consommations sur le réchauffement climatique. Ainsi, si la logique de « sobriété, efficacité, compensation » ne s’est démocratiser que plus tard, les considérations d’efficacité énergétique des bâtiments étaient d’ores et déjà considérés comme clés dans le plan de lutte pour réduire la consommation d’énergie (approx un tiers de la consommation de l’UE) et donc des émissions de gaz à effets de serre. Les lacunes traitées par cette directive sont les problématiques d’installations de chauffage et de refroidissement, d'éclairage, d'emplacement et d’orientation des bâtiments et la récupération de chaleur. La transposition de la directive en droit Français a vu naître le Diagnostique de Performance Énergétique, une mesure de la performance énergétique d’un logement. Ainsi, la loi défini la performance énergétique comme la consommation annuelle d’énergie (kWh), le positionnement en consommation d’énergie primaire (kWh/m2/an) et en émission de gaz à effet de serre (gCO2e/m2/an), descriptif du logement (Bâtis, machines, ventilation etc.). Le DPE sert alors à agréger ses informations sous forme d’une note de A (meilleure) à G (pire) et classe alors les logements. Cette note devant systématiquement être mentionnée en cas de vente ou de location.

Bien qu’il fasse partie depuis 2006 de la vie quotidienne des Français, le DPE demeure une classification floue pour les membres de la société et une mesure imprécise et non normalisée pour les acteurs du secteur. En effet, si l’on considère l’univers étudiée (Ω) comme étant le parc de logement en France, les individus et les paramètres (X) les logements, et le DPE la classe (Y) des logements issus des mesures nécessaires, alors les méthodologies de classements ont été remis en cause car il n’y avait pas de définition précise entre les différents acteurs du DPE. Ainsi, indicateurs provenant d’acteurs différents auraient donné des résultats différents pour des logements identiques. Le caractère moyennant de cet indicateur implique ainsi des divergences dans le résultat.

### Après 2021 : Un indicateur normalisé et opposable réellement fiable ?

Pour ces raisons, il a été décidé en 2018, de corriger la définition et le cadre légale du DPE dans le cadre de la loi ELAN dont l’ambition est de « construire plus de logements, simplifier les normes, protéger les plus fragiles et mettre les transitions énergétique et numérique au service des habitants ». La refonte du DPE entrera en vigueur en totalité le 1er juillet 2021 et aura pour vocation d’être plus fiable et lisible.

En effet, la méthodologie de calcul a été revue de sorte à uniformiser la catégorisation énergétique du parc de logement. Ainsi, la méthode « sur factures » mentionnée plus haut a été abandonnée et les paramètres à considérer ont été prédéfinis. Ainsi, pour les auditeurs et autres experts, il ne sera plus nécessaire de définir les paramètres (et ce faisant une matrice X) mais n’auront qu’à mesurer et renseigner les équipements énergétiques du logement : la qualité de l’isolation, la ventilation, le type de fenêtres, le système de chauffage etc., mais aussi des paramètres qui s'appliquent à une échelle plus grande que celle du logement, à savoir la prise en compte des scénarios météorologiques. En définissant les données d’entrées, la convergence des résultats est accrue.
Par ailleurs, afin d’assurer la lisibilité des résultats pour les citoyens, la refonte du DPE prévoit aussi la modification de la présentation des résultats de la classification en y rendant notamment plus visible l’estimation des coûts annuels d’énergie du logement, métrique plus compréhensible pour les Français.


Ainsi, la compréhension de la nécessité d’interprétabilité de cette mesure par les autorités compétentes montre que le DPE pré-2021 ne suffisait pas pour atteindre l’objectif initial d’information pour les citoyens. De plus, le nouveau cahier de charge prévoit aussi de rendre le document du DPE plus complet, en y renseignant aussi des mesures qui concerne l’usager du logement directement à savoir, le confort d’été (hors climatisation), le schéma des déperditions de chaleur ainsi que les recommandations et travaux nécessaires pour améliorer les performances énergétiques du logement et les coûts liés.

Finalement, le nouveau DPE devient opposable. Ainsi, le document aura valeur juridique au même titre que les autres audits du bâtiment (sécurité électrique, présence d’amiante etc.). De ce fait, le résultat de la classification pourra être utilisé par les autorités pour définir des réglementations comportant potentiellement des mesures coercitives ou des interdictions, comme notamment le gel de l’augmentation des loyers ou l’interdiction des locations pour les passoires thermiques.

La refonte du DPE traduit ainsi d’une part la nécessité de normalisation des méthodes de calculs assurant la comparabilité des mesures et donc le niveau de fiabilité à l’échelle nationale d’une mesure qui a vocation d’être à échelle nationale, la réflexion a alors été mené sur les données d’entrées ainsi que le système ou « moteur » de calcul utilisé pour la classification. D’autre part, cette révision met en exergue aussi l’importance des informations communiqués pour répondre à l’objectif initiale du DPE (comprendre l’efficacité énergétique du parc de logement nationale en mesurant, ou en prévoyant sa consommation d’énergie primaire), la réflexion se porte ici alors sur les données de sorties considérés, leur présentation mais aussi, le poids juridique et réglementaire de ces données.

## IV. Les usages que permettent cette base de données

### La collecte des données par l'ADEME
Depuis 2013, et faisant suite à la Loi n° 2010-788 du 12 juillet 2010 portant engagement national pour l'environnement, tous les DPE réalisés doivent être transmis à l’ADEME. Ces dispositions ont été renforcées par l’Arrêté du 31 mars 2021 relatif aux méthodes et procédures applicables au diagnostic de performance énergétique et aux logiciels l’établissant, précisant que la transmission des diagnostics réalisés par les logiciels conformes à la méthode de calcul dite “3CL” est obligatoire, et se fait par voie informatique.

L’ADEME a ainsi créé l’Observatoire DPE pour collecter et publier ces données, et notamment permettre de retrouver le contenu d’un DPE, d’avoir accès à une liste de diagnostiqueurs, de pouvoir consulter des statistiques ou télécharger des base de données, et potentiellement à l’avenir d’effectuer des simulations de DPE. 

Depuis la généralisation de cette nouvelle méthode de calcul, au 1er juillet 2021, plus de 3 millions de DPE logements ont été reçus par l’Observatoire DPE de l’ADEME, 268 297 pour le mois d’octobre 2022.

Depuis le 3 août 2022, les DPE collectés depuis le 1er juillet 2021 par l’Observatoire DPE sont disponibles en Open Data, sur le site de l’observatoire DPE ou sur le site de l’ADEME. 

### Manipulations de la base de données pour obtenir un échantillon plus représentatif du parc de logements français
L’une des limites principales de l’exploitation de cette base de données elle sa non-représentativité de l’ensemble du parc de logement en France. L’INSEE dénombrait 37,6 millions de logements en France hors Mayotte au 1er janvier 2022, presque 8,5% des logements français figurent donc dans la bse de données des DPE logements réalisé depuis le 1er juillet 2021 (en admettant qu’il y ai peu de doublons, ce qui est une autre limite de la base de données). Malgré cette taille importante, le DPE ne concerne que les logements neufs, en vente ou en location. Le parc locatif et de logements neufs y est donc surreprésenté. 

Il est cependant possible de redresser cette base de données (en pondérant donc chaque DPE selon les caractéristiques du logement, pour obtenir un échantillon plus représentatif. Pour se faire, plusieurs travaux utilisent les données des Fichiers démographiques sur les logements et les individus (Fidéli) de l’INSEE, qui intègre des données fiscales pour caractériser les différents logements.

On peut citer une étude menée par l’Observatoire national de la rénovation énergétique (ONRE, “Le parc de logements par classe de performance énergétique au 1er janvier 2022”, juillet 2022), qui utilise cette méthode de redressement, et détaille en annexe cette méthodologie. Il faut ainsi noter que l’étape d'appariement entre la bse de données des DPE et le répertoire Fidéli n’est pas toujours exact, car les logements ne disposent pas d’un identifiant propre. C’est donc selon leurs caractéristiques (taille, date de construction, type de logement, localisation géographique, etc.) que l’association est faite entre un DPE et les informations fiscales du répertoire Fidéli.

![Sans titre](https://user-images.githubusercontent.com/115630234/203338449-3763126e-3587-41c8-88a9-467bedb5bc88.png)
Source : Fidéli 2020 ; base des DPE décembre 2021-mars 2022 de l’Ademe, calculs SDSE, à partir de ONRE, “Le parc de logements par classe de performance énergétique au 1er janvier 2022”, juillet 2022.

On remarque ainsi que les classes les moins énergivores sont surreprésentées dans les données des DPE, contrairement aux logements ayant les étiquettes D et E. 

### Une base de données utile pour zoner et cartographier
Les données DPE permettent, notamment pour les collectivités locales, d’avoir une idée de l’état de leur parc de logement. Data.gouv.fr indique ainsi que l’un des usages qui peut être fait de ces bases de données ets le suivant : “Pour les acteurs publics qui souhaitent piloter leurs politiques publiques par la donnée : l'exploitation des données DPE permettrait de mieux caractériser le parc immobilier français, d'identifier les zones d'habitat indigne, de favoriser le recours à certains modes de consommation, etc.” (La base des diagnostics de performance énergétique (DPE) - data.gouv.fr. 2020. En ligne : https://www.data.gouv.fr/fr/posts/la-base-des-diagnostics-de-performance-energetique-dpe/ [consulté le 22 novembre 2022]). 

 Ce sont d’ailleurs des visualisations géographiques qui sont proposées en premier sur le site de l’Observatoire DPE. À partir de ces données, on peut par exemple réaliser une carte représentant le pourcentage de passoires thermiques par région avec les données des DPE établis depuis le 1er juillet 2022. 

![export](https://user-images.githubusercontent.com/115630234/203339992-2102ef2d-f283-48fd-a7c3-0c70f5a9394a.png)
Source : ADEME - Observatoire DPE (Diagnostic de Performance Énergétique). En ligne : https://observatoire-dpe.ademe.fr/statistiques/outil [consulté le 22 novembre 2022]. Traitement avec Magrit.

### Des usages prospectifs, en laissant notamment des acteurs privés ou des chercheurs s’emparer de ces données, avec opérations de valorisation ponctuelles
Du 11 au 22 juin 2020 a eu lieu le Hackathon RenovAction, dont le but était de laisser des développeurs travailler sur des projets de valorisation des données de l’ADEME, dont les DPE et trouver des solutions pour accompagner la rénovation énergétique. Certains projets présentés proposaient par exemple d’identifier sur un territoire le potentiel de rénovation, et faciliter la mise en relations des acteurs qui auraient besoin d’y être impliqués, par une cartographie de la performance énergétique des bâtiment, croisée avec le potentiel de rénovation de ces mêmes bâtiments, selon leurs caractéristiques.

### Bibliographie/Webographie
ADEME. DPE Logements existants (depuis juillet 2021). 2022. En ligne : https://data.ademe.fr/datasets/dpe-v2-logements-existants/full (consulté le 21 novembre 2022).

Freppel, Camille. 37,6 millions de logements en France au 1er janvier 2022 - Insee Focus - 279. 2022. En ligne : https://www.insee.fr/fr/statistiques/6653801 (consulté le 21 novembre 2022).

La base des diagnostics de performance énergétique (DPE) - data.gouv.fr. 2020. En ligne : https://www.data.gouv.fr/fr/posts/la-base-des-diagnostics-de-performance-energetique-dpe/ (consulté le 21 novembre 2022).

LOI n° 2010-788 du 12 juillet 2010 portant engagement national pour l’environnement (1).

Arrêté du 31 mars 2021 relatif aux méthodes et procédures applicables au diagnostic de performance énergétique et aux logiciels l’établissant.

ADEME - Observatoire DPE (Diagnostic de Performance Énergétique). En ligne : https://observatoire-dpe.ademe.fr/statistiques/outil (consulté le 21 novembre 2022).

Le parc de logements par classe de performance énergétique au 1er janvier 2022. En ligne : https://www.statistiques.developpement-durable.gouv.fr/le-parc-de-logements-par-classe-de-performance-energetique-au-1er-janvier-2022-0 (consulté le 21 novembre 2022).

L’Observatoire des diagnostics de performance énergétique – Ademe. En ligne : https://expertises.ademe.fr/batiment/chiffres-cles-observations/lobservatoire-diagnostics-performance-energetique (consulté le 21 novembre 2022).

Fichiers démographiques sur les logements et les individus - Insee. En ligne : https://www.insee.fr/fr/metadonnees/source/serie/s1019 (consulté le 21 novembre 2022).

ADEME - Observatoire DPE (Diagnostic de Performance Énergétique). En ligne : https://observatoire-dpe.ademe.fr/statistiques/outil (consulté le 21 novembre 2022).
