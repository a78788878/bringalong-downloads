# 出門帶了嗎 0.2.0（1）

[下載最新 IPA](https://github.com/a78788878/bringalong-downloads/releases/latest/download/BringAlong.ipa) · [所有版本](https://github.com/a78788878/bringalong-downloads/releases)

## 最簡單的更新方式（只需設定一次）

1. Windows 開啟 AltServer，iPhone 用 USB 連上電腦並解鎖。
2. iPhone 開啟 AltStore Classic → 底部獨立的 Sources 分頁 → ＋，貼上下面來源網址並加入。Sources 不在 Browse 裡；AltStore 2.3 支援自訂來源。
3. 在來源裡選「出門帶了嗎」安裝／更新，使用原本的 Apple ID。保留原 App 直接覆蓋；不要先刪除。

來源網址：

```text
https://github.com/a78788878/bringalong-downloads/releases/latest/download/altstore-source.json
```

以後有新版：AltStore → My Apps → 出門帶了嗎 → Update。AltStore 會依來源版本資訊顯示可用更新；新版發佈後才會出現。

若來源加入失敗：用 Safari 下載上面的 IPA，AltStore → My Apps → ＋ → 選 Downloads 裡的 BringAlong.ipa。

安裝後開啟 App → 設定，核對版本並做「30 秒後鎖屏測試」。定位設「永遠」、開啟精確位置，再確認監控地點數量；200 公尺仍需實走測試。

## 完全不用開發者模式：需改用 TestFlight

AltStore 安裝／更新的 App 使用開發簽署，iPhone 開發者模式必須保持開啟。開啟一次後正常更新不必反覆切換；關閉後再使用開發簽署 App 仍需重新開啟。App 程式無法取消這項系統要求，本 App 不需要 Enable JIT。

若要求開發者模式保持關閉，請使用 TestFlight 或 App Store 發行版本。TestFlight 使用者不用開發者模式，可開啟自動更新；發行者需具備 Apple Developer Program 會員及完成 Apple 簽署／上傳。現在尚無 TestFlight 邀請，本 IPA 不能當成 TestFlight 安裝包。

AltStore 2.3 的 Remote AltServer 可減少接電腦，但不取消開發者模式或每週續簽要求。設定入口是 Settings → Set up Remote AltServer；依官方流程一次配對並設定 LocalDevVPN，以後使用 Wi-Fi（非行動網路）與 LocalDevVPN 安裝／續簽。這是可選方案，不符合「完全不用開發者模式」的要求。

官方來源：[Apple 開發者模式](https://developer.apple.com/documentation/xcode/enabling-developer-mode-on-a-device) · [Remote AltServer](https://faq.altstore.io/altstore-classic/remote-altservers)

## 簽署期限

免費 Apple ID 的簽署通常 7 天到期。Refresh All 是延長期限，Update 是安裝新版。AltStore 的 Background Refresh 可嘗試背景重新簽署，需能連上 AltServer；並不保證自動安裝新版。手機提示無法開啟時，先檢查 AltStore 到期日。

本安裝檔未簽署，需 AltStore；手機無法只靠 Safari 直接完成安裝。原本已安裝 AltStore 的使用者可直接照上面操作。後續 TestFlight 發佈完成後，改由 TestFlight 的「自動更新」處理。

此下載區只有 App 安裝檔、圖示及更新資訊；App 不會把你的清單或住家位置放進安裝檔。安裝包未經 Apple 外部測試審查，提醒可靠度不保證即時，尤其不要強制關閉 App。
