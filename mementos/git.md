# Git

💠 _Les paramètres globaux sont enregistés dans le fichier de configuration **.gitconfig**_

![logo de Git](https://nsa40.casimages.com/img/2021/03/14/210314041119892755.png)

**SOMMAIRE**
+ [Afficher la version](#afficher-la-version)
+ [Afficher les changements entre commits/arbre de travail](#afficher-les-changements-entre-commis-arbre-de-travail)
+ [Afficher l'état de l'arborescence](#afficher-létat-de-larborescence)
+ [Afficher l'historique des commits](#afficher-lhistorique-des-commits)
+ [Ajouter un fichier à l'index du dépôt](#ajouter-un-fichier-à-lindex-du-dépôt)
+ [Annuler des commits](#annuler-des-commits)
+ [Changer de branche courante](#changer-de-branche-courante)
+ [Cloner un dépôt](#cloner-un-dépôt)
+ [Configurer des informations globales](#configurer-des-informations-globales)
+ [Créer une nouvelle branche](#créer-une-nouvelle-branche)
+ [Créer un nouveau dépôt vide](#créer-un-nouveau-dépôt-vide)
+ [Déplacer ou renommer un fichier](#déplacer-ou-renommer-un-fichier)
+ [Fusionner une branche à la branche principale](#fusionner-une-branche-à-la-branche-principale)
+ [Lister les branches](#lister-les-branches)
+ [Lister les informations de configuration](#lister-les-informations-de-configuration)
+ [Mettre à jour le dépôt distant avec les changements en local](#mettre-à-jour-le-dépôt-distant-avec-les-changements-en-local)
+ [Supprimer un fichier](#supprimer-un-fichier)
+ [Synchroniser les fichiers d'un dépôt distant avec le dépôt local](#synchroniser-les-fichiers-dun-dépôt-distant-avec-le-dépôt-local)
+ [Valider les changements dans le dépôt](#valider-les-changements-dans-le-dépôt)

---

## Afficher la version

```powershell
git version
git --version
```

## Afficher les changements entre commits/arbre de travail

```powershell
git diff <some_commit_id> <other_commit_id>
```

## Afficher l'état de l'arborescence

```powershell
git status
```

## Afficher l'historique des commits

```powershell
git log
```

## Ajouter un fichier à l'index du dépôt

```powershell
git add <file>
git add *.html
```

## Annuler des commits

```powershell
git revert <commit_id> # remet le dépôt dans l'état où il se trouvait au moment de ce commit
```

## Changer de branche courante

```powershell
git checkout <branch>
```

## Cloner un dépôt

```powershell
git clone <repository> # git clone https://github.com/microsoft/vscode.git
```

## Configurer des informations globales

> Retirer l'argument **--global** appliquera la configuration au dépôt courant uniquement

```powershell
git config --global init.defaultbranch "<default_branch_name>"
git config --global core.editor "<path_to_file_editor>"
git config --global user.name "<username>"
git config --global user.email "<email>"
```

## Créer une nouvelle branche

```powershell
git branch <name>
```

## Créer un nouveau dépôt vide

> Si le dépôt existe déjà, va le réinitialiser<br>
> Par défaut, la branche est du même nom que celui configuré dans les paramètres
 
```powershell
git init
git init -b <branch_name>
```

## Déplacer ou renommer un fichier

```powershell
git mv <old_file> <new_file>
git mv <old_path_to_file> <new_path_to_file>
```

## Fusionner une branche à la branche principale

```powershell
git merge <branch>
```

## Lister les branches

```powershell
git branch
```

## Lister les informations de configuration

```powershell
git config --list
```

## Mettre à jour le dépôt distant avec les changements en local

```powershell
git push # git push origin master
```

## Supprimer un fichier

```powershell
git rm <file>
```

## Synchroniser les fichiers d'un dépôt distant avec le dépôt local

```powershell
git pull
```

## Valider les changements dans le dépôt

```powershell
git commit
git commit -m "<message>"
```
