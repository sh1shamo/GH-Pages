---
layout: post
title: "【BMW M235i (F22)】コーディング備忘録"
date:   2025-02-11 00:00:00 +0900
categories: car
background: ''
---
備忘録がてら現在のコーディング内容を紹介します。  
  
## 車体  
BMW M235i (F22)  
VIN からデコードした限り、 2015/9 製造らしい。  
  
## i-Step バージョン  
F020-16-03-502  
  
## コーディング内容
<s>Markdown の表すごく見づらい</s>  
  
  
| <small><b>設定内容</b></small> | <small><b>設定箇所</b></small> | <small><b>設定値</b></small> | <small><b>備考</b></small> |
|-------------------------------|-------------------------------|-----------------------------------------|-----------------|
| <small>ASD オフ</small> | <small>1: HU_NBT2 / 3009 EFFICIENT_DYNAMICS / ASD_SOUND_OFF<br/>2: ASD / 3000 ASD-Configuration / Engine<br/>3: ASD / 3000 ASD-Configuration / Model Range</small> | <small>1: aktiv<br/>2: N74B66<br/>3: F001</small> | <small>1 だけではオフにならない様子。 2, 3 は実車と異なる設定であれば何でも良い。</small> |
| <small>GPS 時刻同期</small> | <small>1: HU_NBT2 / 3000 HMI / CLOCK_CHANGE_AUTOMATIC<br/>2: HU_NBT2 / 3000 HMI / SETTINGS_TIME_AUTOMATIC</small> | <small>1: aktiv<br/>2: navigation</small> ||
| <small>iDrive 起動ロゴ M Performance 化</small> | <small>HU_NBT2 / 3001 EXBOX / STARTUP_EMBLEM</small> | <small>variant_01</small> |  |
| <small>アイドリング ストップ デフォルト無効化</small> | <small>FEM_BODY / 3023 TcMaster2 / TCM_MSA_DEFAULT_OFF</small> | <small>aktiv</small> ||
| <small>オーディオ設定変更</small> | <small>HU_NBT2 / 3002 AUDIO_TUNER_TRAFFIC / AUDIO_SYSTEM</small> | <small>individual_sound</small> | <small>ここはお好み。<br/>individual_sound > highpremium > hifi_system_harmankardon の順でドンシャリ度が高いらしく、だいたいこの 3 つのどれかにしている人が多い印象。</small> |
| <small>デイライト (フロント; 眉毛消灯)</small> | <small>1: FEM_BODY / 3060 LceMaster / TFL_MODUS<br/>2: FEM_BODY / 3063 LceLampMapping2 / MAPPING_UNIVERSAL_1_OUTPUT<br/>3: FEM_BODY / 3063 LceLampMapping2 / MAPPING_UNIVERSAL_2_OUTPUT</small> | <small>1: tfl_s<br/>2: off<br/>3: off</small> | <small>1 だけだと眉毛も点灯。</small> |
| <small>デイライト (リア)</small> | <small>1: REM / 3062 LceLampMapping1 / MAPPING_TAGFAHRL_H_L_OUTPUT<br/>2: REM / 3062 LceLampMapping1 / MAPPING_TAGFAHRL_H_R_OUTPUT</small> | <small>1: sl_l<br/>2: sl_r</small> ||
| <small>デイライト メニュー追加</small> | <small>HU_NBT2 / 3000 HMI / DAYDRIVING_LIGHT</small> | <small>standard</small> | <small>iDrive にデイライトのオンオフの項目を追加。</small> |
| <small>デジタル スピード メーター (BC)</small> | <small>KOMBI / 3000 Anzeige_Konfiguration / BC_DIGITAL_V</small> | <small>aktiv</small> ||
| <small>レーン・ディパーチャー・ウォーニング 検知対象拡張</small>   | <small>KAFAS2 / 3020 TLC_CODING / ROAD_EDGE_WARNING_ENABLED</small> | <small>detection_for_grass_edge_and_curb_stone</small> | <small>白線以外に草や縁石にも反応するようになるらしい。</small> |
| <small>レーン・ディパーチャー・ウォーニング 有効化速度</small> | <small>1: KAFAS2 / 3020 TLC_CODING / THRV_AVAI_TLC_HIGH<br/>2: KAFAS2 / 3020 TLC_CODING / THRV_AVAI_TLC_LOW</small> | <small>1: 1E<br/>2: 19</small> | <small>1 を超えると有効になり、 2 を下回ると無効になる。<br/>値はそれぞれ 16 進数表記。 (それぞれ '30' と '25' )</small> |
| <small>ロック時ドアミラー格納</small> | <small>FEM_BODY / 3053 PwMaster / KOMFORT_SCHLIESSEN</small> | <small>00</small> | <small>ドアミラー格納までのホールド時間。リモコン キーとコンフォート アクセスとで若干挙動が異なる。<br/>【リモコン キーによるロック】<br/>'00' (= 0.0 秒) のときホールド不要でドアミラー格納。 '05' (= 0.5 秒) のときは要 0.5 秒ホールド。<br/>【コンフォート アクセスによるロック】<br/>'00' のときも気持ち要ホールド。 '05' のときはリモコン キーと同様。</small> |
| <small>後退時ドアハンドル点灯</small> | <small>FEM_BODY / 3070 LciMaster / OVT_BEI_RUECKFAHRLICHT</small> | <small>aktiv</small> | <small><s>正直見やすくなるとかはない。</s></small> |