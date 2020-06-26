## Guardando tus nombres de usuario favoritos

Probablemente quieras considerar algunos nombres de usuario diferentes. Agreguemos los nombres de usuario que te gusten a una lista.

\--- task \---

Crear una nueva lista llamada ` nombres que me gustan`:

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

La lista aparecerá en el escenario. Arrástrala a la derecha del objeto de tu persona y hazla más amplio.

![names I like list with resize in bottom left highlighted](images/usernames-like-stage.png)

\--- /task \---

\--- task \---

Añade el objeto `Botón4`, que parece <span style="color: green;">✔</span>, y arrástralo a la derecha de la burbuja de voz.

![green tick sprite on the stage next to the names I like list](images/usernames-tick.png)

You may need to move the `names I like` list if the `Button4` sprite is underneath it.

\--- /task \---

\--- task \---

Add code to the button sprite so that when it is clicked, the current username is added to `names I like`.

![button sprite](images/button-sprite.png)

```blocks3
when this sprite clicked
add (username :: variables) to [names I like v]
```

\--- /task \---

\--- task \---

Test your code by clicking on the person sprite until you find a username you like and then clicking the <span style="color: green;">✔</span>.

![names i like list populated](images/usernames-like-list.png)

\--- /task \---

\--- task \---

You can export your list of usernames to a text file to save them. Right-click on the `names I like` list on the stage, click **Export**, and choose a place to save the list as a file.

![list menu with export option highlighted](images/usernames-export.png)

You now have a text file containing a list of names that you can open with Notepad or another text editor.

\--- /task \---