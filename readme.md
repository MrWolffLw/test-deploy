# Rapport de déploiement - [PELISSON Cédric]

## Liens

- **Application en ligne :** (<https://test-deploy-pelisson.osc-fr1.scalingo.io/>)

- **Dépôt de code :** https://github.com/MrWolffLw/test-deploy

## Prérequis techniques

#### -PHP 8.4+ avec l'extension pdo_msql
#### -Composer installé
#### -Un compte Scalingo

## Fichier de configuration CI

#### Le fichier de configuration de l'intégration continue se trouve dans : .github/workflows/ci.yaml

## Procédure de déploiement pas à pas

A. Initialisation sur Scalingo
1. Créer l'application


1. APP_ENV = prod
2. APP_SECRET = (par exemple copier la valeur de :
echo bin2hex(random
_
bytes(16)) )
C. Préparation du code
1. Commit des changement git commit -m "Mise à jour effectuée"
D. Mise en ligne
2. Push des commits : git push