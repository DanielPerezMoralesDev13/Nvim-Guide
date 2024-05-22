<!-- Autor: Daniel Benjamin Perez Morales -->
<!-- GitHub: https://github.com/DanielPerezMoralesDev13 -->
<!-- Correo electrónico: danielperezdev@proton.me  -->
# **_Instalación y Uso de Neovim en Linux_**

## _**Instalación**_

> _Para instalar Neovim en Linux, puedes usar el gestor de paquetes de tu distribución. Por ejemplo, en Ubuntu, puedes usar `apt-get`:_

```bash
sudo apt-get update
```

```bash
sudo apt-get install neovim
```

## _**Ejecución**_

_Para ejecutar Neovim, simplemente abre una terminal y escribe `nvim`._

```bash
nvim
```

## _**Ver la versión**_

> _Para ver la versión de Neovim que tienes instalada, puedes usar el comando `:version` dentro de Neovim._

```bash
nvim
:version
```

## _**Escribir en un fichero**_

> _Para escribir en un fichero, primero debes abrirlo con Neovim. Por ejemplo, para abrir un fichero llamado `fichero.py`, usarías el siguiente comando:_

```bash
nvim fichero.py
```

- **Una vez abierto el fichero, puedes empezar a escribir en él. Para entrar en el modo de inserción (donde puedes escribir texto), presiona `i`.**

## _Guardar cambios_

> _Para guardar los cambios que has hecho en un fichero, usa el comando `:w`._

```bash
:w
```

## _**Salir sin guardar cambios**_

> _Si quieres salir de Neovim sin guardar los cambios que has hecho, puedes usar el comando `:q!`._

```bash
:q!
```

## _Salir normalmente_

_Para salir de Neovim normalmente (es decir, cerrar Neovim), puedes usar el comando `:q`._

```bash
:q
```

## _**Comandos abreviados y su significado**_

- **`:w` - Guardar los cambios en el fichero actual.**
- **`:q` - Salir de Neovim.**
- **`:q!` - Salir de Neovim sin guardar los cambios.**
- **`:wq` o `:x` - Guardar los cambios y salir de Neovim.**
- **`i` - Entrar en el modo de inserción.**
- **`ESC` - Salir del modo de inserción.**

## _**Comandos sin abreviar**_

- **`:write` - Guardar los cambios en el fichero actual.**
- **`:quit` - Salir de Neovim.**
- **`:quit!` - Salir de Neovim sin guardar los cambios.**
- **`:writequit` o `:exit` - Guardar los cambios y salir de Neovim.**
- **`:insert` - Entrar en el modo de inserción.**

- **En Neovim y Vim, la tecla `a` se utiliza para entrar en el modo de inserción después del carácter actual. Esto significa que si tienes el cursor en un carácter específico en tu fichero y presionas `a`, podrás comenzar a escribir después de ese carácter.**

- **Es similar a `i` (insertar), pero `i` comienza a insertar antes del carácter actual, mientras que `a` comienza a insertar después del carácter actual.**

- **El comando `:Tutor` inicia una sesión interactiva de tutoría en Neovim. Esta es una excelente manera de aprender los conceptos básicos de Neovim, ya que te guía a través de una serie de lecciones interactivas.**

_Para iniciar el tutor, simplemente abre Neovim y escribe `:Tutor`, luego presiona Enter._

```bash
nvim
:Tutor
```

> _Puedes moverte por las lecciones usando las teclas de navegación y seguir las instrucciones en pantalla._

_El comando `:h vim-modes` en Neovim o Vim abre la ayuda para los diferentes modos en Vim. Vim tiene varios modos, incluyendo el modo normal, el modo de inserción, el modo visual, entre otros._

_Aquí hay una breve descripción de algunos de los modos más comunes:_

- **Modo normal: Este es el modo predeterminado cuando abres Vim. En este modo, puedes ejecutar comandos y moverte por el fichero.**

- **Modo de inserción: En este modo, puedes insertar texto en tu fichero. Puedes entrar en este modo desde el modo normal presionando `i` para insertar texto donde está el cursor, `a` para insertar texto después del cursor, o `o` para abrir una nueva línea después de la línea actual y comenzar a insertar texto allí.**

- **Modo visual: En este modo, puedes seleccionar texto. Puedes entrar en este modo desde el modo normal presionando `v` para la selección de caracteres, `V` para la selección de líneas, o `Ctrl+v` para la selección de bloques.**

- **Modo de comando: En este modo, puedes escribir comandos de línea completa. Puedes entrar en este modo desde el modo normal presionando `:`.**

> _Para obtener más información sobre estos y otros modos en Vim, puedes usar el comando `:h vim-modes` en Vim o Neovim._

