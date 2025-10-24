# nilo-pr（Pixel Representation）
## "視覚構造を自然言語的に表現する、GUIの座標・形状・スタイルに特化した言語、エンジン”
niloのための生成AIに正確なGUIを認識させることに特化した曖昧な言語。
prファイルの拡張子は.nlpr
## prエンジンとは？
自然言語に近い、ピクセル単位で正確なGUIを表現することに特化した言語を生成するための独自のエンジン。
niloフレームワークのStencilとレンダラの中間に存在し、軽量で高速。

## なにができる？
AIに画像を使用せずに現在のレンダリング結果を共有することができる。
mcpサーバーとして使用することでシームレスに共有可能。
これまでのフレームワークよりもUIの指示をしやすく。

## 仕様上できないこと
* prファイルをstencilに変換、もしくは描画すること。
    * prファイルはあくまで生成AIに結果を共有することに特化していて、変換などは向かない。

## 構文の構想
screen 1280x720 dark gray

rect at 0,0 size 1280x64 gradient blue to dark blue
text "Dashboard" near 20,22 white size 22 bold
circle center 640,360 radius 120 fill light gray
rect at 980,20 size 100x36 color #333 text white "Sign out"
triangle points (200,500), (400,500), (300,300) fill orange

## 開発
@kamedaga[https://github.com/kamedaga/]
