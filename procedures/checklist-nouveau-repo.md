- Créer le repo sur Github
- Ajouter le hook Github: Jenkins Git vers <http://jenkins.xivo.io>

OU

- Rouler le script xivo-tools/dev-tools/new-repo

PUIS

- Ajouter le repo dans xivo-build-tools/etc/packages
- Ajouter le repo dans xivo-tools/dev-tools/repos si ce n'est pas un repo \*-packaging
- Ajouter le job sur Jenkins
- Ajouter le repo sur travis (?)