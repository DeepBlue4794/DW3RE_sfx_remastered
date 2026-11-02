# 原版提示音還原 v0.5：音量加強

仍只替換 Sys08–12，對應原版 linkdata_00006–00010。
本版從原始 WAV 重建，使用相對 v0.3 的 +10 dB 輸入增益及平滑飽和處理，提高聲音主體音量。這不是完全保留動態的線性放大：較強波峰會壓縮，音色可能稍硬。ADPCM 編碼另限制重建峰值；最終解碼無滿刻度樣本。

| 音效 | 相對 v0.4 的平均 RMS 增加 |
|---|---:|
| Sys08 擊敗敵將 | 4.61 dB |
| Sys09 我方將領敗走 | 4.23 dB |
| Sys10 情報 | 4.82 dB |
| Sys11 歡呼 | 5.07 dB |
| Sys12 警告 | 4.23 dB |

## 安裝

1. 關閉遊戲。
2. 移除舊版 MOD 的 .pak、.utoc、.ucas 三個檔案，例如 zDW3_ClassicAlerts_v04_P.*。同時也不要保留更舊版本。不要移除原廠 DW3CE_RE-Windows.* 或 global.*。
3. 將本包 DW3CE_RE 資料夾複製到 F:\SteamLibrary\steamapps\common\DW3CE_RE，合併資料夾。
4. 確認 zDW3_ClassicAlerts_v05_P.pak、.utoc、.ucas 三檔位於遊戲的 DW3CE_RE/Content/Paks。

只啟用一版。本包未自動安裝，遊戲內音量與音色仍待試聽。移除新版三檔可恢復原廠音效；放回 v0.4 三檔可回退。

## 驗證與後續

容器檢查、封裝後重新抽取比對通過，全部 53 個音效均能解碼，其餘 48 個與原基準完全一致。
後續修改沿用 v0.5 設定，從原始 WAV 重建，不逐版累加增益。設定為 work/mod-development/audio_settings.json；建置使用 build_v05.py、audio_processing.py 與 adpcm_encoder_safe.py。
