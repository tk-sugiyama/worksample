# worksample
`self`には<u>**2つの利用方法**</u>があります。  
[![Selfの使い方](https://github.com/tk-sugiyama/worksample/raw/master/img/Self.png)](https://github.com/tk-sugiyama/worksample/blob/master/img/Self.png)

**インスタンスオブジェクト内**で利用される場合、<u>インスタンスオブジェクト自身を参照</u>します。

**メソッド定義**で`Self.メソッド名`で利用する場合、<u>クラスメソッドを定義</u>します。　　

記載例 

```
class Dive
  attr_accessor :name

#instance1 を参照します。
  def instance1(name)
self　　
  end
  
#クラスメソッド
  def self.code
  
#この場合のselfの扱いは、Diveクラス
    puts "#{self}クラス"
  end
end

#Diveのオブジェクトを生成。引数を与えます
test = Dive.new("Dive太郎")

#クラスメソッドの呼び出し
Dive.code
```