- **`Shift + i` (o `I`): Entra en el modo de inserción al inicio de la línea actual.**

- **`Shift + a` (o `A`): Entra en el modo de inserción al final de la línea actual.**

- **`s`: Borra el carácter bajo el cursor y entra en el modo de inserción.**

- **`Shift + o` (o `O`): Abre una nueva línea por encima de la línea actual y entra en el modo de inserción.**

- **`o`: Abre una nueva línea debajo de la línea actual y entra en el modo de inserción.**

> _En NeoVim, puedes deshacer y rehacer cambios utilizando los siguientes comandos:_

- _`u`: Deshace el último cambio. Puedes presionar `u` varias veces para deshacer múltiples cambios._

- _`Ctrl + r`: Rehace el último cambio que se deshizo. Puedes presionar `Ctrl + r` varias veces para rehacer múltiples cambios._

> _Recuerda que estos comandos deben ser ejecutados en el modo normal. Para volver al modo normal desde cualquier otro modo, puedes presionar la tecla `Esc`._

- _**Comandos básicos de NeoVim en el modo visual:**_

_En el modo visual de NeoVim, los comandos que utilizan la tecla `Shift` son los siguientes:_

- _`D` o `Shift + d`: Corta desde la posición actual del cursor hasta el final de la línea._

- _`Y` o `Shift + y`: Copia la línea completa en la que se encuentra el cursor._

- _`p` o `shift + p` o `yy`: puedes pegar el texto que has copiado o cortado utilizando el comando presiona `p` para pegar el texto después del cursor, o `P` para pegar el texto antes del cursor `yy` o `shift + y`. Esto copiará la línea completa, incluyendo el salto de línea al final.._

- _`V` o `Shift + v`: Entra en el modo visual de línea. Selecciona líneas completas._

- _`>` o `Shift + .`: Indenta el texto seleccionado a la derecha._

- _`<` o `Shift + ,`: Indenta el texto seleccionado a la izquierda._

- _`U` o `Shift + u`: Convierte el texto seleccionado a mayúsculas._

- _`gu` puedes convertir el texto seleccionado a minúsculas utilizando el comando `gu`._

- _`G` o `Shift + g`: Mueve el cursor al final del fichero._

- _`gg`, te lleva al inicio del fichero._

- _`A` o `Shift + a`: Entra en el modo de inserción al final de la línea._

- _`I` o `Shift + i`: Entra en el modo de inserción al inicio de la línea._

- _`O` o `Shift + o`: Abre una nueva línea por encima de la línea actual y entra en el modo de inserción._

- _`C` o `Shift + c`: Corta desde la posición actual del cursor hasta el final de la línea y entra en el modo de inserción._

- _`R` o `Shift + r`: Entra en el modo de reemplazo, permitiendo sobrescribir caracteres._

**Recuerda que estos comandos deben ser utilizados después de entrar en el modo visual con `v`, `V` o `ctrl + v`.**

- _`D` o `Shift + d`: Corta desde la posición actual del cursor hasta el final de la línea._

- _`Y` o `Shift + y`: Copia la línea completa en la que se encuentra el cursor._

- _`V` o `Shift + v`: Entra en el modo visual de línea. Selecciona líneas completas._

- _`>` o `Shift + .`: Indenta el texto seleccionado a la derecha._

- _`<` o `Shift + ,`: Indenta el texto seleccionado a la izquierda._

- _`U` o `Shift + u`: Convierte el texto seleccionado a mayúsculas._

- _`G` o `Shift + g`: Mueve el cursor al final del fichero._

- _`A` o `Shift + a`: Entra en el modo de inserción al final de la línea._

- _`I` o `Shift + i`: Entra en el modo de inserción al inicio de la línea._

- _`O` o `Shift + o`: Abre una nueva línea por encima de la línea actual y entra en el modo de inserción._

- _`C` o `Shift + c`: Corta desde la posición actual del cursor hasta el final de la línea y entra en el modo de inserción._

- _`R` o `Shift + r`: Entra en el modo de reemplazo, permitiendo sobrescribir caracteres._

_En NeoVim, existen tres modos visuales: el modo visual normal, el modo visual de línea y el modo visual de bloque._

1. _**Modo visual normal (`v`)**: Permite seleccionar texto carácter por carácter. Puedes moverte con las teclas de dirección para seleccionar texto._

2. _**Modo visual de línea (`V` o `Shift + v`)**: Selecciona líneas completas. Independientemente de dónde esté el cursor en la línea, al presionar `V`, se seleccionará toda la línea._

