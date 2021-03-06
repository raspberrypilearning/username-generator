## 好きなユーザー名を保存する

ちがうユーザー名をいくつか考えるのも良いでしょう。 好きなユーザー名をリストに追加しましょう。

--- task ---

`好きな名前`という新しいリストを作りましょう。

[[[generic-scratch3-make-list]]]

--- /task ---

--- task ---

リストがステージ上に表示されます。 リストを人物のスプライトの右にドラッグして、はばを広げます。

![左下でハイライト表示されている、サイズをかえた「好きな名前」リスト](images/usernames-like-stage.png)

--- /task ---

--- task ---

<span style="color: green;">✔</span>のような`Button4` (ボタン4) スプライトを追加し、ふきだしの右にドラッグします。

![ステージ上の「好きな名前」リストのとなりにある緑色のチェックマークのスプライト](images/usernames-tick.png)

`Button4`スプライトが`好きな名前`リストの下にある場合は、リストを動かす必要があるかもしれません。

--- /task ---

--- task ---

ボタンのスプライトにコードを追加して、スプライトがクリックされたら、今のユーザー名を`好きな名前`に追加するようにします。

![ボタンのスプライト](images/button-sprite.png)

```blocks3
when this sprite clicked
add (ユーザー名 :: variables) to [好きな名前 v]
```

--- /task ---

--- task ---

好きなユーザー名が出てくるまで人物のスプライトをクリックし、その後に<span style="color: green;">✔</span>をクリックしてコードをテストしましょう。

![ユーザー名が追加された「好きな名前」リスト](images/usernames-like-list.png)

--- /task ---

--- task ---

テキストファイルにエクスポートして、ユーザー名のリストを保存できます。 ステージにある`好きな名前`リストを右クリックして、**書き出し**をクリックし、ファイルとして保存する場所をえらびます。

![「書き出し」オプションがハイライト表示されたリストメニュー](images/usernames-export.png)

メモ帳や他のテキストエディターで開くことができる、ユーザー名のリストをふくむテキストファイルが作成されています。

--- /task ---