Checklist des choses à ne pas oublier lors de l'ajout d'un nouveau service à XiVO

- Le fichier de log par défaut a les bons droits pour être écrit par le service
- Le fichier de PID et son répertoire ont les bons droits pour être écrits par le service
- Le service est ajouté à xivo-service si nécessaire
- Le service est monitoré
- Le service est bien installé sur une install fraîche
- Le service est bien démarré sur un reboot
- Le service est bien démarré sur un xivo-upgrade
- Le service est bien dans un état correct lors d'une mise à jour du slave
- Le service est bien ajouté au schéma d'architecture
- Le service n'est pas root par défaut
- Si le service doit avoir le fichier de conf par défaut de consul, il fait partie du groupe consul
- Les fichiers de config du service sont copiés par xivo-backup
- La doc de backup précise que les fichiers sont copiés