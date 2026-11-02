# 目前狀態

更新：2026-11-02

目前版本 v0.5。Sys08–12 對應原版 linkdata_00006–00010：擊敗敵將、我方將領敗走、情報、歡呼、警告。使用者確認 v0.3 可用，後續回報音量不足；v0.5 尚待遊戲內音量／音色回饋。

v0.5 解碼後平均 RMS 相對 v0.4 增加約 4.2–5.1 dB；其餘 48 個音效未變。封裝驗證、重新抽取比對、53 個音效解碼通過。

後續沿用 audio_settings.json 的 v0.5 增益與平滑飽和處理，從原始 WAV 重建，不逐版累加。完整驗證記錄在 ../rel/ClassicAlerts-v0.5/validation.json。

編輯音效辨識對照表.md 追蹤使用者辨識；targets_v03.json 為目前五個對應的建置資料，名稱為歷史版本名，v0.5 仍使用同一組。

原製作腳本、解包工具與基準音庫仍位於 C:/Users/User/Documents/Codex/2026-10-22/new-chat/work/mod-development，最新建置腳本為 build_v05.py。本次整理素材、發行包及紀錄，尚未把完整建置環境搬入此專案。原腳本的來源路徑需要在下次建置前改為本專案 origin_sfx_res。

## 專案整理與 Git（2026-11-02）

原始 758 檔已複製至 ../origin_sfx_res，總計 64,307,345 bytes；SHA-256 與 origin_sfx_manifest.json 一致。刪除 F 槽來源的命令被自動核准審查拒絕，尚未執行，因此來源仍保留。本次整理為已驗證複製，尚未完成來源清除。

origin 設定為 https://github.com/DeepBlue4794/DW3RE_sfx_remastered.git。已成功 fetch，並以 merge 保留本機與遠端各自的初始提交；main 已追蹤 origin/main。本機目前領先遠端兩筆提交（原本機初始提交與合併提交），素材與整理文件尚未提交或推送。
