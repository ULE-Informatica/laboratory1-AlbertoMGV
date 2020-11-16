<!-- Banner cutre pero kuki <3 -->
<br />
<p align="center">
  <img src="https://www.unileon.es/themes/ulebase/images/escudo-ule.svg" alt="Logo" width="250" height="200"/>
  <a href="https://agora.unileon.es/mod/assign/view.php?id=63782"><h3 align="center">Laboratorio 1</h3></a>
  <p align="center">
    Diseño y Programación Seguras
    <br/>
    <p align="center">Alberto Miranda García</p>
  </p>
</p>

<!-- Indice -->
## Índice

* [Información General ](#información-general)
* [Supresion de Warnings y Cambios](#supresion-de-warnings-y-cambios)
* [Reglas y Recomendaciones](#reglas-y-recomendaciones)

<!-- Informacion General -->
## Información General

En esta practica he utilizado la maquina virtual que uso para la Universidad, tengo Ubuntu 20.04.1 LTS y GCC con la version 9.3.0. En esta practica, he compilado el codigo siguiendo dos diferentes estandares,  ISO/IEC 9899:2011 (C11) y ISO/IEC 9899:1999 (C99). En el cmake dejo los dos estandares para compilarlo a tu gusto. Los comandos que he usado son los siguientes:
```console
albertomgv@cole:~$ gcc -Wall -std=c99 exampleStrings.c 
```
```console
albertomgv@cole:~$ gcc -Wall -std=c11 exampleStrings.c 
```
<!-- Supresion de Warnings -->
## Supresion de Warnings y cambios

 - Funcion gets_example_func es void y devuelve un valor.
 - Sustitución de funcion gets (deprecated) por fgets.
 - Declaración de variable s1 (multilinea).
 - Declaración de variable ptr_char (Para permitir ser modficado de forma segura).
 - Tamaño variable response en get_y_or_n innecesario.
 - Comentar variables no utilizadas.
 - Reservar memoria para variable slash.

<!-- Reglas y Recomendaciones Generales -->
## Reglas y Recomendaciones

  - ARR02-C: Explicitly specify array bounds, even if implicitly defined by an initializer. [ l18 ]
  - ARR32-C: Ensure size arguments for variable length arrays are in a valid range. [ l48 ]
  - MSC24-C: Do not use deprecated or obsolescent functions. [ l51 ]
  - STR11-C: Do not specify the bound of a character array initialized with a string literal. [ l72 ]
  - STR03-C: Do not inadvertently truncate a string. [ l77-79 ]
  - STR30-C: Do not attempt to modify string literals. [ l100 ]


## Referencias

  - [Carnegie Mellow University Wiki](https://wiki.sei.cmu.edu/confluence/display/c/2+Rules)
  - [Sonar Source](https://rules.sonarsource.com/c/RSPEC-3519)
  - [Listado de Reglas y Recomendaciones - Agora](https://agora.unileon.es/pluginfile.php/141504/mod_resource/content/1/DPS_Plantilla.pdf)