3. _**Modo visual de bloque (`Ctrl + v`)**: Permite seleccionar bloques de texto. Puedes seleccionar un bloque rectangular de texto en lugar de líneas completas._

_Característica del modo visual de bloque en NeoVim. Cuando seleccionas un bloque de texto y luego entras en el modo de inserción (por ejemplo, presionando I), cualquier texto que escribas se insertará en la misma posición en todas las líneas del bloque seleccionado._

_Después de escribir el texto, debes presionar Esc para salir del modo de inserción. Al principio, puede parecer que el texto solo se ha insertado en la primera línea, pero una vez que presiones Esc, verás que el texto se ha insertado en todas las líneas del bloque seleccionado._

**Comandos:**

- _`Shift + $` en el modo visual seleccionará todo el texto desde la posición actual del cursor hasta el final de la línea._

- _`c` en el modo visual cortará el texto seleccionado y entrará en el modo de inserción, permitiéndote reemplazar el texto seleccionado con lo que escribas a continuación._

- **Las diferencias radican en cómo seleccionan el texto: carácter por carácter, por líneas completas o en bloques rectangulares.**

_Los registros de copia (o "buffers" de copiado) en NeoVim no son los mismos que los del sistema operativo por defecto. NeoVim tiene su propio sistema de registros que es independiente del portapapeles del sistema operativo._

_En la mayoría de las terminales, puedes usar Ctrl + Shift + C para copiar el texto seleccionado al portapapeles del sistema operativo y Ctrl + Shift + V para pegar el contenido del portapapeles del sistema operativo en la terminal._

- **Para entrar en el modo terminal en NeoVim, puedes usar el comando `:terminal`. Esto abrirá una terminal en una nueva ventana de buffer para escribir en la terminal presiona `i`.**

- **Para salir del modo terminal, puedes usar el comando `<Ctrl-\><Ctrl-n>`. Esto te llevará de vuelta al modo normal.**

_El modo Ex en NeoVim es un modo de línea de comandos que te permite ejecutar comandos Ex. Aquí hay algunos comandos útiles:_

- **`:e file.py` o `:edit file.py`: Abre el fichero `file.py` en el buffer actual. Si `file.py` no existe, crea un nuevo fichero con ese nombre.**

- **`:w`: Guarda los cambios en el fichero actual.**

- **`:q`: Cierra el buffer actual. Si hay cambios no guardados, NeoVim te advertirá.**

- **`:wq` o `:x`: Guarda los cambios y cierra el buffer actual.**

- **`:ls` o `:buffers`: Lista todos los buffers abiertos.**

- **`:bn` y `:bp`: Navega a través de los buffers abiertos.**

- **`:split` o `:vsplit`: Divide la ventana en horizontal o vertical respectivamente.**

- **`:help`: Muestra la ayuda de NeoVim.**

_El explorador de ficheros, puedes usar el comando `:Explore` (o `:E` para abreviar) para abrir el explorador de ficheros en el directorio actual. Desde allí, puedes navegar por los directorios y abrir ficheros._

_Por ejemplo, `:E` abrirá el explorador de ficheros, y luego puedes usar las teclas de dirección para navegar, `Enter` para abrir un fichero o directorio, y `-` para subir un nivel de directorio._

- **`Shift + %`: En el explorador de ficheros (`netrw`), este comando no tiene una funcionalidad predeterminada. Sin embargo, en el modo normal, `%` se usa para saltar entre paréntesis, corchetes o llaves coincidentes.**

- **`:r file.py` o `:read file.py`: Lee el contenido del fichero `file.py` e inserta ese contenido en la línea debajo de la posición actual del cursor.**

- **`Ctrl + 6` (en algunos teclados), que cambia al buffer más recientemente usado.**

- **`:bn` y `:bp`: Estos comandos cambian al siguiente (`bn`) y al anterior (`bp`) buffer en la lista de buffers. Sin embargo, puedes agregar números a `:bn` y `:bp` para saltar a buffers específicos. Por ejemplo, `:b2` te llevará al buffer número 2.**

  - _`n` y `p` en el explorador de ficheros (`netrw`): `n` cambia el ordenamiento de los ficheros y `p` va al directorio padre._

- **El comando `:r !ls -la` en NeoVim ejecuta el comando `ls -la` en el shell y luego inserta la salida de ese comando en el archivo en la línea debajo de la posición actual del cursor.**

_Por lo tanto, `:r !ls -la` insertará una lista de todos los archivos en el directorio actual en tu archivo._

- **En `nvim` (NeoVim), puedes usar los siguientes comandos para moverte al principio y al final de una línea:**

- **Para ir al principio de una línea, usa `0` (cero).**
- **Para ir al final de una línea, usa `$`.**
