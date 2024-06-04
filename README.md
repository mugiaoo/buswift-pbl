
# swift2022a
##コードディング規約
[参考URL](https://trinitas.tech/2021/02/03/1007/)<br>

1　関数の命名<br>
　　キャメルケースを用いる　＝　小文字で始め、単語の区切りで大文字を使う<br>
　　(例)　バスの運行時刻をprintする関数　＝＞　busTimePrint　<br>
　　命名時の使用する単語は基本的に英語（止むを得ない場合は相談）<br>
  
2　変数の命名<br>
　　キャメルケースを用いる<br>
　　変数には関係のある英単語を使用する（止むを得ない場合は相談）<br>
　　関係のない変数は基本使わない（i,j,k,x,y,z等）<br>

3　定数の命名<br>
　　基本的にグローバル定数は全て大文字で宣言する<br>
　　その他の定数ではキャメルケースを用いる<br>

4　Swiftファイルの命名<br>
　　大文字で始め、単語の区切りで大文字を使う<br>
　　（例）　firebaseのデータを引っ張ってくる　＝＞　FireBaseData<br>

5　インデント<br>
　　インデントはXcodeのデフォルト規則に依存<br>
　　⌘Aで全選択し、Ctrl+iで自動整形を定期的に実行し整頓する<br>

6　コメントアウト、コメントによる説明<br>
　　基本的に変数の宣言時や構造体などについて説明を載せる<br>
　　関数の場合は、引数で何を受け取り、返り値で何を返すのかを説明<br>
```swift
    /*関数名：abcd
      引数：〇〇〇〇
      返り値：〇〇〇〇*/
```    
　　また、返り値がない場合は何を行う処理なのかを説明<br>
　　変数や構造体やクラスの説明　＝　1行コメントアウト　＝　//説明内容<br>
　　関数の説明　＝　ブロックコメントアウト　＝　/* 説明内容 */<br>
　　コメントアウトしたコードはGithubにpushするときには消去する（不要なコードを残さない）<br>

7　if文<br>
　　今回の開発では厳密なルールを定めない<br>
　　1つ値に対して複数のif文により条件を分岐させる際は、swich文を用いると良い<br>
　　if文の条件が長くなりすぎるときは、正規表現を利用すると良い（詳しくは「Swift　正規表現」で検索）<br>

8　ループ（for文、while文）<br>
　　今回の開発では厳密なルールを定めないため、どちらでも可<br>
　　参考程度にwhileを利用するときはbreakやcontinueをよく活用すること<br>
　　無限ループのときはwhileを利用すると良い<br>

9　定数<br>
　　if文などで何度も同じ文字列を使わず、グローバル定数化して保守性を上げよう<br>
　　これを行うことによって、修正箇所が出た際に作業が減る<br>

10　その他コードスタイル例<br>
　　返り値がない場合はVoid表記入りません<br>

```swift
    // Bad
    func update() -> Void {
    }
    // Good
    func update() {
    }
```
  「{」位置は開始行、「}」は改行して最終行へ<br>

```swift
    // Bad
    func update() 
    {
    }
    // Good
    func update() {
    }
```
```swift
    //追記分
```
```swift
    //追記分
```
```swift
    //追記分
```
```swift
    //追記分
```

11　StoryboardとViewController<br>
　　storyboard = 大文字で始め、単語の区切りで大文字を使う(基本的に英語を推奨するが、相談次第では日本語でも可)<br>
　　ViewController = Storyboard名＋ViewController<br>
  
12　ブランチ名<br>
　　＜タスクラベル例＞<br>
　　フロントエンド作業 = front<br>
　　バックエンド作業 = back<br>
　　GTFSに関する作業 = gtfs , GTFS<br>
　　その他にも作業内容も意味がわかるように適宜つける基本英語（日本語のローマ字でも仕方ない時はある）<br>
  
　　＜作業内容例＞<br>
　　HOME画面の修正、実装 = home, Home<br>
　　一覧画面の実装 = itiran, Itiran<br>
　　詳細画面の実装 = detail, Detail<br>
　　その他にも作業内容も意味がわかるように適宜つける基本英語（日本語のローマ字でも仕方ない時はある）<br>
  
　　ブランチ名は、"タスクラベル"-"作業内容"_"作業者名字"とする。<br>
　　（タスクと作業の間はハイフン繋ぎ）<br>
　　例：front-JsonPrint_name<br>
  
13　追記分<br>
14　追記分<br>
15　追記分<br>
    

##すうぃふと2022 交通支援グループ