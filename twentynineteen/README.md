# ■ Wordpressのインストール
wordpress ローカル環境構築ツール - 「LocalbyFlywheel」 

公式サイト - https://localwp.com/  
使い方 - https://bazubu.com/local-by-flywheel-33920.html

# ■ twentynineteen テーマの場所
\wp-content\themes\twentynineteen

![image](https://user-images.githubusercontent.com/64624465/101326889-43099380-38b1-11eb-9513-876ac9e9fb88.png)
# ■ 子テーマの作成
直接style.cssを修正すればデザインは変わりますがテーマがアップデートされると消えてしまいます。  
子テーマを作成してアップデートに影響のないようにします。 

子テーマの作り方 - https://2019tn.plu-plu.net/childtheme/

# ■ Node.jsのインストール
https://techacademy.jp/magazine/16050

# ■ npm install 実行
まずはパッケージをインストールします。
```
cd \wp-content\themes\twentynineteen
npm install
```
# ■ sassファイルの修正
対象ファイルは \wp-content\themes\twentynineteen\sass の配下のファイルになります。

# ■ コンパイルコマンド実行
下記のコマンドでstyle.cssが更新されます。  
※使用コンパイラーは node-sass です。
```
cd \wp-content\themes\twentynineteen
npm run build
```
# ■ 他のコマンド
```
# style.cssのみ更新
npm run build:style

# style-editor.cssみを更新
npm run build:style-editor

# style-editor-customizer.cssのみ更新
npm run build:style-editor-customizer

# style-rtl.cssのみ更新
npm run build:rtl

# print.cssのみ更新
npm run build:print

# 上記全てのcssファイル更新
npm run build

# 変更を監視し自動的に再コンパイルする
npm run watch
```