## Enregistrement de tes noms d'utilisateur favoris

Tu veux probablement utiliser quelques noms d'utilisateur différents. Ajoute des noms d'utilisateur que tu aimes dans une liste.

--- task ---

Crée une nouvelle liste appelée `noms que j'aime`:

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

La liste apparaîtra sur la scène. Glisse-la à la droite de ton lutin de personne et élargis-le.

![« noms que j'aime » avec redimensionnement en bas à gauche en surbrillance](images/usernames-like-stage.png)

--- /task ---

--- task ---

Ajoute le sprite `Button4` qui ressemble à <span style="color: green;">✔</span>, et fais-le glisser sur la scène à droite de la bulle de parole.

![lutin en tick vert sur la scène à côté des « noms que j'aime »](images/usernames-tick.png)

Tu auras peut-être besoin de déplacer la liste `noms que j'aime` si le sprite `Button4` est en dessous.

--- /task ---

--- task ---

Ajoute du code au lutin de bouton pour que, lorsqu'il est cliqué, le nom d'utilisateur actuel soit ajouté aux `noms que j'aime`.

![lutin de bouton](images/button-sprite.png)

```blocks3
when this sprite clicked
add (nom d'utilisateur :: variables) to [noms que j'aime v]
```

--- /task ---

--- task ---

Teste ton code en cliquant sur le lutin de la personne jusqu'à ce que tu trouves un nom d'utilisateur que tu aimes, puis en cliquant sur le <span style="color: green;">✔</span>.

![liste remplie des « noms que j'aime »](images/usernames-like-list.png)

--- /task ---

--- task ---

Tu peux exporter ta liste de noms d'utilisateurs vers un fichier texte pour les sauvegarder. Fais un clic droit sur les `noms que j'aime` sur la scène, clique sur **Exporter**, et choisis un endroit où enregistrer la liste en tant que fichier.

![menu liste avec option d'exportation en surbrillance](images/usernames-export.png)

Tu as maintenant un fichier de type texte contenant une liste de noms que tu peux ouvrir avec Notepad ou un autre éditeur de texte.

--- /task ---