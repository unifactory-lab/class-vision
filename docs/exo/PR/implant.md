# Etude d'implantation

L'utilisation d'algorithmes génératifs, comme les LLM de type ChatGPT, est strictement prohibée à toutes les étapes du projet.

## Compétences
- Utilisation de RoboDK ou Roboguide pour la simulation de robots, de cameras et de leurs environnements.
- Acquisition des bases de la vision industrielle.
- Lecture de documentation techniques.
- Connaissance de l'état de l'art sur les robots, les préhenseurs et la vision industrielle.

## Sujet
Une entreprise spécialisée dans la fabrication de boissons vendues dans des bouteilles en verre souhaite moderniser son outil de production et internaliser la part variable de fabrication de bouteilles actuellement sous-traitée. Ce processus consiste à collecter, trier les bouteilles endommagées, enlever les anciennes étiquettes, laver et conditionner les bouteilles en caisses pour une nouvelle utilisation dans le processus de remplissage, d’étiquetage et de conditionnement avant expédition vers ses clients. L’objectif est de proposer une solution robotisée en sortie de la centrale de lavage sur les opérations d’encaissage et de palettisation.

Description du cycle

- Un poste amont assure le chargement des bouteilles et caisses à laver dans la centrale de lavage
- Les caisses et les bouteilles traversent le poste OP10, la centrale de lavage, qui assure les opérations de lavage et de séchage d’où les bouteilles ressortent séparément sur des convoyeurs :
    - Les caisses vides arrivent propres et sèches sur le convoyeur central.
    - Les bouteilles arrivent propres et sèches sur les deux convoyeurs latéraux situés de part et d’autre du convoyeur central.
    - Les caisses et les bouteilles arrivent positionnées et orientées de façon quelconque sur le convoyeur.
- Les bouteilles sont mises par 24 dans les caisses
- Les caisses pleines sont stockées sur palettes.
- Les palettes pleines sont évacuées par un opérateur à l’aide d’un système de manutention

Informations complémentaires

- Le système de gestion des palettes est constitué de 2 convoyeurs parallèles, un pour l’entrée des palettes vides et l’autre pour la sortie des palettes pleines. Un dispositif assure le transfert automatique d’une palette vide arrivant sur le convoyeur d’entrée vers le convoyeur de sortie. Chaque convoyeur peut recevoir 3 palettes.

- Le remplissage de la palette s’effectue, juste après le transfert, lorsqu’elle se trouve au tout début du convoyeur de sortie.

- Le périmètre de l’ilot est sécurisé par des barrières matérielles. Dans le cadre de la modernisation de cet ilot, les sécurités doivent être upgradées (mises à jour) pour répondre aux normes actuelles.

- Les zones potentielles d’implantation du ou des robots sont déjà identifiées.

- Données dimensionnelles :
    - Caisse : 1,25 kg, 398 x 331 x 259.5 mm
    - Palette : 20kg, 1 000 x 800 x 144 mm
    - Bouteille : 0,45 kg, Ø 65 mm h : 238 mm
    - Hauteur des grillages de sécurité : 2 700 mm/sol
    - Température des produits en sortie de la centrale de lavage : 30°C

<img class="img-no-border" src="../images/impl_size.png" alt="image montrant la taille relative des objets utilisés sur la ligne de production"/>

## Etapes

- Choix des robots, des préhenseurs et des systèmes de vision : type de robots, charge utile, zone de travail, technologie de préhenseur, vision classique, lidar, stéréovision, etc.
- Etude de l'implémentation des materiels choisis : positionnement du matériel, interconnexion, etc.
- Choix et prise en main du logiciel de simulation : RoboDK ou Roboguide (solution FANUC).
- Simulation de la solution de l'implémentation.

## Ressources
- [RoboDK API Examples](https://www.robodk.com/doc/en/PythonAPI/examples.html)
- [Guide des stages](https://moodle-amiens.unilasalle.fr/course/view.php?id=322)
- [Cours de Robotique de Jacques Gangloff](https://www.youtube.com/playlist?list=PLMXdciyMZwAAUlCQ_9mVs_CqQ9YaRTptX)
- [Livre : Robotics](http://pdf.lib.vntu.edu.ua/books/Springer/2020/2019_Book_Robotics.pdf)
- Documentation Roboguide sous format papier.

## Livrables
- ### Fichiers utilisés pour le développement
    - Projet RoboDK (.rdk) / Roboguide

- ### Rapport
    - Page de garde
    - Table des matières
    - Table des figures
    - Introduction : contexte, présentation du sujet, plan du rapport
    - Corps : objectifs détaillés, outils utilisés, méthodologies, travail réalisés, explications des éléments techniques et scientifiques, moyens mis à disposition, difficultés rencontrées et solutions
    - Conclusion : résumé du corps, commentaire sur le résultats, comparaison avec les objectifs fixés, perspectives et potentiel travaux futurs.
    - References : ressources (universitaires, librairies, tutoriels, cours, etc.) utilisés dans le projet.
    - Annexes : documentation pertinente mais non indispensable à la lecture du rapport (documentation technique trop lourde, developpement mathématique, etc.)
