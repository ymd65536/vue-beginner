# はじめに

利用している JS  
[jsdeliver](https://www.jsdelivr.com/)

[HelloVue.js](https://ymd65536.github.io/vue/hello_vue/)  
[todo 管理](https://ymd65536.github.io/vue/todo_manage/)  
[bitcoin 表示](https://ymd65536.github.io/vue/bitcoin/)

## ざっくりと

## 注意事項

## よくあるエラー

## はじめの一歩

## Vue.js を使うには

Vue.js を扱うためのインスタンス、Vue インスタンスが必要

## インスタンスのプロパティ

### 書き方の例

```javascript
var app = new Vue({
  el: "#app",
  data: {
    bpi: null,
    hasError: false,
    loading: true,
  },
  methods: {
    hello: function () {},
  },
  mounted: function () {},
  filters: {},
});
```

### el

Vue.js を適用するタグを指定するプロパティのこと

### data

Vue.js 上で扱う変数を定義するプロパティのこと

### methods

Vue.js 上で扱う関数を定義するプロパティのこと  
※s をつけ忘れない！！

### mounted

インスタンスの el オプションにマウントされたときに実行されるプロパティのこと  
※タグに Vue.js が適用された瞬間

### ディレクティブ

> ディレクティブとは  
> コンピュータプログラムのソースコードに記述される要素の一つで  
> そのコードを解釈・変換するソフトウェア（コンパイラやプリプロセッサなど）への  
> 指示や指定などを与えるためのもの。

要するに命令文の一種と捉えておけば OK  
HTML ならばドックタイプに相当する。

Vue.js では v-～始まるディレクティブをタグの属性として付与することで  
Vue による操作が可能になる。

## ディレクティブの種類

### v-bind

任意のタグに属性を付与する。

### v-if

任意のタグに対して表示非表示の条件をつける。  
タグを挿入しない。たくさん入れると遅くなる。

### v-show

任意のタグに対して表示非表示の条件をつける。  
CSS を適用する。
**_ポイント_**

### v-for

ざっくり言えば、VueJ.js におけるループ文  
foreach 的な使い方をする場合は値,キーという順で書く。  
rate が値、currency がキーの時は以下のように書く。

```javascript

  <li v-for="(rate,currency ) in bpi">
    {{ currency }} : {{ rate.rate_float | curencyDecimal}}
  </li>

```

### v-on

## マスタッシュ構文

別名：口ひげ構文

Vue.js では変数展開時に用いる。

```javascript
{
  {
  }
}
```

## 具体的な手順

## テンプレート構文
