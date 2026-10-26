# 79G 雷達設定（網頁版 App）

Open it in Chrome on an Android phone. It connects to the radar over Bluetooth (Web Bluetooth) and needs to be served over HTTPS, for example on GitHub Pages.

- `index.html`: the whole app. The installer password is `INSTALLER_PIN` near the top of the script.
- `manifest.json`, `sw.js`, `icon-*.png`: make it installable to the home screen and let it open offline.
- Put `logo.png` in this folder to show the company logo.
- Protocol: service 0xAE30, write 0xAE01, notify 0xAE02. Text commands end with `\n`; see the protocol doc.
