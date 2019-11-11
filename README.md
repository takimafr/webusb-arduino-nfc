<div align="center">
<h1>Arduino NFC Reader through WebUSB️ 💻</h1>

![nfc tag]
![arduino tag]
![react tag]
![node tag]
![electron tag]
![socketio tag]

Multiple ways to develop a web application communicating with a NFC reader.

<h2>See the <a href="https://slides.com/gautierdarchen/webusb-arduino-nfc/fullscreen">slides</a></h2>

</div>

---

This repo aims at explaining how I ended up building a NFC Reader with an Arduino using the WebUSB API.

You will find the three solutions I developed to make a web application communicate with a NFC Reader.

## Solution 1 - Electron application using a NFC Reader

![nfc tag] ![react tag] ![electron tag]

Using a ACR122U NFC Reader, I firstly implemented an Electron application to handle NFC reading.

You can find the code for this solution in the `./1-electron` folder.

### See the [1-electron/README.md](1-electron/README.md) file to understand how it works.

## Solution 2 - Local server NFC Reader and _web-sockets_

![nfc tag]
![react tag]
![node tag]
![socketio tag]

Still using a ACR122U NFC Reader, I implemented the a local Node.js server handling the NFC reading part and sending the read payload to a front-end application through _web-sockets_.

You can find the code for this solution in the `./2-local-nfc-server` folder.

### See the [2-local-nfc-server/README.md](2-local-nfc-server/README.md) file to understand how it works.

[react tag]: https://img.shields.io/badge/react-JS-blue?style=for-the-badge&logo=react
[nfc tag]: https://img.shields.io/badge/nfc-PCSC-green?style=for-the-badge&logo=data:image/png;base64,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
[electron tag]: https://img.shields.io/badge/electron-JS-blue?style=for-the-badge&logo=electron
[arduino tag]: https://img.shields.io/badge/Arduino-IOT-00979d?style=for-the-badge&logo=arduino
[node tag]: https://img.shields.io/badge/Node.js-JS-43853d?style=for-the-badge&logo=node.js
[socketio tag]: https://img.shields.io/badge/Socket.io-Websockets-black?style=for-the-badge&logo=socket.io
