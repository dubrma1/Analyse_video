# Outil d'Analyse Vidéo pour la Physique

Un outil web simple et interactif conçu pour faciliter l'analyse de mouvements à partir de vidéos. Idéal pour les étudiants, les enseignants ou toute personne souhaitant effectuer des mesures de position (x, y) image par image et exporter les données pour une analyse plus approfondie (par exemple, en physique pour étudier la cinématique).

[![Capture d'écran de l'application](https://i.imgur.com/V7gK4zR.png)](https://dubrma1.github.io/Analyse_video/)
*(Remplacez le lien de l'image ci-dessus par une capture d'écran réelle de votre application et assurez-vous que le lien pointe vers votre démo en direct si l'URL est différente).*

## Démo en Direct

Vous pouvez essayer l'outil ici : **[https://dubrma1.github.io/Analyse_video/](https://dubrma1.github.io/Analyse_video/)**
*(Assurez-vous que ce lien correspond à l'URL de déploiement de votre projet sur GitHub Pages. Si votre fichier HTML principal s'appelle `index.html`, ce lien devrait fonctionner si le dépôt s'appelle `Analyse_video`)*

## Fonctionnalités

* **Chargement de Vidéo :**
    * Charge automatiquement une vidéo d'exemple (`Projectile.mp4`) au démarrage.
    * Permet aux utilisateurs de télécharger leurs propres fichiers vidéo.
* **Analyse Image par Image :**
    * Contrôles de navigation : image suivante, image précédente, lecture/pause.
    * Curseur (slider) pour une navigation rapide dans la vidéo.
    * Affichage du numéro de l'image actuelle et du temps écoulé.
* **Collecte de Données :**
    * Interface de pointage intuitive : cliquez sur la vidéo pour marquer la position (x, y) d'un objet.
    * Un marqueur visuel indique le point sélectionné sur l'image courante.
    * Les données (numéro d'image, temps, coordonnées x, y) sont affichées dans un tableau.
* **Gestion des Données :**
    * Possibilité de supprimer des points de données individuels.
    * Bouton pour effacer toutes les données collectées.
* **Exportation :**
    * Exportez facilement les données collectées au format CSV pour une utilisation dans des tableurs (Excel, Google Sheets, etc.) ou des logiciels d'analyse.
* **Interface Utilisateur :**
    * Design épuré et responsive grâce à Tailwind CSS.
    * Icônes Font Awesome pour une meilleure expérience utilisateur.

## Comment Utiliser

1.  **Accéder à l'outil :** Ouvrez le lien de la [Démo en Direct](https://dubrma1.github.io/Analyse_video/).
2.  **Charger une Vidéo :**
    * La vidéo `Projectile.mp4` est chargée par défaut.
    * Pour analyser votre propre vidéo, cliquez sur "Télécharger une autre vidéo" (ou l'intitulé équivalent) et sélectionnez un fichier vidéo depuis votre ordinateur.
3.  **Naviguer dans la Vidéo :**
    * Utilisez les boutons <i class="fas fa-step-backward"></i> (Image Précédente), <i class="fas fa-play"></i>/<i class="fas fa-pause"></i> (Lecture/Pause), et <i class="fas fa-step-forward"></i> (Image Suivante) pour vous déplacer dans la vidéo.
    * Le curseur sous la vidéo permet un accès direct à n'importe quelle image.
4.  **Marquer des Points :**
    * À chaque image où vous souhaitez enregistrer une position, cliquez sur l'objet d'intérêt dans la zone d'affichage de la vidéo.
    * Un point rouge apparaîtra, et les coordonnées (x, y) ainsi que le temps et le numéro de l'image seront ajoutés au tableau "Points Enregistrés".
    * Si vous cliquez à nouveau sur la même image, le point existant pour cette image sera mis à jour.
5.  **Consulter et Gérer les Données :**
    * Le tableau "Points Enregistrés" affiche toutes les données collectées.
    * Pour supprimer un point spécifique, cliquez sur l'icône <i class="fas fa-trash-alt"></i> dans la ligne correspondante du tableau.
    * Pour effacer toutes les données, cliquez sur le bouton "Effacer Tout".
6.  **Exporter les Données :**
    * Lorsque vous avez terminé, cliquez sur le bouton "<i class="fas fa-file-csv"></i> Exporter les Données en CSV".
    * Un fichier `donnees_mouvement.csv` sera téléchargé, contenant vos données prêtes à être analysées.

## Technologies Utilisées

* **HTML5**
* **CSS3**
    * [Tailwind CSS](https://tailwindcss.com/) : Framework CSS utilitaire pour un design rapide et moderne.
* **JavaScript (ES6+)** : Pour toute la logique de l'application, y compris la manipulation vidéo, le dessin sur canvas et l'interaction utilisateur.
* **Font Awesome** : Pour les icônes.

## Pour Exécuter Localement

Si vous souhaitez exécuter ce projet sur votre machine locale :

1.  **Clonez le dépôt :**
    ```bash
    git clone [https://github.com/dubrma1/Analyse_video.git](https://github.com/dubrma1/Analyse_video.git)
    ```
    *(Remplacez `dubrma1/Analyse_video.git` par l'URL SSH ou HTTPS de votre dépôt)*
2.  **Naviguez dans le dossier du projet :**
    ```bash
    cd Analyse_video
    ```
3.  **Ouvrez le fichier HTML :**
    Ouvrez le fichier `index.html` (ou le nom de votre fichier HTML principal) directement dans votre navigateur web.

Aucune étape de construction ou de dépendance complexe n'est nécessaire car il s'agit d'une application purement front-end.

## Améliorations Possibles (Contributions Bienvenues !)

* Calibration de l'échelle (pixels vers unités réelles, par exemple, mètres).
* Définition de l'origine et orientation des axes.
* Détection automatique du frame rate de la vidéo.
* Fonction de zoom/panoramique sur la vidéo.
* Prévisualisation graphique des données (trajectoire x vs y, x vs t, y vs t).
* Support multilingue.
* Amélioration des performances pour l'extraction d'images sur de très longues vidéos.

## Contribuer

Les contributions, les rapports de bugs et les demandes de fonctionnalités sont les bienvenus ! N'hésitez pas à ouvrir une "Issue" pour discuter d'une idée ou d'un problème, ou à soumettre une "Pull Request" avec vos améliorations.

1.  Fork le projet.
2.  Créez votre branche de fonctionnalité (`git checkout -b feature/NouvelleFonctionnalite`).
3.  Commitez vos changements (`git commit -m 'Ajout de NouvelleFonctionnalite'`).
4.  Poussez vers la branche (`git push origin feature/NouvelleFonctionnalite`).
5.  Ouvrez une Pull Request.

## Licence

Ce projet est distribué sous la licence MIT. Voir le fichier `LICENSE` pour plus de détails.
*(N'oubliez pas d'ajouter un fichier `LICENSE` à votre dépôt. Vous pouvez facilement en créer un sur GitHub ou copier le contenu d'une licence MIT standard.)*

---

N'hésitez pas à modifier ce template pour qu'il corresponde encore mieux à votre vision du projet !
