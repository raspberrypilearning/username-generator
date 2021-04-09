## Desafío: añadir un número

En sitios web y aplicaciones populares, puede ser muy difícil encontrar un nombre de usuario que otra persona no esté usando. O puede ocurrir que el nombre de usuario que usas en un sitio ya está cojido en otros sitios. Para evitar esto, puedes agregar un número al final de tu nombre de usuario. **Recuerda no usar tu edad, fecha o año de nacimiento.**

¿Puedes usar los siguientes bloques para generar nombres de usuario con un número aleatorio al final?

```blocks3
set [username v] to [0]

join [hello] [world]

username :: variables

pick random (20) to (99)
```

Los nuevos nombres de usuario que generes ahora deberían tener números al final:

![captura de pantalla](images/usernames-with-numbers.png)