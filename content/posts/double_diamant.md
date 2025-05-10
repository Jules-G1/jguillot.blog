---
title: "💎 Quand la Data Rencontre le Double Diamant : L'Équation du Succès"
date: 2024-11-08T00:00:00+00:00
tags: ["Product Analytics"]
author: "Jules Guillot"
showToc: true
TocOpen: false
draft: false
hidemeta: false
comments: true
canonicalURL: "https://canonical.url/to/page"
disableHLJS: true # to disable highlightjs
disableShare: true
disableHLJS: false
hideSummary: true
searchHidden: true
ShowReadingTime: true
ShowBreadCrumbs: true
ShowPostNavLinks: true
ShowWordCount: false
ShowRssButtonInSectionTermList: true
UseHugoToc: true
cover:
    image: "dd_image.png" # image path/url
    alt: "<alt text>" # alt text
    caption: "<text>" # display caption under cover
    relative: false # when using page bundles set this to true
    hidden: true # only hide on current single page
editPost:
    URL: "https://github.com/Jules-G1/jguillot.blog/content"
    Text: "Suggest Changes" # edit text
    appendFilePath: true # to append file path to Edit link
---


Travailler dans un environnement de start-up ou de scale-up présente un éventail de défis uniques, notamment en matière de priorisation des initiatives de développement produit. Face à des contraintes de temps et de ressources, il est essentiel de ne pas se reposer uniquement sur l'intuition pour déterminer la marche à suivre. L'analyse de données devient alors un outil stratégique crucial pour guider les décisions, en éclairant le chemin qui mène d'une idée large à une action ciblée et efficace.

Dans cet article, nous explorerons comment l'analyse de données peut être intégrée dans chaque étape du modèle du double diamant, un cadre méthodologique clé en développement produit.


{{< inTextImg url="https://upload.wikimedia.org/wikipedia/commons/6/65/Double_Diamond_by_the_Design_Council.png" height="280" >}}


Design Council - https://www.designcouncil.org.uk/our-work/the-double-diamond/ ([CC BY 4.0](https://creativecommons.org/licenses/by/4.0))

## Qu'est-ce que le Double Diamond ?

Le double diamant est le nom d'un modèle de processus de conception popularisé par le British Design Council en 2005, adapté du modèle divergence-convergence proposé en 1996 par le linguiste américain d'origine hongroise Béla H. Bánáthy[1][2]. Il est principalement utilisé dans les domaines du design et de la gestion de produit pour structurer le processus de développement. Le modèle est divisé en quatre phases : deux de divergence (exploration large) et deux de convergence (focalisation et finalisation), permettant aux équipes de passer de l'identification d'un problème à la mise en œuvre d'une solution efficace.

Bien que le modèle soit souvent appliqué dans des contextes où la donnée qualitative prime (comme les interviews utilisateurs), il peut être enrichi par une approche quantitative. En tant que data analyst, l'objectif est d'utiliser ce cadre pour soutenir les Product Managers et Product Designers dans la prise de décisions éclairées.

## Étape 1 : Découverte du Problème (Discovery Phase)

**Objectif :** La première phase du double diamant consiste à explorer un large éventail de problèmes potentiels au sein du produit. L'idée est d'élargir le champ d'analyse pour identifier les défis qui méritent d'être résolus.

**Approche :** L'analyse de données dans cette phase doit permettre d'identifier des signaux d'alerte à travers des Key Performance Indicators (KPI) et d'autres métriques pertinentes. Pour ce faire, il est essentiel de se baser sur trois critères principaux : l'urgence, l'impact, et l'effort requis.

- **L'urgence :** Les dégradations observées dans les KPI critiques, comme une hausse du taux de churn ou une baisse significative des taux de conversion, peuvent indiquer des problèmes à résoudre en priorité. Par exemple, si l'on remarque une baisse dans le taux de conversion des utilisateurs après une certaine étape du funnel, cela pourrait indiquer un obstacle spécifique qui nécessite une analyse approfondie.
- **L'impact :** L'analyse de données doit permettre d'estimer quel levier aura le plus d'impact sur le business. Par exemple, on peut comparer l'effet d'une amélioration de la conversion de 1% avec une augmentation de l'acquisition de 10%. Une analyse de sensibilité basée sur des données historiques peut aider à identifier l'action qui apportera le plus de valeur.
- **L'effort :** Il est crucial d'évaluer la marge de manœuvre et les ressources nécessaires pour améliorer un KPI. Par exemple, si un KPI est déjà proche de son potentiel maximum, les gains marginaux pourraient ne pas justifier l'investissement en temps et en ressources.

