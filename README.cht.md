# 切石機增强

[简体中文](README.md) | [繁體中文](README.cht.md) | [English](README.en.md)

> NOTICE
>> This language file is translated by [fanyi.baidu.com](https://fanyi.baidu.com). If you want to improve the translated content, please create a pull request.

![icon](pack.png)

- 數据包支持版本: 1.14.4 -> 1.18.1
- Github: [https://github.com/Mo-yis/CutterPlus](https://github.com/Mo-yis/CutterPlus)

## 說明

- 一個羽量級數据包，添加了大量切石機的工作配方。
- 你甚至可以用切石機切木頭！ Emmm… 在生活中是可以的。
- 從版本 “2.4” 開始，使用 “Forge” 的通用礦物詞典標籤。
- 未加載的配方使用 “空氣” 填充，保證多個模組之間相容。
- 如果覺得空氣配方礙眼，可以將沒有的模組對應的以“support”開頭的資料夾删：

```
1. minecraft --------- 《Minecraft》是最早支持的內容。
2. tconstruct -------- 《匠魂 - 1.16.5》從版本 “2.4” 開始支持。
3. create ------------ 《機械動力 - 1.16.5》從版本 “2.9” 開始支持。
4. twilightforest ---- 《暮色森林 - 1.16.5》從版本 “2.10” 開始支持。
5. biomesoplenty ----- 《超多生物群系 - 1.16.5》從版本 “2.11” 開始支持。
6. bayou_blues ------- 《長沼藍調 - 1.16.5》從版本 “2.12” 開始支持。
7. autumnity --------- 《秋原 - 1.16.5》從版本 “2.13” 開始支持。
8. quark ------------- 《誇克 - 1.16.5》從版本 “2.14” 開始支持。
```

## 特性

- 要經過燒煉才能獲得的方塊無法從切石機獲得，如平滑石頭。
- 切石機只能加工固態物品和沒有 NBT 標籤的物品（從設計的角度上來看）。
- 同一類的方塊（材質不同）之間可以相互轉化（方塊，樓梯，臺階，牆）。
- 苔石和苔石磚是由圓石和石磚加工而來，故不能相互轉化。 其他情况類似。
- 樓梯可以加工成對應的臺階。
- 請在WIKI頁面查看詳細配方: [https://github.com/Mo-yis/CutterPlus/wiki](https://github.com/Mo-yis/CutterPlus/wiki)

## 計畫更新

- 更新模組內容的支持
- 添加更多模組間相容性配方
- 調整資料夾目錄、規範檔案命名
- 支持更多 1.16.5 的模組

## 使用方法

- Github: 右上角點擊**綠色**的 “**Code**” 再點擊 "**Download ZIP**"。
- 如果你打算將數据包放入存檔中，請解壓在 ".minecraft \\ saves \\ (存檔名稱) \\ datapacks \\ " 目錄下。
- 如果你正準備新建世界，請將解壓出的資料夾添加到遊戲中。
- 如果你打算加載到已經啟動的遊戲或服務器中，請在後臺或以3級操作員身份鍵入 "/reload" 以加載數据包。
- 相關疑問請査詢 Minecraft Wiki。

## 注意

- 與模組不同，數据包僅對單個世界有效。 但是有些 MOD 可以實現在多個世界中共亯數据包。
- 數据包相容一定範圍內的版本，但是不會針對舊版本進行維護。
- 請勿添加功能類似或相同的數据包。
- 當數据包成功加載時，遊戲中會提示 "[ 數据包名稱 ] Loading Successful !"。
- 版本低於 1.15.2 無法顯示提示資訊，請以管理員身份鍵入命令 "/datapack list" 查看數据包資訊。
