## 自動販売機（オブジェクト、DOM、イベント処理）のミニレポート
### Q4-1. Itemクラスのメソッドについて説明せよ。
* showItemListがクラスメソッドである理由を考察せよ。
* 処理の内容がshowItemListの外に処理を依頼するのではなく、配列"items"に格納されているデータをコンソールで出力する処理内容のため。
* buyItemがインスタンスメソッドである理由を考察せよ。
* 外からデータを受け取る処理が行われている。そのため、毎回データが変わりその都度データを取得し処理を行うため、インスタンスメソッドにすることでコードの簡略化を行えるから。
* 
### Q4-2. 商品の購入ボタンをクリックすると、どのような処理でセルの値が減少するか説明せよ。
* 購入された商品の在庫数のセルをどのようにして特定するのか説明せよ。
* 課題4-2で作成した商品表出力のコードに"button"idとは別に"stock"idを指定。そのidで在庫表のエレメントを抽出することにより、〇番が購入されたときに、〇番の在庫を読み込むことができた。
* 特定したセルの値をどのように変更するのか説明せよ。
* "this.stock -= 1"で在庫を減らした後、先程抽出した"stock"エレメントを利用し、innerHTMLで"stock"セルを1減らした"this.stock"を指定し、更新することで購入が完了したような仕組みにした。
* 
### Q4-3. 感想
* 今回の課題で苦労したこと
* コンソール上で在庫を削減できても、HTML内の在庫を更新する方法が分からず、苦戦した。
* 演習を通して理解できたこと
* HTMLの、元々のデータを更新することで、今回の応用である。出席プログラムやゲーム性に富んだプログラムを作成できることが分かった。
* この自動販売機プログラムの追加機能や課題など
おつりの返却ボタンと、返却機能。そして新たに在庫を増やす機能。
