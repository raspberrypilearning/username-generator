## حفظ أسماء المستخدمين المفضلة لديك

ربما تريد التفكير في بعض أسماء المستخدمين المختلفة. دعونا نضيف أسماء المستخدمين التي تحبها إلى قائمة.

\--- task \---

قم بإنشاء قائمة جديدة تسمى `اسماء احبها `:

[[[generic-scratch3-make-list]]]

\--- /task \---

\--- task \---

ستظهر القائمة على المسرح. قم بسحبها إلى يمين الكائن الخاص بك واجعل عرضها أوسع.

![قائمة اسماء احبها مع تغيير الحجم في أسفل اليسار](images/usernames-like-stage.png)

\--- /task \---

\--- task \---

أضف كائن الزر ` Button4 `، والذي يبدو بالشكل <span style="color: green;"> ✔ </span> ، واسحبه عبر الجزء الرئيسي إلى يمين فقاعة الكلام.

![كائن علامة خضراء على المسرح بجوار قائمة اسماء احبها](images/usernames-tick.png)

قد تحتاج إلى نقل قائمة `اسماء احبها ` إذا كان الكائن ` Button4 ` تحتها.

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