# Git

▶ Les paramètres globaux sont enregistés dans le fichier de configuration **.gitconfig**

**SOMMAIRE**
> + [Afficher l'historique des commits](#afficher-lhistorique-des-commits)
> + [Ajouter un fichier à l'index du dépôt](#ajouter-un-fichier-à-lindex-du-dépôt)
> + [Configurer des informations globales](#configurer-des-informations-globales)
> + [Créer un nouveau dépôt vide](#créer-un-nouveau-dépôt-vide)
> + [Lister les informations de configuration](#lister-les-informations-de-configuration)
> + [Valider les changements dans le dépôt](#valider-les-changements-dans-le-dépôt)

---

## Afficher l'historique des commits

```powershell
git log
```

## Ajouter un fichier à l'index du dépôt

```powershell
git add <file>
```

## Configurer des informations globales

> Retirer l'argument **--global** appliquera la configuration au dépôt courant uniquement

```powershell
git config --global init.defaultbranch "<default_branch_name>"
git config --global core.editor "<path_to_file_editor>"
git config --global user.name "<username>"
git config --global user.email "<email>"
```

## Créer un nouveau dépôt vide

> Si le dépôt existe déjà, va le réinitialiser<br>
> Par défaut, la branche est du même nom que celui configuré dans les paramètres
 
```powershell
git init
git init -b <branch_name>
```

## Lister les informations de configuration

```powershell
git config --list
```

## Valider les changements dans le dépôt

```powershell
git commit
git commit -m "<message>"
```
