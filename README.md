# ability-hand-sample-touchdesigner

<img src="https://img.shields.io/badge/Python-3.11 or Later-blue?&logo=Python"> <img src="https://img.shields.io/badge/TouchDesigner-2023-blue?"> <img src="https://img.shields.io/badge/License-MIT-green">

[PSYONIC, Inc.](https://www.psyonic.io/)が販売しているAbility HandをTouchDesignerから制御するためのサンプルです。

This sample is for controlling the Ability Hand available from [PSYONIC, Inc.](https://www.psyonic.io/) from TouchDesigner.

# Table Of Contents <!-- omit in toc -->
<details>
<summary>Details</summary>

- [ability-hand-sample-touchdesigner](#ability-hand-sample-touchdesigner)
- [Copyright](#copyright)
- [Environment](#environment)
- [Installation](#installation)
  - [How to connect](#how-to-connect)
- [Description](#description)
- [References](#references)
- [Troubleshooting](#troubleshooting)
- [Versions](#versions)
- [Author](#author)
- [License](#license)
</details>

# Copyright
このプログラムは[PSYONIC, Inc.](https://www.psyonic.io/)が開発、公開している[Ability Hand用のPython API](https://github.com/psyonicinc/ability-hand-api)を編集して作成しています。

This program is created by editing the [Python API for Ability Hand](https://github.com/psyonicinc/ability-hand-api) developed and published by [PSYONIC, Inc.](https://www.psyonic.io/)

Copyright © 2023-2024 PSYONIC, Inc. All Rights Reserved.


# Environment
- TouchDesigner 2023
- Python 3.11 or later

# Installation
事前にTouchDesignerがインストールされており、Pythonの外部モジュールを読み込むパスが正しく通っていることを確認してください。
また、以下のモジュールを参照できることを確認してください。
- serial

まだの場合は、以下を実行してインストールしてください。
また、TouchDesignerから読み込んでいるモジュールのパスに以下が配置されていることを確認してください。
```bash
pip install pyserial
```


Please make sure that TouchDesigner has been installed and that the path to load Python external modules has been properly passed in advance.
Also please make sure that the following modules can be referenced.
- serial

If not already installed, perform the following to install.
Also, please make sure that the following are placed in the path of the module you are loading from TouchDesigner
```bash
pip install pyserial
```

## How to connect
![HowToConnect](https://github.com/user-attachments/assets/47038b82-8f04-41eb-8816-7ece3a7bed89)

# Description
Ability Handにシリアル通信で接続し、スライダーによって各指を制御するデモが含まれています。
また、各指のセンサデータを読み取るデモも含まれています。

1. Connect to the Ability Hand ボタンを押す
2. Ability Handが動くことを確認する
   - この時、TouchDesignerのコンソールにもログが出力されます
3. Send data トグルスイッチをOnにする
4. 各指のスライダーを動かすとAbility Handの指が動く
   - この時、Open sensor data viewer ボタンを押すと指のセンサデータを表示します
5. Send data トグルスイッチをOffにする
6. 1から繰り返し


This project includes a sample that connects to Ability Hand via serial communication and controls each finger with a slider.
Also included is a sample that reads the sensor data for each finger.

1. Press the “Connect to the Ability Hand” button
2. Make sure that each finger of the Ability Hand moves
   - At this time, logs are also output to the TouchDesigner console
3. Set the “Send data” toggle switch to On
4. Move the slider for each finger to move the finger of the Ability Hand
   - At this time, press the "Open sensor data viewer" button to display the finger sensor data
5. Turn off the “Send data” toggle switch
6. Repeat from 1


# References
- [PSYONIC, Inc.](https://www.psyonic.io/)
- [Python API for Ability Hand](https://github.com/psyonicinc/ability-hand-api)


# Troubleshooting


# Versions
- 1.0.0: 2024/10/18

# Author
- Takayoshi Hagiwara
    - Graduate School of Media Design, Keio University
    - Toyohashi University of Technology


# License
- MIT License