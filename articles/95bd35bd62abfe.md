---
title: "JS　変数宣言"
emoji: "📝"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["JavaScript","初心者"]
published: true
---
# 変数宣言の種類
以下の3つの変数宣言キーワードが存在する
- var
- let
- const

## varの特徴
- 古くから変数宣言に用いられていたキーワード。
意図しない動作を生み出しやすいことが懸念された。
- 初期値無しの変数宣言が可能。
- 変数への値の再代入が可能。
- 同じ変数名を再定義してもエラーにならない。
```js:定義方法
var 変数名;
var 変数名 = 初期値;
```

```js:
var title = "JavaScript入門";
var title = "JavaScript初級";// 変数titleの値は「JavaScript初級」へと上書きされる

var title = "JavaScript入門";
var title;                    // この時点では「JavaScript入門」のまま
var title = "JavaScript初級"; // 変数titleの値は「JavaScript初級」へと上書きされる
```

## letの特徴
- 初期値無しの変数宣言が可能。
- 同じ変数名を複数定義しようとすると構文エラーとなる。
- 変数が参照する値を変化させたい場合など、変数への再代入が必要な場合はletを利用する
```js:定義方法
let 変数名;
let 変数名 = 初期値;
```

```js:
let title = "JavaScript入門";
title = "JavaScript初級";     // 「JavaScript入門」から「JavaScript初級」へ値を再代入
```

## constの特徴
- 初期値は必須。
- constで宣言された変数には再代入できない。
- 同じ変数名を複数定義しようとすると構文エラーとなる。
- 変数に対して値を再代入する必要がない場合は、constが推奨されている。
```js:定義方法
const 変数名 = 初期値;
const title = "JavaScript入門"
```