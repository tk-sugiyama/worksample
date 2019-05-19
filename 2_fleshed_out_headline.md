# DIVE INTO CODE worksample



# 初めに
本テキストはこれから学ぶ、Railsの概要をイメージするものです。



## Railsとは

Ruby on Rails（ROR）ともいわれる、Webアプリを簡単に作る為の便利なtoolを集めたフレームワークです。  Ruby on Railsの記載からも連想される通り、RubyとRailsの両方の知識を使い作成を行います。
以下サイトがRailsを利用して作成されているホームページです。 
- [Cookpad](https://cookpad.com/)
- [CrowdWorks]( https://crowdworks.jp/)
- [Hulu](https://www.happyon.jp/)
- [食べログ](https://tabelog.com/)

なお、公式なワークフレームパッケージはRubyのライブラリやアプリケーションのRubyGemsにより
配布されています。
　RubyGems：https://github.com/rubygems/rubygems



## Railsの考え方

いくつかある基本理念のうち、覚えてほしい2つの基本理念。

### DRY（Don’t Repeat Yourself：同じことは繰り返さない）

　様々な個所に複数記述せず、1か所に記述することで、変更が生じた際の保守性をさ高めます。

### CoC（Convention over Configuration：設定より規約）
　従来のフレームワークのように設定を大量に記述せず、規約にのっとってプログラミングを行う。
　そうする事で、余計なプログラミングや設定を省くことができます。   
　規約にのっとることで、クラスとテーブルのマッピング等をRailsでは自動的に行います。   
　その為、開発者はクラスとテーブルを関連付ける設定を行う必要がなく、開発者は本来やるべき部分の  
　開発に、注力することができます。



## Railsを利用するメリット

- Rubyという言語自体が書きやすい為、プログラムの処理を覚えることに適しています。
- 日本語での記事が多く、主要な機能は調べながら、すぐに作成できます。
- ルールが細かく決まっている為、ルールに沿って書いていくことで簡単にアプリケーションが作れます。
- ルールが決まっていいる為、少ないコード量で書くことができ、作成時間を短縮できます。



## Railsで利用するMVC

RailsではPCに画面を表示する為に、モデル/ビュー/コントローラと呼ばれるものが出てきます。
モデル/ビュー/コントローラは頭文字を取ってMVCと呼ばれます。

- モデル（Model）：データを扱う部分
- ビュー（View）：ユーザーに見える結果を作る部分
- コントローラ（Controller）：ユーザーからのリクエストを処理し、モデルやビューと連携を行なう部分

![MVC概要](https://github.com/tk-sugiyama/worksample/blob/master/img/MVC.png)



<u>リクエストから画面表示までの一連の流れ</u>

1. 利用者がブラウザ経由で送信したリクエストをWebサーバからURLとして受け取ります。

2. フレームワーク内の「routes.rb」ファイルでどのコントローラのどのアクションを呼び出せばいいのが列挙します。
   ![routes.rbイメージ](https://github.com/tk-sugiyama/worksample/blob/master/img/routes.png)

3. 利用者からのリクエストで呼び出されたアクションは、モデルを介してデータベースとのやり取りを行い、データを取得したり新しいデータを格納したりします。
   ![コントローラとDBの連携イメージ](https://github.com/tk-sugiyama/worksample/blob/master/img/Model.png)

4. 取得したデータをビューにセットし、HTML文書を作成しコントローラへ返します。
   ![このトローラとビューの連携イメージ](https://github.com/tk-sugiyama/worksample/blob/master/img/View.png)

5. コントローラが作成されたHTMLデータを利用者へ返します。
   ![ページ表示イメージ](https://github.com/tk-sugiyama/worksample/blob/master/img/Return.png)

   

## まとめ

Railsの概要を上記のように記載いたしましたが、まとめると、
フレームワークを利用することで、***早く***、***簡単***に、***上質***なWeb開発が可能となります。
