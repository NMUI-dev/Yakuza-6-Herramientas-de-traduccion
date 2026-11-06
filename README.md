# Yakuza 6: The Song of Life: herramientas y guía para traducir

Todo lo necesario para corregir la traducción al español de Yakuza 6: The Song of Life, pasarla a otro idioma o
traducir otro juego de la saga. **Incluye los `.exe`**, así que no hay que descargar nada más que Python.

**Para jugar no hace falta nada de esto:** descarga la
[traducción](https://github.com/NMUI-dev/Yakuza-6-The-Song-of-Life-Espa-ol-Spanish/releases/latest).

## Empieza aquí

**[Paso a paso](PASO_A_PASO.txt)**: qué se hizo, con qué programas, dónde guarda el texto el juego y qué trampas tiene.
**[Cómo usar el programa](COMO_USAR.txt)**: sacar todos los textos a una hoja, corregirlos y volver a meterlos.

En resumen:

1. Descarga y descomprime la [traducción](https://github.com/NMUI-dev/Yakuza-6-The-Song-of-Life-Espa-ol-Spanish/releases/latest).
2. Descomprime este repositorio **dentro** de esa carpeta, en una carpeta llamada `Herramientas para traduccion`
   (junto a `archivos` y a `INSTALAR o QUITAR.bat`).
3. Instala [Python 3](https://www.python.org) y marca **Add python.exe to PATH**.
4. Doble clic en `EXTRAER textos.bat`.
5. Corrige la columna `espanol` de `trabajo\textos.csv`.
6. Doble clic en `APLICAR textos.bat`.
7. Instala con `INSTALAR o QUITAR.bat`, en la carpeta de la traducción.

## Las cifras

| | |
|---|--:|
| Textos distintos | 29.349 |
| Textos traducidos (el resto son nombres, marcas y códigos) | 28.021 |
| Veces que aparecen en el juego | 60.928 |
| Letras en inglés | 1.476.219 |
| Imágenes con texto traducidas | 323 |
| Archivos del juego que cambian | 223 |

## Qué hay aquí

| Archivo | Para qué |
|---|---|
| `PASO_A_PASO.txt` | Qué se hizo y cómo funciona el juego por dentro |
| `COMO_USAR.txt` | Cómo usar el programa de textos |
| `EXTRAER textos.bat`, `APLICAR textos.bat` | Sacan los textos a una hoja y los vuelven a meter |
| `herramienta_traduccion.py` | El programa que usan esos `.bat` |
| `datos/` | Dónde está cada texto: tablas, diálogos y subtítulos de escenas |
| `programas/ParTool/` | Abre y rearma los `.par` |
| `programas/reARMP/` | Lee y escribe las tablas ARMP |

Este repositorio no lleva archivos del juego, así que necesitas tu propia copia. Tampoco se suben `trabajo/` ni
`salida/`, las carpetas que se crean al usarlo.

## Antes de corregir diálogos

- Mira **quién habla y a quién**: el inglés no marca el género («I'm sure», «Are you ready?»). Kiryu es hombre; las
  anfitrionas hablan de sí en femenino.
- Cada frase inglesa distinta se traduce **una sola vez** para todo el juego (columna `veces`). Si sale en escenas con
  personas distintas, usa una forma que valga para todas («¿De verdad?» en vez de «¿Estás seguro?»).
- En el chat en vivo, lo que se teclea va en MAYÚSCULAS sin tildes y no debe quedar cortado a media frase.

## Programas incluidos

Son de sus autores. Se incluyen sin cambios, con su licencia al lado.

| Programa | Autor | Licencia | SHA-256 |
|---|---|---|---|
| [ParTool 1.3.4](https://github.com/Kaplas80/ParManager/releases/tag/v1.3.4) (ParManager) | Kaplas80 | MIT | `b798027a243229c04741e491abb1f92ae4cc7a379c0cba31b81446f9be4e5b3f` |
| [reARMP](https://github.com/Ret-HZ/reARMP) | Ret-HZ | GPL-2.0 | |

Si el antivirus avisa, comprueba la SHA-256 con `certutil -hashfile <archivo> SHA256` o descarga el programa de su autor.

## Avisos

- Mod no oficial, gratuito y sin fines de lucro. **Prohibido venderlo.**
- Hecho con IA y supervisado por una persona. No está afiliado a SEGA. Más detalles en [AVISO.txt](AVISO.txt).
- El código propio es MIT ([LICENSE](LICENSE)). Yakuza y sus textos e imágenes son de SEGA.

## English

Tools and a step-by-step guide (in Spanish) to edit the Spanish fan translation of *Yakuza 6: The Song of Life*, or to
translate it or another game in the series. ParTool and reARMP are included. You need your own copy of the game.
