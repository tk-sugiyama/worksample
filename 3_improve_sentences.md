# worksample
DIVE INTO CODE worksample  
【担当するIssue】  
「selfについて」説明文が難しかったです。  

selfはインスタンスオブジェクト自身を指しています。
クラスの中でインスタンスオブジェクトを呼び出す際やそのインスタンスオブジェクトを呼び出す際は、selfを使用します。



Selfには2つの利用方法があります。  
<img src="img/Self.png" alt="Selfの使い方" title="Self画像">


## インスタンスオブジェクト内で利用される場合
インスタンスオブジェクト自身を参照します。

## メソッド定義で'Self.メソッド名'を利用する場合
クラスメソッドを定義します。　　
  
例  
`class Dive
  attr_accessor :name

  def instance1(name)
	#instance1 を参照します。
	self　　
  end


  # クラスメソッド
  def self.code
    # この場合のselfの扱いは、Diveクラス
    puts "#{self}クラス"
  end
end

# Diveのオブジェクトを生成。引数を与えます
test = Dive.new("Dive太郎")

# クラスメソッドの呼び出し
Dive.code`