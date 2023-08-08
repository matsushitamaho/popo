---
title: "JS　prompt"
emoji: "📝"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["Javascript","初心者"]
published: false
---
# promptとは？
入力ダイアログのこと。
```js:基本的な書き方(例)
let promptStr = prompt('何か好きな文字を入力してください。');

alert(promptStr);
```
## 複数の関数を定義する
```js:
let user_hand = prompt('じゃんけんの手をグー、チョキ、パーから選んでください。');

alert('あなたの選んだ手は' + user_hand + 'です。');
```
