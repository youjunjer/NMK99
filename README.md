# NMK99
小霸王有限公司 NMK99開發板

本次設計的開發板NMK99v2採用ESP32核心，規格如下：

1. 記憶體8M/40Mhz
2. 雙核心(160/240)
3. TypeC接口
4. 支援相機ov2640,3360,5640
5. 38隻GPIO，腳位參閱附圖
6. USB Serial採用CH341驅動，可在這裡下載：https://twgo.io/ch340

Arduino開發板選擇方式，相容A.ESP32 Dev Module或者B.ESP32 Wrover Module

A. ESP32 Dev Module，參考以下設定：

  <img width="657" height="456" alt="image" src="https://github.com/user-attachments/assets/52595588-ebd4-4b87-90b3-ff9f01f435c9" />

  1. Flash Frequency：40MHz，Flash記憶體使用40MHz
  2. Flash Size：8MB(64Mb)，Flash記憶體提昇至8MB
  3. PSRAM：Enabled，本裝置使用PSRAM，可加快相機效能

B. ESP32 Wrover Module，參考以下設定：

  <img width="581" height="233" alt="image" src="https://github.com/user-attachments/assets/8433c19d-085b-47c3-bc18-2b8dec805206" />

  1. Flash Frequency：40MHz，Flash記憶體使用40MHz
  2. Partition Scheme：8M with spiffs(3MB APP/1.5MB SPIFFS)

