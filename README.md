# Lady Stalker — Traducción al castellano

[![Invítame a un café en Ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/johanderohan)

Traducción al **castellano de España** de *Lady Stalker: Kako kara no Chousen*, para Super Nintendo / Super Famicom. El guion parte del original japonés.

La descarga contiene un parche XDELTA. Necesitas tu propia copia del juego; no se incluye la ROM.

## Estado

Última versión: **[v1.0](../../releases/tag/v1.0)**. Estado: **en revisión de partida**.

El trabajo incluye 1220 mensajes principales, 352 registros de diccionario BYTE y 6 WORD —conservando sus vacíos originales—, 30 líneas de prólogo, menús y gráficos funcionales. Los créditos y las pantallas de final incluyen 31 rótulos localizados; se mantienen nombres de personas y logotipos.

Los objetos y algunas habilidades utilizan nombres abreviados en listas estrechas. Los diálogos conservan los nombres completos. Se mantienen las siglas LP/SP del original.

### Comprobaciones y límites

Probado con Snes9x 1.63 mediante libretro en Linux. Se ha recorrido desde partida nueva el prólogo, el puerto, el inventario, el equipo, los atributos y una tienda, incluyendo compra y venta. Se han comprobado también, mediante rutas dirigidas declaradas, combate con objeto y magia, Plan, guardado, cargas normales desde SRAM en procesos nuevos, copia y borrado de una copia, almacén/banco, viajes, casino y créditos/final.

La candidata se ha reconstruido de forma independiente desde fuentes congeladas y el resultado es idéntico. El parche se ha reaplicado al original y comparado byte a byte. La auditoría final incluye controles, fuentes, punteros, bancos, aliases, cifras y las regresiones de ventanas y del ticker de combate.

Quedan términos puntuales pendientes de contraste visual: un parentesco, la referencia espacial al horno, el tipo de transporte a la mina y un nombre de enemigo. No se acredita la revisión contextual de todas las escenas ni de todos los objetos y destinos.

La traducción, el romhacking y la revisión están asistidos por IA. No se acredita una partida completa, revisión humana independiente ni prueba en consola física. Las pruebas dirigidas se identificarán separadamente del recorrido normal.

## Cómo aplicar el parche

1. Descarga el archivo `.xdelta` de [Releases](../../releases).
2. Comprueba que tu ROM es la japonesa original, sin cabecera de copiador ni otros parches:

   | Dato | Valor |
   |---|---|
   | Archivo de referencia | `Lady Stalker - Kako kara no Chousen (Japan).sfc` |
   | Tamaño | 2.621.440 bytes |
   | MD5 | `25694e43df2dd3f8cd756132778911a1` |
   | SHA-256 | `d0275f6fdc38f26b53b017bdd7fe26e13b9871a93671c76f48800e4f733b2385` |
   | CRC32 | `4390D719` |

3. Aplica el parche con Delta Patcher o con `xdelta3`:

   ```sh
   xdelta3 -d -s "Lady Stalker - Kako kara no Chousen (Japan).sfc" "Lady-Stalker-Castellano-v1.0.xdelta" "Lady Stalker - Castellano.sfc"
   ```

4. Verifica el resultado: tamaño 4.194.304 bytes; MD5 `6bb5683f217f436418806646ee9dab6f`; SHA-256 `cea1f6da27d6b491ba5b79b7a1222532f71c5ffac516bd61ef50828e4f0f9ff3`.
5. Empieza una partida nueva. No cargues estados de emulador creados con la ROM original u otra candidata. La prueba de guardar/cargar se refiere a partidas normales de esta versión.

Cada versión se aplica sobre la ROM japonesa original, no sobre una traducción anterior.

## Cambios

### v1.0 — 28 de octubre de 2026

- Primera publicación de historia, prólogo, interfaz, objetos, equipo, habilidades y consignas de Plan en castellano.
- Caracteres españoles y ajuste de palabras; aliases locales que mantienen los nombres completos en el diálogo.
- Casino traducido tanto en fondos como en sprites activos, incluyendo instrucciones y resultados.
- Rótulos de créditos y final localizados, conservando nombres propios y marcas.
- Guardado/carga, ventanas compartidas y banda del ticker comprobados en el alcance indicado.

## Créditos y aviso

Proyecto de [johanderohan](https://github.com/johanderohan). Lady Stalker y sus personajes pertenecen a sus respectivos titulares. Este proyecto no está afiliado a Climax ni a Taito; distribuye únicamente un parche para una copia propia.

Se consultó un toolkit público como referencia técnica. El guion se tradujo desde el japonés: no se aplicó una traducción inglesa como base.

Algunos rótulos compactos se han rasterizado a partir de DejaVu Sans. Los nuevos glifos de sistema tienen diseño propio; se conservan las formas nativas que el motor necesita. Se incluye el aviso de licencia de la fuente empleada en los rótulos.

<details>
<summary>Licencia de DejaVu Sans / Bitstream Vera</summary>

```text
Fonts are (c) Bitstream (see below). DejaVu changes are in public domain.
Glyphs imported from Arev fonts are (c) Tavmjong Bah (see below)


Bitstream Vera Fonts Copyright
------------------------------

Copyright (c) 2003 by Bitstream, Inc. All Rights Reserved. Bitstream Vera is
a trademark of Bitstream, Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of the fonts accompanying this license ("Fonts") and associated
documentation files (the "Font Software"), to reproduce and distribute the
Font Software, including without limitation the rights to use, copy, merge,
publish, distribute, and/or sell copies of the Font Software, and to permit
persons to whom the Font Software is furnished to do so, subject to the
following conditions:

The above copyright and trademark notices and this permission notice shall
be included in all copies of one or more of the Font Software typefaces.

The Font Software may be modified, altered, or added to, and in particular
the designs of glyphs or characters in the Fonts may be modified and
additional glyphs or characters may be added to the Fonts, only if the fonts
are renamed to names not containing either the words "Bitstream" or the word
"Vera".

This License becomes null and void to the extent applicable to Fonts or Font
Software that has been modified and is distributed under the "Bitstream
Vera" names.

The Font Software may be sold as part of a larger software package but no
copy of one or more of the Font Software typefaces may be sold by itself.

THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT OF COPYRIGHT, PATENT,
TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL BITSTREAM OR THE GNOME
FOUNDATION BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, INCLUDING
ANY GENERAL, SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL DAMAGES,
WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF
THE USE OR INABILITY TO USE THE FONT SOFTWARE OR FROM OTHER DEALINGS IN THE
FONT SOFTWARE.

Except as contained in this notice, the names of Gnome, the Gnome
Foundation, and Bitstream Inc., shall not be used in advertising or
otherwise to promote the sale, use or other dealings in this Font Software
without prior written authorization from the Gnome Foundation or Bitstream
Inc., respectively. For further information, contact: fonts at gnome dot
org.

Arev Fonts Copyright
------------------------------

Copyright (c) 2006 by Tavmjong Bah. All Rights Reserved.

Permission is hereby granted, free of charge, to any person obtaining
a copy of the fonts accompanying this license ("Fonts") and
associated documentation files (the "Font Software"), to reproduce
and distribute the modifications to the Bitstream Vera Font Software,
including without limitation the rights to use, copy, merge, publish,
distribute, and/or sell copies of the Font Software, and to permit
persons to whom the Font Software is furnished to do so, subject to
the following conditions:

The above copyright and trademark notices and this permission notice
shall be included in all copies of one or more of the Font Software
typefaces.

The Font Software may be modified, altered, or added to, and in
particular the designs of glyphs or characters in the Fonts may be
modified and additional glyphs or characters may be added to the
Fonts, only if the fonts are renamed to names not containing either
the words "Tavmjong Bah" or the word "Arev".

This License becomes null and void to the extent applicable to Fonts
or Font Software that has been modified and is distributed under the 
"Tavmjong Bah Arev" names.

The Font Software may be sold as part of a larger software package but
no copy of one or more of the Font Software typefaces may be sold by
itself.

THE FONT SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT
OF COPYRIGHT, PATENT, TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL
TAVMJONG BAH BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY,
INCLUDING ANY GENERAL, SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL
DAMAGES, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF THE USE OR INABILITY TO USE THE FONT SOFTWARE OR FROM
OTHER DEALINGS IN THE FONT SOFTWARE.

Except as contained in this notice, the name of Tavmjong Bah shall not
be used in advertising or otherwise to promote the sale, use or other
dealings in this Font Software without prior written authorization
from Tavmjong Bah. For further information, contact: tavmjong @ free
. fr.

TeX Gyre DJV Math
-----------------
Fonts are (c) Bitstream (see below). DejaVu changes are in public domain.

Math extensions done by B. Jackowski, P. Strzelczyk and P. Pianowski
(on behalf of TeX users groups) are in public domain.

Letters imported from Euler Fraktur from AMSfonts are (c) American
Mathematical Society (see below).
Bitstream Vera Fonts Copyright
Copyright (c) 2003 by Bitstream, Inc. All Rights Reserved. Bitstream Vera
is a trademark of Bitstream, Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of the fonts accompanying this license (“Fonts”) and associated
documentation
files (the “Font Software”), to reproduce and distribute the Font Software,
including without limitation the rights to use, copy, merge, publish,
distribute,
and/or sell copies of the Font Software, and to permit persons  to whom
the Font Software is furnished to do so, subject to the following
conditions:

The above copyright and trademark notices and this permission notice
shall be
included in all copies of one or more of the Font Software typefaces.

The Font Software may be modified, altered, or added to, and in particular
the designs of glyphs or characters in the Fonts may be modified and
additional
glyphs or characters may be added to the Fonts, only if the fonts are
renamed
to names not containing either the words “Bitstream” or the word “Vera”.

This License becomes null and void to the extent applicable to Fonts or
Font Software
that has been modified and is distributed under the “Bitstream Vera”
names.

The Font Software may be sold as part of a larger software package but
no copy
of one or more of the Font Software typefaces may be sold by itself.

THE FONT SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS
OR IMPLIED, INCLUDING BUT NOT LIMITED TO ANY WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT OF COPYRIGHT, PATENT,
TRADEMARK, OR OTHER RIGHT. IN NO EVENT SHALL BITSTREAM OR THE GNOME
FOUNDATION
BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, INCLUDING ANY GENERAL,
SPECIAL, INDIRECT, INCIDENTAL, OR CONSEQUENTIAL DAMAGES, WHETHER IN AN
ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF THE USE OR
INABILITY TO USE
THE FONT SOFTWARE OR FROM OTHER DEALINGS IN THE FONT SOFTWARE.
Except as contained in this notice, the names of GNOME, the GNOME
Foundation,
and Bitstream Inc., shall not be used in advertising or otherwise to promote
the sale, use or other dealings in this Font Software without prior written
authorization from the GNOME Foundation or Bitstream Inc., respectively.
For further information, contact: fonts at gnome dot org.

AMSFonts (v. 2.2) copyright

The PostScript Type 1 implementation of the AMSFonts produced by and
previously distributed by Blue Sky Research and Y&Y, Inc. are now freely
available for general use. This has been accomplished through the
cooperation
of a consortium of scientific publishers with Blue Sky Research and Y&Y.
Members of this consortium include:

Elsevier Science IBM Corporation Society for Industrial and Applied
Mathematics (SIAM) Springer-Verlag American Mathematical Society (AMS)

In order to assure the authenticity of these fonts, copyright will be
held by
the American Mathematical Society. This is not meant to restrict in any way
the legitimate use of the fonts, such as (but not limited to) electronic
distribution of documents containing these fonts, inclusion of these fonts
into other public domain or commercial font collections or computer
applications, use of the outline data to create derivative fonts and/or
faces, etc. However, the AMS does require that the AMS copyright notice be
removed from any derivative versions of the fonts which have been altered in
any way. In addition, to ensure the fidelity of TeX documents using Computer
Modern fonts, Professor Donald Knuth, creator of the Computer Modern faces,
has requested that any alterations which yield different font metrics be
given a different name.

$Id$
```
</details>
