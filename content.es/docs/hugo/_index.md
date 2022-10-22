---
weight: 2
bookFlatSection: true
title: "Sobre Hugo"
---

# Hugo

## ¿Qué es HUGO?
Hugo es un generador de sitios web estáticos, construidos con el lenguaje GO. Fue creado en el año 2013.

Con él se pueden generar sitios web en poco tiempo, versátiles y muy rápidos.

## ¿Cómo instalar HUGO?
Hugo se puede instalar en múltiples sistemas operativos. Aquí vamos a explicar cómo instalarlo en MacOS, Linux y Windows.

{{< tabs "uniqueid" >}}
{{< tab "MacOS" >}} # Instalación Hugo en MacOS
Podemos utilizar Homebrew o MacPorts para instalar Hugo en MacOS:

Con *Homebrew*
```shell
brew install hugo
```

Con *MacPorts*
```shell
port install hugo
```
 {{< /tab >}}
{{< tab "Linux" >}} # Instalación Hugo en Linux
```shell
sudo apt-get install hugo
```
 {{< /tab >}}
{{< tab "Windows" >}} # Instalación Hugo en Windows
Podemos utilizar Chocolatey o Scoop para instalar Hugo en Windows:

Con *Chocolatey*
```shell
choco install hugo -confirm
```

Con *Scoop*
```shell
scoop install hugo
```
 {{< /tab >}}
{{< /tabs >}}

## ¿Cómo crear un sitio con HUGO?
Nos situamos en la carpeta en la que queramos guardar los directorios y archivos del sitio y escribimos el siguiente comando:

```shell
$ hugo new site <nombre_sitio>
```

!Y así ya tenemos el sitio creado con HUGO!