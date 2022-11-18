# 使用方法
アニメーション GIF を含むあらゆる種類の画像形式を読み取ります。

## インストール
最初に led-image-viewer に GraphicsMagick のインストールが必要です。インストール後、make led-image-viewer を使用できます。
````
sudo apt-get update
sudo apt-get install libgraphicsmagick++-dev libwebp-dev -y
make led-image-viewer
````

## 注意点
### GPIO速度
gif 画像形式を使用すると、LED に表示されるアニメーションは画像と同じ速度ではない場合があります。
````
--led-slowdown-gpio=（1-···）
````
減速したい速度を（）内に入力してください。
### サイズ
````
--led-rows=（rows）
--led-cols=（cols）
````
--led-rows=(rows) および --led-cols=(cols) で使用される LED のサイズを入力する必要があるタイプは異なります。

たとえば、64x32 LEDを使用している場合は、フラグ --led-cols=64 --led-rows=32を指定する必要があります。


## 例
````
sudo ./led-image-viewer （.bmp，.jpg，.png，.gif）
sudo ./led-image-viewer --led-rows= 32 --led-cols=64 --led-slowdown-gpio=200 （.bmp，.jpg，.png，.gif）
````
再生したい画像ファイルを入力してください。
