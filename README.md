## What's this?

msgpack.org の top ページにある，プロジェクトごとのAPIドキュメントを追加する方法について説明します．

## 追加方法

1. 該当する github レポジトリの Description に，```msgpack.org[ProjctName]``` を追加してください．
2. 追加したいドキュメントを，レポジトリの直下の以下のいずれかの名前で配置します．
  * msgpack.org.md
  * README.md
  * README.markdown
  * README.rdoc
  * README.rst
  * README 

msgpack.org に表示される際の優先順位は，```msgpack.org.md``` >```README.md``` > ```README.markdown``` > ```README.rdoc``` > ```README.rst``` > ```README``` です．```README.md``` の他に ```msgpack.org.md``` を配置しておくことで，github レポジトリに表示するドキュメントとは別のドキュメントを配置することができます．
3. しばらく待つと，クローラが巡回して msgpack.org のページが更新され，msgpack.org.md が表示されます．


## チュートリアル

1. msgpack-java の場合: Description に ```msgpack.org[Java]``` と追加します．
2. レポジトリに ```msgpack.org.md```を追加します．
3. しばらく待つと，クローラが巡回して msgpack.org のページが更新されます．

## 仕組み

github.com の description を，[クローラ](https://github.com/msgpack/website/blob/master/update-index.rb)に巡回させることで実現しています．クローラは1時間に1回起動されるため，description を変更してからある程度遅延があります．