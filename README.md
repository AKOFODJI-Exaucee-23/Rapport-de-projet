# Fichier reademe.md

# IFRI_MentorLink
Ce projet est une application web d'interconnexion conçue pour mettre
en relation les étudiants de l'IFRI souhaitant bénéficier ou offrir du
mentorat qu'il soit académique ou professionnel.
# Description du projet
   IFRI_MentorLink permet à chaque utilisateur de créer un compte, autrement 
   dit un profil personnalisé afin de publier ou de rechercher des offres ou
   des demandes de mentorat. Elle vise à faciliter le partage de compétences 
   entre individus au seins des différentes filières de l'IFRI.

# Architecture et modules clés
    L'application repose sur une architecture client-serveur et s'articule autour
de trois (03) modules fondamentaux:
    1. La gestion des comptes et profils utilisateurs: Chaque utilisateur (étudiant
     comme mentor), crée un profil détaillé qui renseigne son nom, sa photo de profil,
     ses compétences spécifiques, ses disponibilités horaire, sa filière d'origine 
     ainsi que son score de compatibilité.
    2. L'algorithme de matching: Analyse les profils pour proposer de manières 
    intelligentes les combinaisons mentor-mentoré les plus pertinentes. Ce calcul
    se base sur trois critères majeurs:
       -La compatibilité des compétences recherchées ou offertes,
       -La proximité des filières et niveaux d'études,
       -La correspondance d'agenda et de disponibilités horaire.
    3. La messagerie instantanée intégrée: Un espace de discussion interne permet 
    aux binomes de s'organiser, de planifier et de suivre efficacement le déroulement 
    de leurs sessions de mentorat. Les utilisateurs doivent recevoir des notifications
    en temps réel lors de la réception de nouveaux messages.
 
# Filières académique
  La plateforme partage les compétences et optimise le matching selon les cinq (05) 
  filières de l'IFRI:
      .IA: Intelligence Artificielle
      .IM: Internet des objets et Multimédia
      .GL: Génie Logistique
      .SE&IoT: Système Emmbarqués et Internet des Objets
      .SI: Sécurité Informatique

# Installation locale
Pour lancer le projet sur votre machine de développement il faut:
   1. Cloner le projet
       bash
       git clone https://github.com
       cd ifri-mentorlink
   2. Créer et activer l'environnement visuel
       bash
      # Sous Linux/macOS
       python 3 -m venv venv
       source venv/bin/activate
      # Sous Windows
        python -m venv venv
        venv\Scripts\activate
   3. Installer les dépendances
        bash
        pip install -r requirements.txt
   4. Appliquer les migrations de la base de données
        bash
        python manage.py migrate
   5. Lancer le serveur de développement
        bash
        python manage.py runserver

# Technologies utilisées
    *Frontend: html, css, JavaScript
    *Base de donnés: PostgresSQL pour la production
    *Backend: Python, Django.

# Roles des utilisateurs
   1. Mentoré (étudiant): Renseigne sa filière, recherche une compétence
    et utilise la messagerie pour planifier ses cours.
   2. Mentor: Configure son profil avec ses expertises, ses horaires
   disponibles et prend en charge des étudiants.
   3. Administrateur: Supervise la plateforme, valide les comptes et assure 
   la modération des échanges.

