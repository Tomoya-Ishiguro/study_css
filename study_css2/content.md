学んだこと

クラスによる指定
.から始まる

idによる指定　
＃から始まる

idとclassの違いは？
idには空白を含んではならない

基本的にclassを使う。

＊　ユニバーサルセレクター
全ての要素にスタイルの適応
article *　のように、何かに合わせて使うことが多い

<a href=""></a>
a [href="部分文字列一致"] {
	color: red;
}

$ 

疑似クラス
p:firs-of-type
p:first-child

nth-of-type
article p:not(:first-of-type)

first-letter

結合子
article p

子孫結合子
main article h1
過剰に長くすると可読性が損なわれるので子孫要素をあまり作らない。


子結合子
main > h1 
main直下

隣接兄弟結合子
article p:not(:first-of-type)
article p + p{
	
}
二番目の要素からスタイルを適応させたい場合に使う。


一般兄弟結合子
　article h1~p{
}

セレクターはこの他にもたくさんある。
必要な時にその都度調べて実装する。