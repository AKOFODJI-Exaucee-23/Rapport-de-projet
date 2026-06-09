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
 
