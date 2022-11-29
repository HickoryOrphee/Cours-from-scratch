
# Cours Github
## version 2
new version pour voir la version 2 hihi  

### ouvrir terminal (gitbash):
* pwd =affiche le nom de l'ordinateur et où on se situe
* cd desktop =cd pour aller au dossier desktop
* cd .. =pour revenir dossier précedent
* cd . =pour ouvrir le dossier dans vscode
* mkdir "nom du fichier" =créer un dossier
* ls =afficher ce que contient le dossier
* touch "nom du fichier" =créer un fichier

### Versionner en local
* git init =initialise le depot
* git add. =ajoute toutes les modifs
* git status =pour afficher le statut des fichiers
* git commit -m"explications" =créer le nouveau commit, point de sauvegarde
* git push u- originin main =appliquer les changements sur github.com  
* git log =list des commits
* git log -n2 =affiche les 2 derniers commits
* git show sha-1 =voir commit(sha-1) spécifique (clic molette souris pour coller)
* git checkout sha-1 =revenir version du sha-1
* git chekout main =remettre version plus récente
   
### Versionner sur Github, premier envoi internet
* aller sur github.com et create new repository
* copier ladresse https
    
### Travailler en equipe
* READ ME.md # titre ## sous titre
* git ignore fichier a creer dans le dossier pour renseigner les fichiers que l'on ne veut pas commits= /nomdufichier ou tous les fichiers dans le dossier= /*
* git blame nomdufichier =afficher le connard qui a fait ca
* git blame -L 10,20 nomduchier =afficher les lignes spécifiques
#### Dépot distant
* git pull =récup MAJ sur depot distant
#### Créer des branches pour na pas avoir de conflits de sauvegarde
* git branch =affiche les branches dispo, main si none
* git branch nomdelabranch =créer une branch en local
* git checkout nomdebranch =rentre dans nomdebranch pour faire des commits sur la branch
* git push --7-upstream origin nomdebranch =crééer la branch sur github(commande a rentrer sur bash dans dossier nomdebranch)
#### Pour commit son projet online
* git add . 
* git commit -n "nom des modifications effectcuées" pour communiquer avé lé cop1
* git push -u origin main =