**Outils utilisés :** Durant cette phase, les outils accessibles comme SQL et les tableaux de bord analytiques restent les plus pertinents pour explorer les données à grande échelle. A condition, pour les dashboards, d’être déjà existants et suffisant macro. Une approche plus technique pourrait impliquer Python pour des analyses plus complexes, comme la modélisation prédictive ou l'analyse de cohortes.

**Exemple :** Imaginons que l'analyse révèle une baisse du taux de conversion sur un produit de commerce en ligne. En creusant dans les données, on pourrait découvrir que cette baisse est liée à un problème spécifique de l'interface utilisateur lors du processus de paiement, ce qui nécessiterait une attention immédiate.

## Étape 2 : Définir le Projet (Define Phase)

**Objectif :** Après avoir exploré divers problèmes potentiels, il s'agit de converger vers un problème spécifique sur lequel se concentrer.

**Approche :** Cette phase consiste à resserrer le périmètre de l'analyse en se focalisant sur un segment de problème précis. L'objectif est d'affiner les hypothèses en s'appuyant sur une analyse comparative des différentes populations d'utilisateurs.

- **Segmentation des utilisateurs :** Une analyse approfondie des segments d'utilisateurs peut révéler des variables discriminantes. Par exemple, en comparant les utilisateurs ayant des taux de rétention élevés avec ceux qui abandonnent rapidement, on pourrait découvrir que les utilisateurs qui interagissent avec une certaine fonctionnalité sont plus susceptibles de rester actifs.
- **Hypothèses d'impact :** Une fois le problème ciblé, il est important de formuler des hypothèses sur l'impact potentiel des différentes interventions. Par exemple, si l'analyse montre que les utilisateurs qui reçoivent des notifications personnalisées ont un taux d'engagement plus élevé, l'hypothèse pourrait être que l'amélioration de l'algorithme de personnalisation pourrait augmenter le taux d'engagement global.
- **Définir les KPI de succès :** Cette phase doit également aboutir à la définition de KPI clairs pour mesurer le succès de l'initiative. Ces KPIs doivent être directement liés aux objectifs stratégiques de l'entreprise et aux résultats attendus de l'intervention.

**Outils utilisés :** Outre les outils d'analyse classiques, cette phase peut nécessiter des techniques de machine learning ou d’inférences causale pour segmenter les utilisateurs, comprendre et prédire l'impact des différentes actions.

**Exemple :** Supposons que l'analyse des données montre que les utilisateurs qui reçoivent une recommandation personnalisée lors de leur première visite ont un taux de conversion nettement supérieur. Le projet pourrait alors se concentrer sur l'amélioration de cet algorithme de recommandation, avec des KPI de succès comme l'augmentation du taux de conversion des nouveaux utilisateurs.

## Étape 3 : Développer des Idées (Development Phase)

**Objectif :** À ce stade, il s'agit de développer et tester des solutions potentielles pour le problème identifié.

**Approche :** L'analyse de données joue un rôle crucial dans la conception et la validation des idées. Il est important d'utiliser des méthodes de web analyse et d'expérimentation pour tester les hypothèses formulées lors de la phase précédente.

- **Analyse du comportement utilisateur :** En analysant le trafic, les points d'entrée, et les parcours utilisateurs, on peut identifier des opportunités pour améliorer l'expérience. Par exemple, un taux de rebond élevé sur une page spécifique pourrait indiquer un problème de contenu ou de mise en page. A l’inverse, on peut s’inspirer de parcours utilisateurs ayant de bonnes performances.
- **Expérimentations et tests A/B :** Pour valider les hypothèses, des tests A/B peuvent être mis en place. Par exemple, si l'on soupçonne qu'une nouvelle mise en page pourrait améliorer la conversion, un test A/B pourrait comparer l'ancienne et la nouvelle version pour mesurer l'impact.
- **Feedback utilisateurs :** Les retours qualitatifs des utilisateurs peuvent être intégrés à l'analyse pour affiner les solutions. Par exemple, si des utilisateurs se plaignent d'une fonctionnalité spécifique, une enquête peut être conduite pour collecter des données supplémentaires, qui seront ensuite croisées avec les données quantitatives pour valider ou invalider ces perceptions.

