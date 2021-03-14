# Git

**SOMMAIRE**
> + [Configurer des informations globales](#configurer-des-informations-globales)
> + [Créer un nouveau dépôt vide](#créer-un-nouveau-dépôt-vide)
> + [Lister les informations globales de configuration](#lister-les-informations-globales-de-configuration)

---

## Configurer des informations globales

> Paramètres personnalisés situés dans le fichier **.gitconfig**

```powershell
git config --global init.defaultbranch "<default_branch_name>"
git config --global core.editor "<path_to_file_editor>"
git config --global user.name "<username>"
git config --global user.email "<email>"
```

## Créer un nouveau dépôt vide

> Si le dépôt existe déjà, va le réinitialiser
> Par défaut, crée une branche du même nom que celui configuré dans les paramètres (**.gitconfig**)
 
```powershell
git init
git init -b <branch_name>
```

## Lister les informations globales de configuration

```powershell
git config --list
```
