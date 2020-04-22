<<<<<<< HEAD
---
layout: post
title:  "Systèmes D'Exploitation"
date:   2020-03-31 00:42:02 +0200
categories: jekyll update
---
=======
>>>>>>> 0adc13d8db16224162c64a87083b7be1d0ea9a92

# Systèmes d'exploitation, TP: Les différences entre Windows et Linux

## Partie 1 : Windows

Ici, nous reverrons les gestes basiques de « tout développeur » sur Windows.

### Exercice 1 : Gestion de fichiers et de dossiers

1. Naviguer à travers des dossiers : Dans ce premier exercice, le travail sera effectué dans un espace personnel (en l’occurrence ici, le vôtre chez Saint-Charles

* Dans la barre des tâches (généralement barre en bas de l’écran) on clique sur l’icône de l’Explorateur Windows, l’icône de dossier.
  > (Avancé : On peut aussi utiliser le raccourci Win+E, Win étant le logo Windows sur le clavier)

![Barre des tâches](Assets/taskbar.PNG)

* Une fois la fenêtre ouverte, dans le menu de gauche on clique sur « Ce PC » - alternativement en fonction de la version de Windows et de la configuration, l’icône est trouvable sur le bureau ou dans le menu démarrer (le menu qui apparaît quand on appuie sur le logo Windows en bas à gauche).

![Illustration 1](https://cubicface.github.io/nsi/cours/cours_se/Assets/WinExplorer1.PNG)

* La fenêtre change et on clique sur le disque assigné à son nom.

![Illustration 2](https://cubicface.github.io/nsi/cours/cours_se/Assets/WinExplorer2.PNG)

* On arrive sur une page à peu près similaire à celle-ci (le contenu diffère en fonction de ce que la personne possédant la session a fait sur cet espace lors des années précédentes dans l’établissement).

![Illustration 3](https://cubicface.github.io/nsi/cours/cours_se/Assets/WinExplorer3.PNG)

2. Créer un dossier « NSI »

* On fait un clic sur le bouton droit de la souris (aussi dit « clic droit ») et dans le menu qui suite on passe la souris sur « Nouveau » et dans le nouveau menu qui apparaît on clique sur « Dossier ».
  > (Avancé : on peut aussi utiliser le raccourci Ctrl+Maj+N)

![Illustration 4](https://cubicface.github.io/nsi/cours/cours_se/Assets/WinExplorer4.PNG)

* Après création, il nous propose déjà de le renommer, donc on le renomme en « NSI » et on appuie sur entrée pour confirmer.

![Illustration 5](https://cubicface.github.io/nsi/cours/cours_se/Assets/WinExplorer5.F.PNG)

* Si on a fait une erreur en renommant le fichier, on peut toujours le renommer en cliquant sur le fichier puis cliquer droit sur le dossier pour afficher un menu similaire à tout à l’heure et cliquer sur renommer.
  > (Avancé : on peut aussi utiliser le bouton F2 sur le clavier pour renommer)

![Illustration 6](https://cubicface.github.io/nsi/cours/cours_se/Assets/WinExplorer6.PNG)

3. Créer un sous-dossier

* Pour créer un sous-dossier, ce sont exactement les mêmes étapes que précédemment, sauf que l’on crée le dossier dans le dossier qu’on a créé. Pour se faire, on double-clique sur le dossier afin d’afficher son contenu (ici vide).
* Créez les sous-dossiers « Cours », « Projet » et « Test ».

4. Supprimer un dossier

* Pour supprimer un dossier, il faut sélectionner et cliquer droit sur le dossier, et cliquer sur « Supprimer » dans le menu.
  > Remarque : toutes ses manipulations de gestion sont identiques pour tout type de fichier.
  >
  > (Avancé : On peut utiliser les raccourcis suivants pour aller plus vite :
  > - Ctrl+Maj+N : Créer un dossier
  > - F2 : Renommer un fichier
  > - Suppr./Del. : Supprimer un fichier)

<p
align="center">
  <img
  src="Assets/WinExplorer7.png">
</p>

---

### Exercice 2: Création d'un fichier: Document texte

Sur Windows on peut créer différents fichiers. Ici nous allons créer un fichier texte.

* Pour se faire, il faut cliquer droit sur un endroit vide, et passer sa souris sur Nouveau.
* Ensuite il faut choisir le type de fichier, ici on veut un document texte, donc on clique sur "Document Texte".
* Comme d'habitude on peut renommer le fichier lors de sa création.

> *Remarque: Pour certains types de fichiers, la création doit se faire directement via le logiciel qui lui correspond.*

<p
align="center">
  <img
  src="Assets/WinExplorer8.png">
</p>

---

### Exercice 3: Modifier un fichier

* Pour modifier le fichier texte que l'on vient de créer, il faut double cliquer sur celui-ci.
  > Une fenêtre blanche s'ouvre dans laquelle on peut écrire.
  > * Essayez d'écrire "J'aime la NSI".
* Enfin, il faut sauvegarder le fiichier. Cliquer en haut à gauche sur "Fichier".
* Et cliquer sur "Sauvegarder" (ou "Enregistrer").
  > (Avancé: utilisez le raccourci Ctrl+S)

<p
align="center">
  <img
  src="Assets/WinExplorer9.png">
</p>

---

## Partie 2: Linux

Avant de commencer, une petite leçon sur les commandes Linux.

Une commande est composé de son nom et __d'attributs__.

Le nom de la commande permet de pouvoir éxecuter la commande en tant que tel, ou, dans certains cas, elle permet de donner la version d'un programme.

Un __attribut__ permet de spécifier comment la commande va agir. Les attributs sont __sensibles à la casse__, une faute de majuscule peut totalement détourner la commande.

Si vous en avez les autorisations nécessaires sur votre session, vous pouvez élever l'éxecution d'une commande à celle "d'Administrateur" ou plus communément appelée __le root__ (la racine), il faut inclure `sudo` avant la ligne de commande (séparé d'un espace). Cela sera utile pour certaines actions si par exemple si un fichier ou dossier est protégé.

Il vous faudra ensuite tapper le mot de passe de votre session. (les lettres seront cachées)

Généralement, soit vous la définissez à l'installation, soit le propriétaire vous le donne, mais il est __impératif__ de ne __JAMAIS__ confier ce mot de passe à qui que ce soit, puisque l'accès __root__ permet d'avoir accès à des fichiers du système.

Une commande Linux peut ressember à ceci:

```bash
ls -a -U --author
```

Ou à ceci pour une exécution avec `sudo`:

```bash
sudo apt-get install npm
```

Lorsque vous vous connecterez sur votre machine, la console pourrait afficher d'autres éléments au démarrage, mais le plus important est que vous voyez le nom de votre session le nom de votre machine sous ce format (ou similaire selon la distribution):

```console
nom@machine:~$
```

C'est à partir de là que vous pourrez entrer des commandes, si cela ne s'affiche pas, c'est qu'un autre programme est en cours d'exécution et qu'il faut attendre que le programme finisse de s'exécuter avant d'entrer une autre commande.

Le signe `~` indique que vous êtes dans votre espace personnel. Ce signe va changer lorsque vous naviguerez à travers les dossiers.

### Exercice 1: Gérer la console et naviguation

Dans cet exercice, nous allons apprendre gérer l'utilisation de la console et de la naviguation à travers les fichiers sur Linux.

#### 1. Afficher le version Linux

Si vous souhaitez utiliser une machine tournant Linux mais qui n'est pas la vôtre, il est important de savoir sur quelle version et sur quelle distribution vous êtes, puisqu'il peut y avoir des différences entre les distributions.

Pour afficher juste le nom du kernel (ici Linux) on tape:

```bash
uname
```

```console
gradient@Gradient-PC:~$ uname
Linux
```

Sinon différents attributs son disponibles afin de pouvoir afficher des données supplémentaires:

```console
  -a, --all                affiche toutes les informations, dans l'ordre qui suit
                             excepté lors de l'utilisation de -p et -i si inconnu:
  -s, --kernel-name        affiche le nom du kernel (par défaut)
  -n, --nodename           affiche le nom de l'hôte
  -r, --kernel-release     affiche la version du kernel (release)
  -v, --kernel-version     affiche la version du kernel (version)
  -m, --machine            affiche le nom de la machine
  -p, --processor          affiche le type de processeur (non-portable)
  -i, --hardware-platform  affiche l'architecture (non-portable)
  -o, --operating-system   affiche le système d'exploitation
      --help     affiche cette aide et quitte
      --version  retourne l'information de la version de la commande et quitte
```

Exemple:

```console
gradient@GRADIENT-PC-vbox:~$ uname -a
Linux GRADIENT-PC-vbox 5.3.0-42-generic #34~18.04.1-Ubuntu SMP Fri Feb 28 13:42:26 UTC 2020 x86_64 x86_64 x86_64 GNU/Linux
```

> Tout au long de cette partie, nous nous baserons sur la distribution Linux: [Ubuntu](https://ubuntu.com/), c'est la distribution la plus facile à approcher pour des débutants en Linux.
>
> Nous n'aborderons cependant pas l'installation d'Ubuntu ou de toute autre distribution Linux. Vous pouvez faire des recherches si vous le voulez, l'installation peut paraître compliquée et dangereuse, mais au fur et à mesure on s'y fait!

#### 2. Changer de dossier

Pour se diriger vers un dossier, il suffit d'utiliser la commande:

```bash
cd <nom du dossier>
```

Exemple:

```console
gradient@Gradient-PC:~$ cd Dossier
gradient@Gradient-PC:~/Dossier$
```

> On remarque ainsi que le signe `~` se transforme en `~/<nom du dossier>`, ainsi entre le `:` et le `$`, cela indique dans quel dossier on se trouve.

Pour revenir au dossier précédent, il suffit remplacer le nom du dossier par `..`:

```console
gradient@Gradient-PC:~/Dossier$ cd ..
gradient@Gradient-PC:~$
```

Pour on peut ainsi se déplacer de dossier en dossier:

```console
gradient@Gradient-PC:~$ cd Dossier
gradient@Gradient-PC:~/Dossier$ cd Sous-Dossier
gradient@Gradient-PC:~/Dossier/Sous-Dossier$ cd ..
gradient@Gradient-PC:~/Dossier$
```

> Il est possible aussi de mentionner des chemins d'accès:
>
> ```console
> gradient@Gradient-PC:~$ cd Dossier/Sous-Dossier
> gradient@Gradient-PC:~/Dossier/Sous-Dossier$ cd ..
> gradient@Gradient-PC:~/Dossier$
> ```
>

Pour revenir directement à l'espace personnel (`~`), il faut juste entrer:

```bash
cd
```

#### 3. Lister la liste des fichiers et des dossiers

En règle générale on utilise la commande suivante pour lister les fichiers et les dossiers:

```bash
ls
```

ou

```bash
l
```

Mais il existe des attributs afin de changer l'affichage en fonction de nos besoins:

```console
  -a, --all                  n'ignore pas les dossiers commençant par .
  -A, --almost-all           ne pas lister implicitement les dossiers . et ..
      --author               avec -l, affiche l'auteur de chaque fichier
  -B, --ignore-backups       ne liste pas les entrées finisssant par ~
  -c                         avec -lt: trie par, et montre le, ctime (heure de la dernière
                               modification du fichier);
                               avec -l: montre le ctime et trie par nom;
                               sinon: trie par ctime, les plus récents en premier
  -C                         liste les entrées par colonne
  -f                         do not sort, enable -aU, disable -ls --color
  -g                         comme -l, mais ne liste pas le propriétaire
  -h, --human-readable       avec -l et/ou -s, affiche les tailles en unités communes
                               (ex: 1K 234M 2G)
      --si                   pareil, mais utilise des puissances de 1000 et non de 1024
  -l                         utilise un long format de listage
  -m                         remplit les espaces avec une séparation avec des virgyles à chaque liste d'entrée
  -n, --numeric-uid-gid      comme -l, mais liste les utilisateurs numériques et les ID de Groupes
  -N, --literal              affiche le nom des entrées sans citer
  -o                         comme -l, mais ne liste pas les informations de groupe
  -r, --reverse              inverser l'ordre lors du triage
  -R, --recursive            liste les sous-dossiers recursivement
  -s, --size                 affiche la taille allouée à chaque fichier, en blocks
  -S                         trier par taille de fichier, les plus larges en premier
  -t                         trier par la date et l'heure de modification, les plus récents en premier
  -u                         avec -lt: trie par, et affiche, la date d'accès;
                               avec -l: affiche la date d'accès et trie par le nom;
                               sinon: trie par la date d'accès, les plus récents en premier
  -U                         do not sort; list entries in directory order
  -x                         liste les entrée par ligne au lieu des colonnes
  -1                         liste un fichier par ligne.  Évitez '\n' avec -q ou -b
      --help     affiche cette aide et quitte
      --version  retourne la version de la commande et quitte
```

Voici des exemples d'utilisation:

```console
gradient@GRADIENT-PC-vbox:~$ ls -1
Desktop
Documents
Downloads
examples.desktop
Music
Pictures
Public
snap
Templates
Videos
gradient@GRADIENT-PC-vbox:~$ ls -1R
.:
Desktop
Documents
Downloads
examples.desktop
Music
Pictures
Public
snap
Templates
Videos

./Desktop:
ne_pas_oublier.txt

./Documents:
Devoirs
fiche_de_paye.txt

./Documents/Devoirs:
cours.txt
exercices.txt

./Downloads:
170649-darwin.tar.gz
darwin

./Downloads/darwin:
animation.png
background.png
box.png
bullet.png
darwin.plymouth
darwin.script
entry.png
lock.png
logo.png
motif.png
progress_bar.png
progress_box_background.png
progress_box_edge.png
progress_box.png
suspend.png

./Music:

./Pictures:

./Public:

./snap:
canonical-livepatch
discord

./snap/canonical-livepatch:
94
95
common
current

./snap/canonical-livepatch/94:

./snap/canonical-livepatch/95:

./snap/canonical-livepatch/common:

./snap/discord:
109
common
current

./snap/discord/109:

./snap/discord/common:

./Templates:

./Videos:
gradient@GRADIENT-PC-vbox:~$
```

#### 4. Une commande qui repose les yeux: nettoyer la console

Si vous en avez marre de voir des lettres partout, vous pouvez juste tout effacer grâce à la commande:

```bash
clear
```

Exemple (c'est animé!):

<p
align="center">
  <img
  size="100%"
  src="Assets/wslExample.gif">
</p>

---

### Exercice 2: Création d'un dossier

Pour créer un dossier, il faut taper la commande:

```bash
mkdir <nom du premier dossier> <nom du deuxième dossier> ... <nom du nème dossier>
```

> *Anecdote: `mkdir` c'est l'acronyme de "Make Directory"*

Ainsi on peut créer autant de dossier qu'on veut (valable pour les sous-dossiers).

Exemple:

```console
gradient@Gradient-PC:~$ mkdir Dossier
gradient@Gradient-PC:~$ mkdir Dossier2
gradient@Gradient-PC:~$ ls -1
Dossier
Dossier2
bin
gradient@Gradient-PC:~$ mkdir Dossier3 Dossier4
gradient@Gradient-PC:~$ ls -1
Dossier
Dossier2
Dossier3
Dossier4
bin
gradient@Gradient-PC:~$ cd Dossier
gradient@Gradient-PC:~/Dossier$ mkdir Sous-Dossier1 Sous-Dossier2
gradient@Gradient-PC:~/Dossier$ ls -1
Sous-Dossier1
Sous-Dossier2
gradient@Gradient-PC:~/Dossier$ cd ..
gradient@Gradient-PC:~$ ls -1R
.:
Dossier
Dossier2
Dossier3
Dossier4
bin

./Dossier:
Sous-Dossier1
Sous-Dossier2

./Dossier/Sous-Dossier1:

./Dossier/Sous-Dossier2:

./Dossier2:

./Dossier3:

./Dossier4:
gradient@Gradient-PC:~$
```

---

### Exercice 3: Création et modification d'un fichier

Pour créer un fichier, il existe deux méthodes:

* Une première méthode pour créer seulement le fichier
* Une deuxième méthode pour créer ET modifier un fichier

#### 1. Créer un fichier (méthode 1)

Pour créer un ou plusieurs fichiers sans les modifier, il suffit d'entrer la commande:

```bash
touch <nom et extension du premier fichier> <nom et extension du deuxième fichier> ... <nom et extension du nième fichier>
```

Exemple:

```console
gradient@Gradient-PC:~$ ls
Dossier  Dossier2  Dossier3  Dossier4  bin
gradient@Gradient-PC:~$ touch fichier.txt
gradient@Gradient-PC:~$ ls
Dossier  Dossier2  Dossier3  Dossier4  bin  fichier.txt
gradient@Gradient-PC:~$
```

> Il est possible d'indiquer un chemin d'accès:
>
> ```console
> gradient@Gradient-PC:~$ touch fichier2.txt Dossier/fichier.txt
> gradient@Gradient-PC:~$ ls -1R
> .:
> Dossier
> Dossier2
> Dossier3
> Dossier4
> bin
> fichier.txt
> fichier2.txt
>
> ./Dossier:
> Sous-Dossier1
> Sous-Dossier2
> fichier.txt
>
> ./Dossier/Sous-Dossier1:
>
> ./Dossier/Sous-Dossier2:
>
> ./Dossier2:
>
> ./Dossier3:
>
> ./Dossier4:
> gradient@Gradient-PC:~$
> ```
>
> *Remarquez aussi qu'on doit toujours indiquer l'extension de fichier*

#### 2. Créer et/ou modifier un fichier (méthode 2)

Pour créer et ou modifier un fichier, on peut utiliser un éditeur sur console. Ici on va utiliser __Nano__ qui est intégré à Ubuntu:

```bash
nano <nom du fichier>
```

> *Notez qu'on ne peut créer qu'un seul fichier lorsque l'on utilise un éditeur.*

```console
gradient@Gradient-PC:~$ nano fichier.txt
```

```console
  GNU nano 2.9.3                                       fichier.txt

|


















^G Get Help     ^O Write Out    ^W Where Is     ^K Cut Text     ^J Justify      ^C Cur Pos      M-U Undo
^X Exit         ^R Read File    ^\ Replace      ^U Uncut Text   ^T To Spell     ^_ Go To Line   M-E Redo
```

> J'utilise une version anglaise car c'est ce qui est installé sur ma machine, vos versions peuvent être différentes.

<<<<<<< HEAD
On peut remarque que l'interface nous donne quelques indications sur quelques raccoucis à utiliser pour effectuer certaines actions.

Le symbole `^` indique la touche `[Ctrl]` de votre clavier.

Ici on ne va s'intéresser qu'à deux de ces actions.
> Libre à vous d'explorer les autres fonctions!

* Le raccourci `^O` (plus ergonomiquement `Ctrl+O`) permet d'enregistrer ce que vous avez fait.
* Le raccourci `^X` (`Ctrl+X`) permet de fermer le fichier (et accessoirement d'enregistrer celui-ci, si cela ne l'avait pas déjà été fait).

Lorsque l'on enregistre avec `Ctrl+O`, le programme nous demande de confirmer le nom du fichier:

```console
  GNU nano 2.9.3                                   fichier.txt                                    Modified

Texte à insérer.
























File Name to Write: fichier.txt
^G Get Help                M-D DOS Format             M-A Append                 M-B Backup File
^C Cancel                  M-M Mac Format             M-P Prepend                ^T To Files
```

Si on veut annuler l'action, on à juste à faire `^C` (`Ctrl+C`).
> On peut remarquer que dès que vous avez commencé à insérer des choses, un petit label `Modifié` est apparu en haut à droite.

Une fois qu'on a enregistré, on peut remarquer qu'un label affiche le nombre de lignes écrites:

```console
  GNU nano 2.9.3                               fichier.txt

Texte à insérer













                                          [ Wrote 1 line ]
^G Get Help   ^O Write Out  ^W Where Is   ^K Cut Text   ^J Justify    ^C Cur Pos    M-U Undo
^X Exit       ^R Read File  ^\ Replace    ^U Uncut Text ^T To Spell   ^_ Go To Line M-E Redo
```

Lorsque l'on fait `^X` (`Ctrl+X`), on retourne sur la console. Mais si on a oublié de faire une sauvegarde, le programme nous demande le nom du fichier à écrire, comme si l'on sauvagardait (et c'est la cas!) mais tout de suite après revenir sur la console.

Généralement, on préfère utiliser `^X` sans passer par `^O`, car c'est plus rapide.

> Bien sûr, lorsque le programme demande un nom de fichier, on peut en choisir un autre pour povoir faire une autre version d'un fichier.
Ainsi, on peut réouvrir le fichier pour le modifier (**avec le même nom et la même casse**).

### 3. Suppression d'un fichier

Pour supprimer un/des fichier(s), il faut utiliser la commande:

```bash
rm <premier fichier à supprimer> <deuxième fichier à supprimer> ...<nième fichier à supprimer>
```

Pour supprimer un/des dossier(s):

```bash
rm -r <premier dossier à supprimer> <deuxième fichier à supprimer> ...<nième fichier à supprimer>
```

Exemple:

```console
gradient@Gradient-PC:~$ ls
Dossier  Dossier2  Dossier3  Dossier4  bin  fichier.txt  fichier2.txt  fichier_le_nom.txt
gradient@Gradient-PC:~$ rm fichier_le_nom.txt fichier2.txt
gradient@Gradient-PC:~$ ls
Dossier  Dossier2  Dossier3  Dossier4  bin  fichier.txt
gradient@Gradient-PC:~$ rm -r Dossier4 Dossier3
gradient@Gradient-PC:~$ ls
Dossier  Dossier2  bin  fichier.txt
gradient@Gradient-PC:~$
```

**ATTENTION**: Lorsque vous supprimez un ou plusieurs fichier et/ou dossiers, il partent **définitivement**, il n'y a pas de corbeille comme dans Windows.

## En conslusion

Lorsque vous utilisez Linux, beaucoup de fonctions essentielles se font à la console, malgré une potentielle interface graphique, il est mieux d'apprendre ces commandes, car si vous comptez utiliser Linux, vous passerez beaucoup plus de temps sur la console, que l'interface graphique (dans la plupart des cas, l'interface graphique peut limiter certaines actions).
=======
