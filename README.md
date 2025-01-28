#  INSTRUCCIONES DE TRABAJO CON ARCHIVOS EN GITHUB

### Creación del proyecto y subida a GitHub

*(Ejemplo con proyecto creado en Symfony)*

Para crear nuestro proyecto, ejecutaremos el siguiente código dentro de la carpeta raíz con la que vayamos a trabajar:

``` php
sympony new (nombre-del-proyecto)
```

Creamos a continuación un archivo README.md como este, añadimos la información que necesitemos y guardamos para, a continuación, efectuar el commit correspondiente.

En GitHub, iniciamos sesión con nuestra cuenta, buscamos el botón **New** en *Top Repositories* y pulsamos para iniciar la creación de un nuevo repositorio.

Una vez entremos introducimos en **Repository Name** el nombre de nuestro proyecto. El resto de campos son opcionales y no los tocaremos. 

Una vez creado, GitHub nos dará una dirección URL que copiaremos para añadirla al siguiente código:

``` shell
git remote add origin
``` 

Finalmente, escribiremos:

``` php
git push -u origin (master o main según sea la rama en la que trabajamos)
```


### Descarga del proyecto desde GitHub

En primer lugar, debemos clonar el repositorio alojado en GitHub. Para ello abriremos un terminal en la carpeta en la que queramos copiarlo y escribiremos:

``` php
git clone (nombre-del-proyecto)
```

GitHub no copia aquellos archivos y carpetas sobre los que no tiene seguimiento. Estos archivos se pueden encontrar en el archivo **.gitignore** de nuestro proyecto. Entre ellos están por lo general las carpetas **var** y **vendor**, que deberemos restaurar ejcutando el siguiente código:

``` php
composer install
```
