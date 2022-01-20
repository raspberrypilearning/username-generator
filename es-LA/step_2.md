## Generando nombres de usuario

Hay muchos sitios web y aplicaciones que utilizan un nombre de usuario para identificarte. Este nombre de usuario es frecuentemente visible para otros. Los nombres de usuario también pueden llamarse nombres de pantalla, etiquetas de jugadores o identificadores.

Es importante que tu nombre de usuario no sea tu nombre real y tampoco incluya ninguna información personal como tu edad, tu año de nacimiento o donde vives. Otras personas verán tu nombre de usuario, así que asegúrate de que sea cortés y ten en cuenta lo que las personas pensarán de ti cuando lo lean. Recuerda que podrías estar usando tu nombre de usuario durante mucho tiempo. ¿Aún te gustará dentro de tres años?

Como puedes ver, es importante elegir tu nombre de usuario cuidadosamente. Vamos a crear un proyecto de Scratch para generar nombres de usuario 'SustantivoAdjetivo' como 'IguanaDeDiamante'.

--- task ---

Abre el proyecto inicial de Scratch.

**En línea**: abre el proyecto de inicio en [scratch.mit.edu/projects/408401239](https://scratch.mit.edu/projects/408401239){:target="_blank"}.

Si tienes una cuenta de Scratch, puedes hacer una copia haciendo clic en **Remix**.

**Sin conexión**: abre el [proyecto de iniciación](https://rpf.io/p/es-LA/username-generator-go){:target=_blank"} en el editor sin conexión.

Si necesitas descargar e instalar el editor offline de Scratch, puedes encontrarlo en [rpf.io/scratchoff](https://rpf.io/scratchoff){:target="_blank"}.

Deberías ver dos listas en el escenario — `adjetivos` y `sustantivos`:

![listas con adjetivos y sustantivos](images/usernames-lists.png)

--- /task ---

--- task ---

Haz clic en **Variables**, y luego haz clic en las casillas junto a `adjetivos` y `sustantivos` para desmarcarlas y ocultar las listas.

![variables de adjetivos y sustantivos](images/usernames-hide.png)

--- /task ---

--- task ---

Añade una variable llamada `nombre de usuario` que debería estar disponible **para todos los objetos**.

[[[generic-scratch3-add-variable]]]

--- /task ---

--- task ---

Haz clic en la casilla junto a `nombre de usuario` para desmarcarlo y ocultar la variable del escenario.

![variable nombre de usuario](images/usernames-hide-variable.png)

--- /task ---

--- task ---

Agrega un objeto de una persona — puedes elegir tu favorito.

![objeto persona](images/usernames-person.png)

También puedes hacer clic en **Disfraces** y elige el disfraz que prefieras.

--- /task ---

--- task ---

Agrega este código a tu objeto persona:

![objeto persona](images/person-sprite.png)

```blocks3
when this sprite clicked
set [nombre de usuario v] to []
```

--- /task ---

--- task ---

Necesitas combinar un adjetivo y un sustantivo, así que añade un bloque `unir`{:class="block3operators"} dentro de tu bloque `establecer`{:class="block3variables"}.

![objeto persona](images/person-sprite.png)

```blocks3
when this sprite clicked
set [nombre de usuario v] to (join [apple] [banana] :: +)
```

--- /task ---

--- task ---

Agrega un adjetivo en la primera caja del bloque `unir`{:class="block3operators"}.

![objeto persona](images/person-sprite.png)

```blocks3
when this sprite clicked
set [nombre de usuario v] to (join (item (1) of [adjetivos v] :: +) [banana])
```

--- /task ---

--- task ---

Elige un adjetivo `aleatorio`{:class="block3operators"} entre 1 y la `longitud de la lista de adjetivos`{:class="block3variables"}

![objeto persona](images/person-sprite.png)

```blocks3
when this sprite clicked
set [nombre de usuario v] to (join (item (pick random (1) to (length of [adjetivos v] :: +) :: +) of [adjetivos v]) [banana])
```

--- /task ---

--- task ---

Agrega un sustantivo aleatorio en el segundo cuadro.

![objeto persona](images/person-sprite.png)

```blocks3
when this sprite clicked
set [nombre de usuario v] to (join (item (pick random (1) to (length of [adjetivos v])) of [adjetivos v]) (item (pick random (1) to (length of [nombres v] :: +) :: +) of [nombres v] :: +))
```

--- /task ---

--- task ---

Ahora agrega bloques de código para que tu persona diga el nombre de usuario.

![objeto persona](images/person-sprite.png)

```blocks3
when this sprite clicked
set [nombre de usuario v] to (join (item (pick random (1) to (length of [adjetivos v])) of [adjetivos v]) (item (pick random (1) to (length of [nombres v])) of [nombres v]))
+ say (nombre de usuario :: variables)
```

--- /task ---

--- task ---

Prueba tu código haciendo clic en el objeto de la persona. Deberías obtener un nuevo nombre de usuario aleatorio cada vez.

![objeto persona diciendo CernícaloÁrtico](images/usernames-click.png)

--- /task ---
