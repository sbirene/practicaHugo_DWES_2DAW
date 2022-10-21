---
weight: 2
bookFlatSection: true
title: "About Hugo"
---

# Hugo

## What is HUGO?
Hugo is one of the most popular open-source static site generators. With its amazing speed and flexibility, Hugo makes building websites fun again.

## How to install HUGO?
Install Hugo on macOS, Windows or Linux.

{{< tabs "uniqueid" >}}
{{< tab "MacOS" >}} # Install Hugo on macOS
We can use Homebrew or MacPorts to install Hugo on MacOS:

With *Homebrew*
```shell
brew install hugo
```

With *MacPorts*
```shell
port install hugo
```
 {{< /tab >}}
{{< tab "Linux" >}} # Install Hugo on Linux
```shell
sudo apt-get install hugo
```
 {{< /tab >}}
{{< tab "Windows" >}} # Install Hugo on Windows
We can use Chocolatey or Scoop to install Hugo on Windows:

With *Chocolatey*
```shell
choco install hugo -confirm
```

With *Scoop*
```shell
scoop install hugo
```
 {{< /tab >}}
{{< /tabs >}}

## How to create a site with HUGO?
We go to the folder where we want to save the directories and files of the site and write the following command:

```shell
$ hugo new site <nombre_sitio>
```

And just like that we have the site created with HUGO!