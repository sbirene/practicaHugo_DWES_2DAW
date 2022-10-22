---
weight: 2
bookFlatSection: true
title: "Sur Hugo"
---

# Hugo

## C'est quoi HUGO?
Hugo est un générateur de site Web statique, construit avec le langage GO. Il a été créé en 2013.

Avec lui, vous pouvez générer des sites Web en peu de temps, polyvalents et très rapides.

## Comment installer HUGO ?
Hugo peut être installé sur plusieurs systèmes d'exploitation. Ici, nous allons vous expliquer comment l'installer sur MacOS, Linux et Windows.

{{< tabs "uniqueid" >}}
{{< tab "MacOS" >}} # Installer Hugo sur MacOS
Nous pouvons utiliser Homebrew ou MacPorts pour installer Hugo sur MacOS :

Avec *Homebrew*
```shell
brew install hugo
```

Avec *MacPorts*
```shell
port install hugo
```
 {{< /tab >}}
{{< tab "Linux" >}} # Installer Hugo sur Linux
```shell
sudo apt-get install hugo
```
 {{< /tab >}}
{{< tab "Windows" >}} # Installer Hugo sur Windows
On peut utiliser Chocolatey ou Scoop pour installer Hugo sur Windows:

Avec *Chocolatey*
```shell
choco install hugo -confirm
```

Avec *Scoop*
```shell
scoop install hugo
```
 {{< /tab >}}
{{< /tabs >}}

## Comment créer un site avec HUGO ?
Nous allons dans le dossier où nous voulons enregistrer les répertoires et fichiers du site et écrivons la commande suivante:

```shell
$ hugo new site <nombre_sitio>
```

Et donc nous avons déjà le site créé avec HUGO!