**Outils utilisés :** Les outils de web analytics (Google Analytics, Mixpanel, Amplitude …) sont particulièrement utiles pour suivre les interactions utilisateurs. Les tests A/B peuvent être utilisés pour évaluer l'impact des changements.

**Exemple :** Supposons que l'analyse révèle que les utilisateurs abandonnent souvent leur panier d'achat après avoir vu les frais de livraison. Un test A/B pourrait être lancé pour comparer l'impact de l'affichage des frais de livraison dès le début du processus d'achat, par rapport à l'affichage traditionnel à la fin.

## Étape 4 : Livraison et Évaluation de l'Impact (Delivery Phase)

**Objectif :** La dernière phase du double diamant consiste à livrer la solution finale et à évaluer son impact sur le produit. On peut aussi considérer cette étape comme la première du nouvelle boucle du double diamond. En cas de performance moins bonnes qu’attendus, les informations collectés lors de la delivery nourrissent l’itération suivante.

**Approche :** L'évaluation de l'impact d'une solution nécessite une analyse rigoureuse pour comprendre son efficacité et ses implications à long terme.

- **Suivi des KPI de succès :** Les KPI définis lors de la phase de focalisation doivent être suivis de près pour mesurer le succès de la solution. Par exemple, si l'objectif était d'améliorer le taux de conversion des nouveaux utilisateurs, le suivi de ce KPI permettra de vérifier si la solution déployée atteint ses objectifs.
- **Surveillance des effets secondaires :** Il est crucial de surveiller les effets de la solution sur d'autres parties du produit. Par exemple, une amélioration du taux de conversion pourrait entraîner une surcharge du service client si le produit n'est pas prêt à gérer une augmentation du nombre d'utilisateurs.
- **Analyse post-implémentation :** Une analyse approfondie après la mise en œuvre permet de comprendre l'impact à long terme de la solution. Par exemple, après avoir livré une nouvelle fonctionnalité, il est important de mesurer non seulement son adoption immédiate, mais aussi sa rétention à moyen et long terme.

**Outils utilisés :** Les tableaux de bord en temps réel, les rapports automatisés, et les outils de monitoring sont essentiels pour suivre l'impact en continu.

**Exemple :** Après avoir lancé une nouvelle fonctionnalité de recommandation, une analyse post-implémentation pourrait révéler que bien que la fonctionnalité ait augmenté les conversions initiales, elle n'a pas réussi à maintenir l'engagement à long terme. Ce type d'analyse permet de boucler la boucle et de retourner à la phase de découverte si nécessaire.

## Conclusion

Le double diamant offre un cadre robuste pour structurer l'approche produit, et l'intégration de l'analyse de données à chaque étape de ce processus permet de garantir que les décisions sont fondées sur des preuves tangibles. En tant que (product) data analyst, il est crucial et d’autant plus intéressant de fournir ces insights tout au long du parcours, en veillant à ce que chaque décision soit prise avec une compréhension claire des données sous-jacentes.

En adoptant cette méthodologie, non seulement vous maximisez l'impact de vos initiatives, mais vous contribuez également à un développement produit plus informé et plus efficace.

---

*Article développé à partir de mes notes, pour le webinar dataScientest: [Double Diamond : Conduire des implémentations Produit de manière data-driven @Malt](https://www.youtube.com/watch?v=7XLdBThKnUk). Rédaction améliorée par ChatGPT.*

---

*Sources :*
1.  *Banathy, Bela H. (1996). [Designing Social Systems in a Changing World](https://www.springer.com/gp/book/9780306452512). Springer US. p. XV, 372. [ISBN](https://en.wikipedia.org/wiki/ISBN_(identifier)) [978-0-306-45251-2](https://en.wikipedia.org/wiki/Special:BookSources/978-0-306-45251-2).*
2. *Möller, Ola (9 January 2015). ["The Double Diamond"](https://web.archive.org/web/20221221104005/https://blog.methodkit.com/the-double-diamond-16c74e3c4869). MethodKit Stories. Archived from [the original](https://blog.methodkit.com/the-double-diamond-16c74e3c4869) on 21 December 2022. Retrieved 3 September 2019.*
