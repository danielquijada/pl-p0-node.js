Practica 0: Tutorial de Instalación de Node.JS
==============================================

## Instalación en Linux

### Instalación normal

En caso de que el paquete esté incluido en el repositorio de paquetes de Ubuntu, y de que no de problemas:

1. Abrir una terminal (Ctrl + T).
2. Introducir los siguientes comandos:
```
sudo apt-get install curl
curl -sL https://deb.nodesource.com/setup | sudo bash
sudo apt-get install -y nodejs
```

### Instalación alternativa. Usando Node Version Manager (NVM)

Hay casos en los que esta instalación puede dar algunos problemas. El comando `apt-get install`dando errores, que se instale una versión no actualizada o que no se añada al PATH, entre otros. Para esos casos, existen alternativas, una de las cuales es:

1. Abrir una consola (Ctrl + T).
2. Introducir los siguientes comandos:
```
$ sudo apt-get update
$ sudo apt-get install build-essential libssl-dev
```
3. Descargar el script de instalación de nvm:
```
$ curl https://raw.githubusercontent.com/creationix/nvm/<span class="highlight">v0.7.0</span>/install.sh | sh
```
4. Una vez hecho esto, hay que salir y entrar de Ubuntu. De forma alternativa, mucho más rápida, recargar el archivo .profile:
```
$ source ~/.profile
```
5. Hecho esto, se puede instalar la versión que deseemos. Para ver un listado de todas las versiones:
```
$ nvm ls-remote
```
6. Elegir la versión deseada (recomendablemente la última estable) e instalarlo con el comando:
```
$ nvm install <numero de version>
```

## Instalación en Windows

También se puede instalar en Windows, para los que no tengan instalada ninguna distribución de Ubuntu. El proceso estándar de instalación es bastante sencillo:

1. Se debe descargar el installer desde: http://nodejs.org/ (Downloads > Elegir el adecuado para tu SO).
2. Ejecutarlo y seguir el Wizard de instalación.
3. Ejecutar desde el ejecutable de Node.JS, o desde la consola con el comando node.

## Utilización

Tanto en Linux como en Windows, dispondrás de una consola de Node.JS; en la que podrás escribir tus funciones y expresiones:

