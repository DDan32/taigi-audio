# taigi-audio

[台語生字簿](https://github.com/DDan32/taigi-notebook)用的錄音，只有 MP3 和這份說明。

## 來源與授權

錄音出自教育部《臺灣台語常用詞辭典》<https://sutian.moe.edu.tw/>（詞條音檔 `sutiau-mp3.zip`、例句音檔 `leku-mp3.zip`，
下載頁：<https://sutian.moe.edu.tw/zh-hant/siongkuantsuguan/>），
依「創用CC 姓名標示-禁止改作 3.0 臺灣」授權使用。**這不是教育部的網站。**

## 做過的處理

原檔 870 MB（56–65 kbps 單聲道 MP3），為了能放上網站，**只改了檔案格式，沒有剪輯、混音或改變內容**：
轉成單聲道、22.05 kHz、32 kbps 的 MP3（414 MB），移除檔案裡的標籤，改了檔名和資料夾。
轉完逐一檢查過：40,205 個檔案都能解碼，長度和原檔相符。工具在
[taigi-notebook/tools/build_audio.py](https://github.com/DDan32/taigi-notebook/blob/main/tools/build_audio.py)。

## 檔案怎麼放

```
w/<詞目id ÷ 1000 的整數>/<詞目id>.mp3        詞條的唸法（22,298 個）
s/<詞目id ÷ 1000 的整數>/<詞目id>-<義項>-<序號>.mp3   例句（17,907 句）
```

詞目 id 和教育部辭典下載檔裡的「詞目id」相同。

## 這個倉庫只放 MP3

同一個 GitHub 帳號的所有 Pages 網站共用同一個網域，網頁或腳本放在這裡，就能讀到同網域其他網站在瀏覽器裡存的資料。
所以這個倉庫**不要放 .html、.js、.svg 之類能執行的檔案**。
