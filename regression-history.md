- 19.15 : 1
  - wazo-agid home directory was not migrated properly
- 19.14 : 0
- 19.13 : 6 (Buster release, first public release since 18.03)
  - RabbitMQ upgrade fail
  - Provd cron /bin/bash
  - wazo-auth memory leak
  - upgrade from 18.01
  - service started with the wrong kombu version
  - wazo-amid conf.d gone
- 19.12 : 2
  - (SI) build ISO brisé par la clé de downloads changé par cloud-init
  - Call logs sur push mobile
- 19.11 : 1
  - Génération des call-logs bloqué (thread bus meurt)
- 19.10 : 0
- 19.09 : 0
- 19.08 : 0
- 19.07 : 1
  - total, filtered érronés dans chatd
- 19.06 : 2
  - manque 1 ACL pour la configuration des auth externe sur l'admin policy
  - LDAP AD: impossible de configurer le unique_field_format en binary_uuid
- 19.05 : 2
  - impossible d'utiliser *3 (ou autres options de Dial)
  - provd n'injecte pas la bonne adresse IP dans la config des téléphones après une installation fraîche
- 19.04 : 4
  - upgrade si fichier devices de provd n'existe pas (slave)
  - upgrade dird -> check version
  - migration config dird auto-générée ne fonctionne pas (events manqués)
  - wazo-chatd: changement de présence -> token object
- 19.03 : 5
  - Variables de template non présentes dans le fichier common.conf.
  - Le fichier de config pour les snom redirigent vers 127.0.0.1.
  - Impossible d'afficher les utilisateurs dans nestbox.
  - ACL de xivo-cti pour provd inccorects.
  - Impossible de supprimer une catégorie de son dans Nestbox sans erreur lorsque connecté à une instance.
- 19.02 : 1
  - Les téléphones des utilisateurs nouvellement créées ne se reconnectent pas sur le slave.
- 19.01 : 4
  - Configuration NAT avec plusieurs local_net. Impossible dans l'interface
  - Autoprov reboot tout les devices en autoprov lors d'un approvisionnement
  - Langue par défaut des devices en autoprov n'a pas de prompt
  - Aastra 6731i pas de son sur les originates et transferts ne fonctionnent pas
- 18.14 : 10  (passage à PJSIP et migration de xivo-service vers wazo-user)
  - PJSIP config dupliqué sur trunk avec même host
  - change-pass-vm token backend
  - timeout nestbox (pjsip reload multiple reads)
  - Trunk SIP same host
  - Paging SIP -> PJSIP
  - Dialplan loop detection PJSIP_HEADER
  - Dird service token
  - Doc migration ligne custom SIP -> PJSIP
  - Agent listen SIP -> PJSIP
  - Call logs xivo-ctid SIP ou PJSIP
- 18.13 : 1
  - Manque une dépendance vers python3-cherrypy3 dans ctid-ng
- 18.12 : 1
  - Fichier nova-compatibility en trop dans /etc/asterisk/cel.d
- 18.11 : 1
  - Nouvelle lignes dans le email body
- 18.10 : 2
  - Routage par compétences avec ancienne configuration
  - Change VM pass multi-tenant/sans authentification
- 18.09 : 1
  - Question sur l'ISO au configure de wazo-auth
- 18.08 : 0
- 18.07 : 1
  - Impossible d'appeler avec wazoclient/unicom
