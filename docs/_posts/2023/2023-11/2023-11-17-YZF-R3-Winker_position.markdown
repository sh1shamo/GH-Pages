---
layout: post
title: "【YZF-R3】ウインカーポジションキットを仕込んでみた"
date:   2023-11-17 11:02:00 +0900
categories: motorcycle
background: '/img/img4articles/2023/2023-11/2023-11-17-YZF-R3-Winker_position/DSC_5063-強化-NR.jpg'
---
ウインカーをポジション化すると視認率が上がって事故予防になるという話があります。  
<small>cf. [バイク事故の原因〜雑学編〜 - bike-lineage.org](https://bike-lineage.org/etc/question/traffic_accident_trivia.html)</small>  
  
そんなわけでR3の前に乗っていたセローではウインカーポジションキットを仕込んでいましたが、R3に乗り換えてからはずっとそのままでした。  
  
▼ウインカーポジション化したセローの図
![ウインカーポジション化したセロー](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\serrow-winker_position.jpg){: .img-fluid}  
  
ウインカー自体はだいぶ前にLED化していて、常時点灯させても消費電力的に問題はないはずなので、そろそろ手を出すことにしました。  
<small>cf. LED化したときの話([【YZF-R3】中華の怪レいLEDウインカー - sh1shamo.github.io](https://sh1shamo.github.io/motorcycle/2022/12/31/YZF-R3_LEDBlinker.html)])</small>  
  
## 1: キットの選定
ウインカーポジション化にあたってよく知られる注意点が1つあります。  
詳細は省きますが、ウインカー作動時の反対側のウインカーの状態について、  
**・平成18年(2006年)1月1日以降の車: 消灯を推奨**  
**・平成17年(2005年)12月31日以前の車: 点灯必須**  
と年式によってルールが異なるため、購入するキットを気をつけないといけません。  
<small>cf. [ウインカーポジションは車検に通るの？　それとも違法？　保安基準を分かりやすく解説 - diylabo.jp](https://www.diylabo.jp/basic/basic-124.html)</small>  
  
先代セローで使っていたキットも今でも持っているのですが、このときのセローは2005年式だったので、後者に対応したキットです。対して今乗っているR3は2021年式です。  
  
前述の参考先のサイトには、  
  
>"**反対側については点灯・非点灯どちらでもよいとも取れます**が、IPFとしては反対側は消灯を推奨しています。  
>(中略)  
>**ディーラー等の見解によっては、反対側が消灯でないとNGと判断される場合がある**ためです。"  
  
<small>[ウインカーポジションは車検に通るの？　それとも違法？　保安基準を分かりやすく解説 - diylabo.jp](https://www.diylabo.jp/basic/basic-124.html) より抜粋</small>  
  
とあり、一応流用しても(法的に)問題はないようです。  
ですが、他方実際の現場ではNGになる可能性があるという旨の記載もあったため、今回は新しく平成18年式以降のものに対応したキットを買い直すこととしました。  
<small>(R3は車検もあるしね…。)</small>  
  
ということで早速Amazonを眺めていたのですが、前回セロー用に購入した際は謎の中華メーカのものを1000円台で購入した記憶があるのに対して、今回は同じような中華メーカのものでも2000円以上はするようでした。  
となると、あまり中華メーカのものを買うメリットもないので、3000円程度でIPFのキットを買うことにしました。  
(持っていれば不要ですが)ギボシ端子等も一通りついてきたので、結果的にはこちらの方がお得かもしれません。  
  
▼今回購入したキット  
<a href="https://www.amazon.co.jp/gp/product/B07D97PGYX?ie=UTF8&psc=1&linkCode=li3&tag=sanma0c7-22&linkId=8774de7846ce8524d0b2f8b978d2a06a&language=ja_JP&ref_=as_li_ss_il" target="_blank"><img border="0" src="//ws-fe.amazon-adsystem.com/widgets/q?_encoding=UTF8&ASIN=B07D97PGYX&Format=_SL250_&ID=AsinImage&MarketPlace=JP&ServiceVersion=20070822&WS=1&tag=sanma0c7-22&language=ja_JP" ></a><img src="https://ir-jp.amazon-adsystem.com/e/ir?t=sanma0c7-22&language=ja_JP&l=li3&o=9&a=B07D97PGYX" width="1" height="1" border="0" alt="" style="border:none !important; margin:0px !important;" />  
[IPF ウィンカーポジションキット X2 LEDウィンカー対応 XW-04](https://amzn.to/47A7foA)  
  
## 2: 取り付け準備
まず、車体に取り付ける前の準備をします。  
  
**【必要な工具(ウィンカーポジションキットに関係するもののみ)】**  
・電工ペンチ(ギボシ端子のカシメに使う)  
・ギボシ端子(付属品を使うなら不要)
・結束バンド(ケーブルの余長を束ねる用)  
・リピートタイ(車体配線時の固定用)  
・スリットチューブ(無くても良いがケーブル保護用)  
・電源分岐ハーネス(ギボシ端子タイプ; すでに使用しているACC電源を分岐させて流用する場合のみ)
  
もともと四輪車用の製品のため、配線のうち青と青/黒の配線が異常に長いので、白と白/黒の配線と同じくらいの長さになるよう束ねておきます。  
加えて、これらウインカーに向かう配線については、車体を這わせる際に外に露出するので、雨風の影響で皮膜が劣化しないようにスリットチューブに入れておくと良いです。  
  
また、シート下に収まる赤と黒の配線についても適当な長さで束ねておくと、こちらも収まりが良いです。  
  
その他、今回電源をACC電源(メスのギボシ端子)から取ることにしたので、赤の配線にオスのギボシ端子を取り付けました。  
~~<small>工具箱をあちこち探して見つけたギボシ端子を取り付けてから、キットの付属品にもギボシ端子がついてきていたことに気づいたのは内緒。</small>~~  
  
▼整線後の状態<small>(※赤の配線の先端に付いている電源分岐ハーネスは別途用意したもの)</small>
![整線後の状態](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\preparation_before_attatchment-01.jpg){: .img-fluid}  
  
次にキットの動作モードを「ウインカー作動時に反対側のウインカーが消灯」となるよう変更します。  
説明書にある通り2つあるDIPスイッチのうち、1番のスイッチを下に倒します。  
  
▼DIPスイッチの状態(モード変更後)  
![DIPスイッチの状態(モード変更後)](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\preparation_before_attatchment-02.jpg){: .img-fluid}  
  
これで車体に取り付ける準備ができたので、早速車体に取り付けます。  
  
## 3: 取り付け
といってもウインカーと車体とがギボシ端子で繋がっているのでその間に噛まして、あとはキット用の電源をACC電源から取るだけなので至極シンプルです。  
まず、配線別接続先は以下の通りです。ウインカーに向かう配線については左右の区別は無さそうなのでお好きな方をどうぞ。  
  
▼配線接続図  
![配線接続図](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\winker_position-wiring.png){: .img-fluid}  
  
**1: リアシート・シート・サイドカバー・メータ両脇のカバーを外す。**  
  
▼メータ両脇のカバーを外すとフロントウインカーのギボシ端子にアクセスできる  
![メータ両脇のカバー](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\front_winkers.jpg){: .img-fluid}  
  
**2: 次にキットの赤配線とACC電源を接続する。(今回は元々ヒューズボックスから電源を取り出していたのでこれを分岐させて流用。)**  
  
▼ACC電源と接続した図
![ACC電源と接続した図](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\acc_power-wiring.png){: .img-fluid}  
  
**3: 青と青/黒(反対は白と白/黒)の配線をウインカーの方まで配線する。** 
  
▼サイドカウルの下を這わせる  
![ウインカー配線その1](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\winker_wiring-1.png){: .img-fluid}  
  
**4: ウインカーの+極のギボシ(純正の場合、右側は緑色/左側は茶色)を外し、キットの青と青/黒(反対は白と白/黒)の配線を繋ぐ。**  
  
▼純正の配線の間にキットの配線を噛ませる  
![ウインカー配線その2](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\winker_wiring-2.png){: .img-fluid}  

**5: 黒の配線をバッテリのマイナス極につなぎ、キット本体をシート下に格納する**  
  
▼ECUの下にスペースがあったのでそこに収めた  
![キット格納先](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\kit_under_ecu.png){: .img-fluid}  
  
## 4: 完成図
![完成図](\img\img4articles\2023\2023-11\2023-11-17-YZF-R3-Winker_position\DSC_5063-強化-NR.jpg){: .img-fluid}  
  
<blockquote class="twitter-tweet"><p lang="ja" dir="ltr">休みの日まで待てなかったから、仕事終わりに取り付けてそのままひとっ走り行ってきた。 うーん、やっぱウインカーポジション良い。<a href="https://twitter.com/hashtag/YZFR3?src=hash&amp;ref_src=twsrc%5Etfw">#YZFR3</a> <a href="https://twitter.com/hashtag/%E3%82%A6%E3%82%A4%E3%83%B3%E3%82%AB%E3%83%BC%E3%83%9D%E3%82%B8%E3%82%B7%E3%83%A7%E3%83%B3?src=hash&amp;ref_src=twsrc%5Etfw">#ウインカーポジション</a> <a href="https://twitter.com/hashtag/%E3%83%90%E3%82%A4%E3%82%AF?src=hash&amp;ref_src=twsrc%5Etfw">#バイク</a> <a href="https://t.co/OcrqueVLyw">https://t.co/OcrqueVLyw</a> <a href="https://t.co/xN2bqdbKYr">pic.twitter.com/xN2bqdbKYr</a></p>&mdash; ししゃも (@sh15ham0) <a href="https://twitter.com/sh15ham0/status/1724454133258973412?ref_src=twsrc%5Etfw">November 14, 2023</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>  
  
安全性云々抜きにしてもウインカーポジションは良い。  
ではまた。  
  
-------------------
P.S. なんとなくメーカはわざわざ目立たない場所にウインカーを配置していそうなのに、それをわざわざ光らせるのはなかなか冒涜的な気がしないでもない…。  
