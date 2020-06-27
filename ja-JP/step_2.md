## ユーザー名の生成

ユーザー名を使って個人を特定 (とくてい) するウェブサイトやアプリはたくさんあります。 このユーザー名は他の人にも見えることが多いです。 ユーザー名はスクリーン名、ゲーマータグ、ハンドルネームともいいます。

ユーザー名が本名ではないこと、そして自分の年や誕生日 (たんじょうび)、住所といった個人情報をふくんでいないことが大切です。 あなたのユーザー名を他の人が見ることになるので、しつれいな名前でないかをたしかめましょう。そして、他の人があなたのユーザー名を読んだときにどう思うかを考えましょう。 ユーザー名は長い間使うかもしれないことをわすれないでください。3年たってもそのユーザー名を好きでいられますか？

このように、ユーザー名はしんちょうにえらぶことが大切です。 「ダイヤでできたイグアナ」（DiamondIguana）のような「形容詞 (けいようし)＋名詞 (めいし) 」のユーザー名を生成する Scratch プロジェクトをつくりましょう。

\--- task \---

基本（きほん）の Scratch プロジェクトを開きます。

**オンライン**: [rpf.io/usernameon](http://rpf.io/usernameon){:target="_blank"}から基本のプロジェクトを開きます。

Scratch アカウントを持っている場合は、**リミックス**ボタンをクリックしてプロジェクトをコピーできます。

**オフライン**: オフラインエディターで[基本のプロジェクト](http://rpf.io/p/en/username-generator-go){:target="_blank"}を開きます。

[rpf.io/scratchoff](http://rpf.io/scratchoff){:target="_blank"}から Scratch オフラインエディターをダウンロードしてインストールできます。

ステージ上に2つのリスト（`形容詞`と`名詞`）があります。

![形容詞と名詞のリスト](images/usernames-lists.png)

\--- /task \---

\--- task \---

**変数** (へんすう) をクリックして、`形容詞`と`名詞`の横にあるチェックボックスをクリックしてチェックを外し、リストを表示 (ひょうじ) しないようにします。

![形容詞と名詞の変数](images/usernames-hide.png)

\--- /task \---

\--- task \---

**すべてのスプライトで**使えるように`ユーザー名`という名前の変数を追加します。

[[[generic-scratch3-add-variable]]]

\--- /task \---

\--- task \---

`ユーザー名`の横にあるチェックボックスをクリックし、チェックを外してステージに変数を表示しないようにします。

![ユーザー名の変数](images/usernames-hide-variable.png)

\--- /task \---

\--- task \---

人物のスプライトを追加しましょう。好きなものをえらんでかまいません。

![人物のスプライト](images/usernames-person.png)

**コスチューム**をクリックして好きなコスチュームもえらべます。

\--- /task \---

\--- task \---

人物のスプライトにこのコードを追加しましょう。

![人物のスプライト](images/person-sprite.png)

```blocks3
when this sprite clicked
set [username v] to []
```

\--- /task \---

\--- task \---

形容詞と名詞をつなげる必要があるので、`〜にする`{:class="block3variables"}ブロックに`〜と〜`{:class="block3operators"}ブロックを追加します。

![人物のスプライト](images/person-sprite.png)

```blocks3
when this sprite clicked
set [username v] to (join [apple] [banana] :: +)
```

\--- /task \---

\--- task \---

Add an adjective in the first box in the `join`{:class="block3operators"} block.

![person sprite](images/person-sprite.png)

```blocks3
when this sprite clicked
set [username v] to (join (item (1) of [adjectives v] :: +) [banana])
```

\--- /task \---

\--- task \---

Pick a `random`{:class="block3operators"} adjective between 1 and the `length of the adjectives list`{:class="block3variables"}

![person sprite](images/person-sprite.png)

```blocks3
when this sprite clicked
set [username v] to (join (item (pick random (1) to (length of [adjectives v] :: +) :: +) of [adjectives v]) [banana])
```

\--- /task \---

\--- task \---

Add a random noun in the second box.

![person sprite](images/person-sprite.png)

```blocks3
when this sprite clicked
set [username v] to (join (item (pick random (1) to (length of [adjectives v])) of [adjectives v]) (item (pick random (1) to (length of [nouns v] :: +) :: +) of [nouns v] :: +))
```

\--- /task \---

\--- task \---

Now add code blocks to get your person to say the username.

![person sprite](images/person-sprite.png)

```blocks3
when this sprite clicked
set [username v] to (join (item (pick random (1) to (length of [adjectives v])) of [adjectives v]) (item (pick random (1) to (length of [nouns v])) of [nouns v]))
+ say (username :: variables)
```

\--- /task \---

\--- task \---

Test your code by clicking on the person sprite. You should get a new random username each time.

![person sprite saying Arctic Kestrel](images/usernames-click.png)

\--- /task \---