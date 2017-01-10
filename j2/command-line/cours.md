# O'Clock j2 - La ligne de commande

Fait par Guillaume L.

Si vous avez des questions : `guillaume.lodi@gmail.com`.

## Avant de commencer

### Ouverture d'un terminal
Plusieurs options possibles :
- En bas a gauche du menu mint, cliquer sur l'icone du terminal
- Depuis n'importe quel endroit, `ctrl + alt + t` ouvre un terminal (et plus généralement dans la plupart des distributions linux).

### La casse
Le **shell script** (ou le language que vous utilisez dans le terminal) est un langage qui est sensible à la casse. C'est à dire que les majuscules et les minuscules sont considérés comme des caractères différents.

Par exemple `pwd` est une commande, alors que `PWD ou Pwd ou pWD...` n'est pas une commande (n'existe pas).

### La tilde `~` ou /home/mint
Dans le terminal, la tilde représente le répertoire HOME de l'utilisateur (vous). Ce répertoire est celui dans lequel vous trouvez (la plupart du temps) les dossiers suivants  :
- Bureau
- Documents
- Modèles
- Public
- Vidéos
- Images
- Musique
- Téléchargements


--------------------
## C'est parti ! Les commandes basiques : naviguez dans vos fichiers à l'aide du terminal.

D'habitude, on utilise un explorateur de fichier, et on clique sur les dossiers pour les ouvrir (ou sur les fichiers). Saviez-vous qu'il était possible d'y naviguer à partir d'un terminal ? Le tout en utilisant seulement trois commandes : `pwd`, `cd` et `ls`.


### `pwd` - Heu je suis où là ?
Première commande. Cette commande est extrèmement utilse si vous êtes perdu, elle sert à afficher le dossier dans lequel vous vous trouvez acutuellement.

Entrez `pwd` dans le terminal et appuyez sur entrée.
```shell
mint@mint ~ $ pwd
/home/mint
```
`pwd` veut dire "print working directorie" et sert à afficher le répertoire courant.
Dans notre cas, le répertoire courant lors de l'ouverture du terminal est `/home/mint`.


### `ls` - Un peu de lumière svp !
Cette commande sert à afficher la liste des fichier du répertoire courant.
Tapez `ls` dans le terminal et appuyez sur entrée.
```shell
mint@mint ~ $ ls
Bureau   Documents  Modèles  Public           Vidéos
Desktop  Images     Musique  Téléchargements
```


### `cd` - C'est naze ici, je me casse !

Cette commande sert à se déplacer parmi les fichiers.
En tapant ls, vous avez précédemment listé les fichiers de votre répertoire courant. Maintenant, essayez de rentrer dans le dossier `Documents` en tapant `cd Documents/`

```shell
mint@mint ~ $ ls
Bureau   Documents  Modèles  Public           Vidéos
Desktop  Images     Musique  Téléchargements

mint@mint ~ $ cd Documents/
mint@mint ~/Documents $
```

Pour entrez dans un dossier tapez `cd nouveauDossier/`

Pour revenir dans le dossier parent tapez `cd ../`

Dans chaque dossier, vous avez `.` qui représente le dossier dans lequel vous êtes, et `..` qui représent le dossier parent.


### `mkdir` - Créer un dossier
Pour créer un dossier, utilisez la commande `mkdir`
```shell
mint@mint ~ $ mkdir nouveauDossier/
```
Créera un dossier dans le répertoire courant.

Autres exemples d'utilisation :
```shell
mint@mint ~ $ mkdir ../nouveauDossier/
mint@mint ~ $ mkdir dossierExistant/nouveauDossier/
```

Vous constatez que mkdir ne se limite pas au dossier actuel, vous pouvez aussi créer des dossiers via mkdir `chemin/nouveauDossier`


--------------------
### L'autocompletion
Très utile. Les développeurs sont des flemmards, c'est pour ça qu'ils ont mis en place l'autocomplétion.
Le principe c'est d'appuyez sur la touche `tabulation` pendant la saisie, et l'ordinateur va compléter tout seul votre saisie **si il peut**.
