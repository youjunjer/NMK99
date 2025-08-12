# NMK99
小霸王有限公司 NMK99開發板

目前出廠版本分為以下三個
1. NMK99v0.5：2023/07開始出廠，數量約5000顆，腳位採用安信可ESP32-S，MicroUSB接口，雙核心，Flash Size 4M/80MHz，內建ov2640接口可拍照，內建WS2812一顆
2. NMK99v1：2025/07開始出廠，數量約5000顆，基本承襲NMK99v0.5，改TypeC接口，以及SH 1.5mm電池接口
3. NMK99v2：2025/07開始出廠，數量約1000顆，基本承襲NMK99v1，Flash Size 8M/40MHz

本次設計的開發板NMK99v2採用ESP32核心，規格如下：

1. 記憶體8M/40Mhz
2. 雙核心(160/240)
3. TypeC接口
4. 支援相機ov2640,3360,5640
5. 38隻GPIO，腳位參閱附圖
6. USB Serial採用CH341驅動，可在這裡下載：https://twgo.io/ch340

Arduino開發板選擇方式，相容ESP32 Dev Module

ESP32 Dev Module，參考以下設定：

  <img width="569" height="436" alt="image" src="https://github.com/user-attachments/assets/00b58f70-aa55-4a2b-9418-58a15c4b6239" />


  1. Flash Frequency：40MHz，Flash記憶體使用40MHz
  2. Flash Size：8MB(64Mb)，Flash記憶體提昇至8MB
  3. Partition Scheme：8M with spiffs(3MB APP/1.5M spiffs)
  4. PSRAM：Enabled，本裝置使用PSRAM，可加快相機效能

