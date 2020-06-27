## チャレンジ: 数字を追加する

人気のあるウェブサイトやアプリでは、他のユーザーがまだ使っていないユーザー名を見つけるのがむつかしいことがあります。 あるいは、あるサイトで使っているユーザー名が他のサイトですでに使われていることに気づくかもしれません。 To get around that, you could add a number to the end of your username. **Remember not to use your age, birth date, or birth year.**

Can you use the following blocks to generate usernames with a random number at the end?

```blocks3
set [username v] to [0]

join [hello] [world]

username :: variables

pick random (20) to (99)
```

New usernames you generate should now have numbers at the end:

![screenshot](images/usernames-with-numbers.png)