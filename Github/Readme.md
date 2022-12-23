
# Cours Github
## version 2
  

### ouvrir terminal (gitbash):
* pwd =affiche le nom de l'ordinateur et où on se situe
* cd desktop =cd pour aller au dossier desktop
* cd .. =pour revenir dossier précedent
* cd . =pour ouvrir le dossier dans vscode
* tree = afficher larborescence de dosiers
* mkdir "nom du fichier" =créer un dossier
* mkdir -p nomdudossier/nomdudossier/ = créer plein de dossiers
* rm nom du fichier = supprime fichier
* rm -r nomdudossier = supprime le dossier
* cp nomdufichier nomdunouveaufichier = copie un fichier
* mv nomdufichier nomdynouveaufichier = renome le fichier
* mv nomdufhier nomdudossier/nouveaunomdufichier = deplace et renomme un fichier
* ls =afficher ce que contient le dossier
* touch "nom du fichier" =créer un fichier
* cat nomdufichier = affiche le contenu du fichier
* cat > nomdufichier = permet decrire dans le fichier. sortir avec CTRL+C
* cat >> nomdufichier = permet de rajouter du texte dans le fichier a artir du terminal.ctrl+c
* head -n 4 nomdufichier = affiche les 4premieres lignes du fichiers
* head -n -16 nom du fichier = affiche le fichier sauf les 16 dernieres lignes
* tail -n 4 nomdufichier = affiche les 4 dernieres lignes
* tail -n +18 nomdufichier = affiche a partir de la ligne 18
* tail -f nomdufichier = affiche les evenements du system de maniere instantanées
* find -name "nomdufichier" = cherche et affiche emplacement du dossier
* find /usr/share/ -name "leo.vim" = cherche dans le dossier share
* find -name "studio*" = cherche tous les fichiers contenant studio
* grep -i Bon nomdufichier = cherche le mot bon dans le fichier, le -i ignore la majuscule
* grep -r 20 /maison = rechercher toutes les lignes de tous les fichiers 20 dans le dossier maison
* which find = ou se situe la commande find et affiche lemplacement
* whereis find = affiche emplacement et retourne la liste des fichiers en lien avec la commande
  
  ### RESEAU
* ip addr = affiche les interfaces reseaux et infos
* ip route = routes dispo a la machine pour sadresser hors de son reseau
* ping -5 adresse ip ou nomdelamachine= test connectivité entre la notre 5 machines distante
* dig linuxtricks.fr = affiche entree dns pour serveur specifique
* wget https..cluster.linuxtricks.fr = Dl page d'un site
* wget -r https...= dl page d'acceuil et tous les elements de ladresse
* curl https..cluster.linuxtricks.fr = affiche contenu du site
* curl -o nouveaunomdfichier adress ip/nomdufichier = recuperer element de la page tous en le renommant
* ssh = connecter a une machine distante. sortir avec exit
  
  ### PROCESSUS
* ps = liste les processus actif dans session en cours
* ps aux =afficher processus auxiliaire et infos
* ps aux | grep galculator = affiche les infos concernant lutilisation du processus galculator
* pidof galculator = affiche le numero des instances, quand a ete lancé la calculette
* kill numerodeprocesseur = arrete le processus
* kill 21333 213300 213333 = kill tous les processus portant le numero..
* killall nomduprogramme = tue tous le sprocessus dont le nom est nomduprogramme
  
  ### SYSTEM
* date = date
* uptime = depuis cb de tps le system est operationnel et infos id
* w = affiche les utilisateurs connectés
* more /proc/cpuinfo = infos systeme de lordi
* more /proc/meminfo = infos relatives a la memoire
* free = sous forme de tableau la conso memoire du system
* df -h = affiche lutilisation de system de fichiers (-h = plus lisible)
* du -sh nomdu dossier = affiche la taille du dossier
 
 ### ARCHIVAGE avec tar
* tar -cf archive1.tar nomdufichier nomdufichier = -c creer archive f indiquer nom du fichier 
* tar -cvf archive2.tar nomdufichier = archiver et afficher nomdufichier dans dossier archive2.tar
* tar -tf archive2.tar =lister contenu de l'archive
* tar -xf archive2.tar = extraire larchive dans le dossier ou on effectue la commande
* tar -czvf archive2.tar.gz = compresser larchive via gzip gz
* tar -xzvf /home/iza/tmp/archive2.tar.gz = extrait moi larchive au format gz (on rajoute le z)

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
* git chekout main =remettre version plus récent
    
### Travailler en equipe
* READ ME.md # titre ## sous titre
* git ignore fichier a creer dans le dossier pour renseigner les fichiers que l'on ne veut pas commits= /nomdufichier ou tous les fichiers dans le dossier= /*
* git blame nomdufichier =afficher le connard qui a fait ca
* git blame -L 10,20 nomduchier =afficher les lignes spécifiques
* 
#### Dépot distant
* git pull =récup MAJ sur depot distant
* 
#### Créer des branches pour na pas avoir de conflits de sauvegarde
* git branch =affiche les branches dispo, main si none
* git branch nomdelabranch =créer une branch en local
* git checkout nomdebranch =rentre dans nomdebranch pour faire des commits sur la branch
* git push --7-upstream origin nomdebranch =crééer la branch sur github(commande a rentrer sur bash dans dossier nomdebranch)

#### Pour commit son projet online
la pemiere fois:
* git remote add origin https://github.com/chrisdavidmills/mon-premier-depot.git (adresse github) 
* git add --all
* git commit -m 'ajout des fichiers au dépôt'
* git push -u origin main
* 
pour actualiser:
* git add --all
* git commit -m 'Un autre commit'
* git push




