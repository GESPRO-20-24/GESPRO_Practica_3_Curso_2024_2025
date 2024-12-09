![header](https://cloud.githubusercontent.com/assets/6546265/22174630/785cdf04-dfe3-11e6-8cf4-024e8dc1c051.png)

[![ZenHub](https://raw.githubusercontent.com/ZenHubIO/support/master/zenhub-badge.png)](https://zenhub.com)
[![Build Status](https://travis-ci.org/davidmigloz/go-bees.svg?branch=master)](https://travis-ci.org/davidmigloz/go-bees)
[![codecov](https://codecov.io/gh/davidmigloz/go-bees/branch/master/graph/badge.svg)](https://codecov.io/gh/davidmigloz/go-bees)
[![Code Climate](https://codeclimate.com/github/davidmigloz/go-bees/badges/gpa.svg)](https://codeclimate.com/github/davidmigloz/go-bees)
[![SonarQube](https://sonarqube.com/api/badges/gate?key=go-bees)](https://sonarqube.com/component_measures/?id=go-bees)
[![Dependency Status](https://www.versioneye.com/user/projects/57f7b19e823b88004e06ad33/badge.svg?style=flat-square)](https://www.versioneye.com/user/projects/57f7b19e823b88004e06ad33)
[![Documentation Status](https://readthedocs.org/projects/go-bees/badge/?version=develop)](http://go-bees.readthedocs.io/es/develop/?badge=develop)

## License

Copyright (c) 2016 - 2017 David Miguel Lozano

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 3 of the License, or
any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.


Autores: David Rey y David Santaolalla.


Guía de cómo se realiza toda la secuencia de acciones desde que nos posicionamos en un nuevo commit del repositorio Go Bees hasta que pasa a estar visible en nuestra rama master local.

  1. Posicionar master en el Commit del repositorio gobees.
       Para esto necesitaremos hacer click derecho sobre el commit que queramos realizar, desde GitKraken, y seleccionamos la opción Reset master to this commit. Como resultado deberemos observar que a la       
       izquierda del commit se posiciona un icono y seguido la palabra master.

  2. Actualizamos el master en nuestro repositorio.
       Una vez se ha realizado el paso uno, desde GitKraken debemos acceder a nuestro repositorio, y desde la rama master debemos hacer un Fetch All y un push y pull para dejar actualizado nuestro master y asi           tener todo listo para poder trabajar sobre nuestro repositorio.

  3. Crear issue con el nombre del commit.
       A partir de este momento debemos de acceder a nuestro repositorio en GitHub y crear una nueva issue con el nombre del commit que estemos trabajando.

  4. Crear rama de la tarea.
       Una vez tengamos creada la tarea, debemos visualizar en la misma pantalla de GitHub, a la derecha sobre la opcion Development aparecerá la opción Create Branch. Clickando en esa opcion crearemos la branch         de nuestra issue. A partir de aqui podemos ir a kitKraken de nuevo, puesto que nuestra rama ya estará creada.

  5. Posicionarnos en la rama local.
       Una vez tengamos la rama creada desde GitKraken seleccionaremos en la tabla de la izquierda la rama recien creada para posicionarnos en local. 

  6. Añadir cambios en la carpeta.
       Abriremos el explorador de archivos y copiaremos todos los archivos de la carpeta gobees exceptuando la carpeta .git, a continuación iremos a nuestra carpeta donde tengamos los archivos de nuestro     
       repositorio y pegaremos sobreescribiendo los archivos antiguos. 

  7. Realizar los cambios en Git Kraken
       Una vez hayamos hecho el pegado de los archivos debemos ir a GitKraken y clickar en stage all changes arriba a la derecha de nuestras pantallas. Posteriormente debemos introducir el nombre del commit abajo        a la derecha y guardar los cambios.
   
       También procederemos a realizar Fetch All, push y pull para actualizar el estado del commit.

  8. Crear Pull Request del commit.
       Uno de nuestros últimos pasos será realizar un Pull Request de nuestro commit, fijandonos que el resultado final del Pull Request tenga la estructura de commit into master from (nombre de nuestra rama). 
 
  9. Hacer Merge del Pull Request.
       Nada más realizar el Pull Request, debemos realizar un merge del mismo, esto lo haremos en la misma pantalla tras haber realizado el Pull Request, en un cuadrado verde aparecerá la opción. Simplemente             clicaremos en ella.

10. Actualizar los cambios en GitKraken.
    Por último nos iremos a nuestro repositorio en GitKraken para realizar un último Fetch All, push and pull para poder visualizar nuestros cambios en el grafo y así completar el commit.


El siguiente paso consiste en posicionarnos en el siguiente commit, y realizar de nuevo todos los pasos, pues debemos hacer esto con cada commit.
