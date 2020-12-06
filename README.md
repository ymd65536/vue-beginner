# はじめに

利用しているJS  
[jsdeliver](https://www.jsdelivr.com/)

[HelloVue.js](https://ymd65536.github.io/vue/hello_vue/)  
[todo管理](https://ymd65536.github.io/vue/todo_manage/)  
[bitcoin表示](https://ymd65536.github.io/vue/bitcoin/)  


## ざっくりと

## 注意事項

## よくあるエラー

# はじめの一歩

## Vue.jsを使うには
Vue.jsを扱うためのインスタンス、Vueインスタンスが必要

# インスタンスのプロパティ

## 書き方の例

``` javascript

var app = new Vue({
  el: '#app',
  data: {
    bpi: null,
    hasError: false,
    loading: true
  },
  methods : {
    hello : function(){

    }
  },
  mounted: function () {

  },
  filters: {

  }
})

```

## el
Vue.jsを適用するタグを指定するプロパティのこと  

## data
Vue.js上で扱う変数を定義するプロパティのこと

## methods
Vue.js上で扱う関数を定義するプロパティのこと  
※sをつけ忘れない！！

## mounted
インスタンスのelオプションにマウントされたときに実行されるプロパティのこと  
※タグにVue.jsが適用された瞬間

# ディレクティブ

> ディレクティブとは  
> コンピュータプログラムのソースコードに記述される要素の一つで  
> そのコードを解釈・変換するソフトウェア（コンパイラやプリプロセッサなど）への    
> 指示や指定などを与えるためのもの。  

要するに命令文の一種と捉えておけば OK    
HTML ならばドックタイプに相当する。  

Vue.jsではv-～始まるディレクティブをタグの属性として付与することで  
Vueによる操作が可能になる。

# ディレクティブの種類

## v-bind
任意のタグに属性を付与する。

## v-if
任意のタグに対して表示非表示の条件をつける。  
タグを挿入しない。たくさん入れると遅くなる。  

## v-show
任意のタグに対して表示非表示の条件をつける。  
CSSを適用する。
***ポイント***  

## v-for
ざっくり言えば、VueJ.jsにおけるループ文  
foreach的な使い方をする場合は値,キーという順で書く。  
rateが値、currencyがキーの時は以下のように書く。

``` javascript

  <li v-for="(rate,currency ) in bpi">
    {{ currency }} : {{ rate.rate_float | curencyDecimal}}
  </li>

```

## v-on

# マスタッシュ構文
別名：口ひげ構文

Vue.jsでは変数展開時に用いる。

```javascript

{{}}  

```

# 具体的な手順

# テンプレート構文
