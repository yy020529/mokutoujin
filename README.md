# rpi-rgb-led-matrix
hzeller ドライバーを使用して RGB LED マトリックス パネルでアニメーション シーケンスを再生する 。
raspberry pi で hzeller のドライバーを使用して(https://github.com/hzeller/rpi-rgb-led-matrix) 、rgb-led-matrix でアニメーションを再生します。
# ノート
rgb-led-matrix を初めて使用する場合は、非常に詳細な hzeller コンテンツを参照できます。
# 部品
・RGB-Matrix-P3-64x32

・raspberry pi （4 Model B）＜--·[テストしたモデル]
# 配線
![image](https://user-images.githubusercontent.com/117965518/201274313-14cf2018-9bbc-4c35-b5e2-65dd3f79b187.png)
![image](https://user-images.githubusercontent.com/117965518/201274588-182289b7-def1-45bf-9c60-9d4ffec7659e.png)
| rgb-led-matrix  | raspberry pi | raspberry pi  | rgb-led-matrix |
| ------------- | ------------- | ------------- | ------------- |
| R1  | 23  | 13  | G1  |
| B1  | 26  | 6  | GND  |
| R2  | 24  | 21  | G2  |
| B2  | 19  | 10  | E  |
| A  | 15  | 16  | B  |
| C  | 18  | 22  | D  |
| CLK  | 11  | 7  | LAT/STB  |
| OE  | 12  | 9  | GND  |

この配線方法以外にも接続方法がありますので、詳しくはこちら(https://github.com/hzeller/rpi-rgb-led-matrix/blob/master/wiring.md) をご参照ください。

# hzeler ドライバーをインストール
デモを実行して、デバイスが機能するかどうかを確認します。