- 18.06 : 0
- 18.05 : 0
- 18.04 : 6
  - Call logs ne sont pas générés lors d'appels juste après l'upgrade
  - Réplication HA envoie des mails par cron toutes les heures
  - Switchboard: téléphones Snom ne décrochent pas lors du clic Wazo Client
  - UNFIXED: (régression connue à l'avance) xlet people et répertoires téléphoniques n'affichent pas les utilisateurs Wazo
  - UNFIXED: impossible de désactiver un utilisateur dans webi
- 18.03 : 1
  - BS filters admin UI: si l'utilisateur boss est supprimé, admin-ui affiche une erreur à la place du BS filter
- 18.02 : 0
- 18.01 : 5
  - auto answer Polycom (nouvelle version de request n'accepte pas de header mal formatté)
  - le module confbridge ne se load plus (erreur dans les sections générées)
  - indicateur du nombre de voicemail dans wazoclient ne fonctionne plus
  - la section interface dans la dwhowebi est cassée (stretch vs eth0)
  - le market de prod avec les versions avec tiret est cassé
- 17.17 : 0
- 17.16 : 1
  - La version pas bumpé du wazoclient permettait de DOSer xivo-ctid
- 17.15 : 0
- 17.14 : 1
  - Traduction du client-qt n'étaient pas disponible sur certaines resources.
- 17.13 : 1
  - Impossible de construire un paquet python debian pour plugind (il manque une dependance python-setuptools)
- 17.12 : 0
- 17.11 : 0
- 17.10 : 1
  - Impossible de supprimer un contact phonebook si on l'a importé avec un field ID.
- 17.09 : 1
  - Oublier de mettre xivo-call-logs en purge (donc certains fichiers se marchaient sur les pieds)
- 17.08 : 1
  - xivo-service status montre wazo-plugind comme "unknown"
- 17.07 : 0
- 17.06 : 1
  - Skill based routing patch mal updaté bloque Asterisk
- 17.05 : 0
- 17.04 : 0
- 17.03 : 1
  - Reverse lookup avec numéro modifiés par in_callerid
- 17.02 : 1
  - Fuite mémoire Asterisk par ari.conf:channelvars
- 17.01 : 1
  - ISO ne finit pas l'installation (BD xivo-auth)
- 16.16 : 1
  - Régression asterisk, on ne peut plus transférer après une mise en attente au switchboard
- 16.15 : 0
- 16.14 : 3
  - POST /calls = priority ne peut pas être un integer
  - monitoring agentd (mauvais PID file)
  - timeout non nécessaire sur les transferts directs
- 16.13 : 0
- 16.12 : 0
- 16.11 : 1
  - Erreur de migration BD lorsqu'il y a presence de multi users par ligne
- 16.10 : 3
  - Échec d'appel XiVO Client #25 avec Aastra
  - Échec d'association multi-user à une même ligne
  - Activation de la séparation par contexte pas pris en compte par xivo-confgend
- 16.09 : 3
  - Transfert vers la mauvaise personne (channel local listés à un user)
  - Impossible de charger le fichier api.json dans xivo-confd
  - Mauvais call logs
- 16.08 : 0
- 16.07 : 0 :D
- 16.06 : 3
  - Oublie le merge d'une branche dans xivo-upgrade
  - Impossible de mettre une majuscule pour le nom d'une ligne custom
  - XiVO confd n'est pas démarré sur un install ISO (donc impossible d'acceder au wizard)
- 16.05 : 1
  - xivo-agid n'a pas le bon acl pour faire un reset autoprov
- 16.04 : 1
  - Timeout dans la webi pour afficher "utilisateurs(exten@context)" dans paging (et autres)
- 16.03 : 1
  - *guest est cassé
- 16.02 : 1
  - Connexion au xivoclient chiffré fail si les certificats n'ont pas été copiés sur le slave.
- 16.01 : 4
  - MWI ne s'affiche pas
  - xivo-auth-keys desync avec HA
  - monit ne démarre pas sur le slave
  - xivo-confd ne démarre pas sur le slave
- 15.20 (jessie) : 4
  - Mise à jour des status
  - restart/stop consul
  - core dump asterisk /var/lib/asterisk
  - migration des /etc/default
  - arrêt des service avec sigkill (systemD)
- 15.19 : 3
  - L’icône mute dans les chambres de conférences n'est plus fonctionnelle
  - Impossible d'empêcher les renvois via la webi (l'option n'est plus appliqué au xivoclient)
  - xivo-ctid perd son token lors d'un update de config
- 15.18 : 1
  - le compteur "état depuis" recommence à 0 lors du wrapuptime (non systématique)(bug 5912)
- 15.17 : 2
  - Impossible de se connecter au serveur CTI
  - Impossible d'appeler un utilisateur
- 15.16 : 1
  - Monit ne redémarre plus
- 15.15 : 2
  - Recherche Switchboard incomplète
  - Le menu du systray sous Ubuntu ne fonctionne plus (X-514)
- 15.14 : 2
  - Xlet queue members ne se rafraichit pas en real-time
  - Impossible d'éditer un contact personnel si importé avec colonne non-XiVO
- 15.13 : 6 (Asterisk 13)
  - BLF sur chambre de conférence
  - Bug affichage webi sur les touches de fonctions non-supervisable
  - Impossible d'appeler une 2eime colonne number (People Xlet)
  - Interception dans XiVO Client
  - Annuler transfert direct
  - Switchboard décroché physique téléphone et faire un transfert
- 15.12 : 1
  - Le check monit de xivo-auth ne fonctionne pas.
- 15.11 : 2
  - Impossible de charger les modules DAHDI (X-451).
  - Problème lors du redémarrage de XiVO-auth (constaté lors des tests de HA).
- 15.10 : 2
  - Display des inputs dans la xlet fax sur MacOS
  - Aucun icon mute dans la xlet conférence (X-106)
- 15.09 : 4
  - Border colonne description xlet people
  - Impossible d'inviter dans une chambre de conférence (xlet contacts)
  - Sysconfd erreur HA
  - Synchronize SCCP phones (X-595)
- 15.08 : 5
  - Visuel de la Xlet People
  - Tri par défaut de la Xlet Historique
  - Couleur du systray pour un agent en pause
  - Effacer un device en autoprov
  - Impossible de rechercher par Vendeur dans l'interface web
- 15.07 : 0
- 15.06 : 1
  - arrondis sur inputs dans fenêtre du login du XiVO Client
- 15.05 : 0
- 15.04 : 0
- 15.03 : 1
  - click to call avec uri tel: sur mac (suite a la migration de mac osx)
- 15.02 : 4
  - chat
  - style
  - historique
  - svg
- 15.01 : 2
  - change vm password
  - call\_from\_result
- 14.24 : 2
  - connexion d'un client CTI chiffré
  - touche de fonction park position
- 14.23 : 0 =D
- 14.22 : 2
  - suppression d'un user
  - CTI + AMI proxy = bloque le démarrage du CTI
- 14.21 : 3
  - confd init
  - aastra phonebook ssl
  - click to call activate
- 14.20 : 0 d:-p
- 14.19 : 3
  - touches de fonction supprimé
  - touches de fonction SCCP custom
  - click-to-call \#25
- 14.18 : 0
- 14.17 : 1
  - check monit sur xivo-amid
- 14.16 : 1
  - daemonize : double xivo-stat == stacktrace
- 14.15 : 1
  - Script migration user fk destination failed xivo-upgrade -d.
- 14.14 : 0
- 14.13 : 2
  - Touches de fonctions disparues
  - Devices SCCP désassociés invisibles dans la liste des devices
- 14.12 : 0 :D
- 14.11 : 0
- 14.10 : 2
  - Voicemail : pas de pagination dans la webi
  - Voicemail : pas de recherche dans la webi
- 14.09 : 2
  - Création des filtres Patrons-Secrétaires
  - Affichage des statistiques
- 14.08 : 2
  - Initialisation de la BD à l'installation ISO
  - XiVO Client activé sans profil pour les users créés par REST API
  - Bonus : Régression introduite en 14.05 : callerID lors de transfert indirect du switchboard (\#5049)
- 14.07 : 4
  - Switchboard ne peut pas raccrocher les appels DAHDI
  - Switchboard ne peut pas raccrocher les appels IAX
  - Réplication HA échoue à cause de la migration table entités de BD Asterisk -\> XiVO
  - Création d'un admin dans la webi
- 14.06 : 5
  - xlet Switchboard sélection des appels invisible (Qt5)
  - xlet Historique : menu contextuel ne s'affiche pas (Qt5)
  - xlets Queues : compteurs de temps ne s'affichent pas (Qt5)
  - click2call n'affiche pas le client (Qt5)
  - Switchboard ne peut pas décrocher les appels DAHDI
- 14.05 : 0 :D
- 14.04 : 1
  - Provisionning : autoprov code n'associait pas la mac du device à la ligne dans la webi
- 14.03 : 3
  - Historique CTI après reverse lookup
  - Touche Fonction BS Filter
  - User migrés sans touche de fonction
- 14.02 : 2
  - XiVO Client - Separation par contexte
  - XiVO Client - Menu de langue
- 14.01 : 3
  - musiques d'attente (migration bd pf-xivo)
  - certificats (migration bd pf-xivo)
  - installation iso - paquets non-configurés à l'installation (migration pf-xivo)
- 13.25 : 0 :D
- 13.24 : 1 ( Génération call logs )
- 13.23 : 2
  - Remonté de fiche standard ne remonte plus
  - Images dans la remonté de fiche (2 bugs - antérieur à 13.23, ne savons pas depuis quand)
- 13.22 : 2
  - xivo-service restart all ne redémarre pas PG
  - Trunks IAX ne fonctionnent plus
- 13.21 : 1
  - X-592 Effacer device associé à un user
- 13.20 : 2
  - X-8 666 match 6666
  - sccp early RTP 7912, 7940
- 13.19 : 0 :D
- 13.18 : 11 (non publiée)
  - Code de provisioning
  - Recherche de devices via webi
  - Effacer la ligne d'un user
  - Pagination de la liste des devices
  - Tri de la liste des devices
  - X-39 Effacer un user avec une ligne et un device
  - Pagination de la recherche de devices
  - Revenir en autoprov
  - Code de provisioning avec touche de fonction
  - Éditer un utilisateur sans rien changer
  - X-29 Journaux d'appel originate
  - Synchronisation des postes SCCP
- 13.17 : 0 :P
- 13.16 : 0 :)
- 13.15 : 7 (non publiée)
  - Édition ligne via user
  - Suppression dial pattern outcall (publiée en 13.14, cf. \#4592)
  - X-47 et X-48 Interception users/groups
  - X-579 DirectMedia On Hold (unresolved)
  - X-327 Edit SIP Username
  - Provisioning code
  - X-534/X-324 : Lignes custom

- post 13.14 : 2
  - X-173 Xlet History avec ligne SCCP

- 13.14 : 4
  - Confgend (colonne internal)
  - X-32 : Perso. du caller ID sur appel sortant
  - X-49:Transfert direct par touche de fonction
  - Reload dialplan après modification extensions

- 13.13 : 3 (même cause)
  - Impossible de passer un appel interne
  - X-542 : infos de renvois d'appel
  - X-404 : accès voicemail via trunk

- 13.12 : 1
  - Cacher/Décacher le XiVO Client (X-518, X-520)

- 13.11 : 1
  - Impossible de passer un appel après activation puis désactivation de la HA

- 13.10 : 4
  - Serveur CTI ne démarre plus si un statut de présence CTI a été supprimé (\#4419)
  - X-13 : Appel entrant vers utilisateur ne fonctionne pas
  - X-159 : Tooltip d'agent mal mis à jour (présent aussi en 13.09)
  - X-493 : Segfault xivoclient lors édition d'un groupe

- post 13.09 : 2
  - Bug \#4401: number cleanup when calling from the xivo client no longer works in Xivo 13.09
  - Bug \#4395: xivo-upgrade -d launches the normal upgrade process instead of only downloading the packets

- 13.09 : 1
  - X-191 : Déloguer l'agent à la fermeture/déconnexion du XiVOClient

- 13.08 : 1
  - X-331 : Ouverture URL - Erreur dans le ctid dp-mysheeturl

- 13.07 : 1
  - X-482 Manipulation de campagnes vides

- 13.06 : 1
  - X-196 Listen d'un agent par un superviseur sans agent associé fait planter le XiVO Client.

- 13.05 : 1
  - X-482 Manipulation de campagnes vides

- 13.04 : 17
  - X-32, X-331 X-163, X-244, X-481, X-233, X-115, X-97, BS Filter, X-156, X-119, X-175, X-179, X-180, X-250, X-183, X-482