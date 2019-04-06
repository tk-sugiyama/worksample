# worksample
DIVE INTO CODE worksample




# 初めに
本テキストはこれから学ぶ、Railsの概要をイメージするものです。

## Railsとは
Ruby on Rails（ROR）ともいわれる、Webアプリを簡単に作る為の便利なtoolを集めたフレームワークです。  
Ruby on Rails（ROR）の記載からも連想される通り、RubyとRailsの両方の知識を使います。  
公式なワークフレームパッケージはRubyのライブラリやアプリケーションのRubyGemsにより配布されています。  
　RubyGems：https://github.com/rubygems/rubygems

## Railsの考え方
いくつかある基本理念のうち、覚えてほしい2つの基本理念。

### DRY（Don’t Repeat Yourself：同じことは繰り返さない）
様々な個所に複数記述せず、1か所に記述することで、変更が生じた際の保守性をさ高めます。
 
### CoC（Convention over Configuration：設定より規約）
従来のフレームワークのように設定を大量に記述せず、規約にのっとってプログラミングを行う。  
そうする事で、余計なプログラミングや設定を省くことができます。  
規約にのっとることで、クラスとテーブルのマッピング等をRailsでは自動的に行います。  
その為、開発者はクラスとテーブルを関連付ける設定を行う必要がなく、開発者は本来やるべき部分の開発に、  
注力することができます。