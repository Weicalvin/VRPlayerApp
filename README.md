# VR Player Pro - Android 應用程式

一個現代化的 VR 播放器應用，採用原生 Android 開發，支援 ExoPlayer 媒體播放和 VR 渲染。

## 專案結構

```
VRPlayerApp/
├── app/
│   ├── src/main/
│   │   ├── java/com/vr/player/
│   │   │   └── MainActivity.kt          # 主活動，包含播放邏輯
│   │   ├── res/
│   │   │   ├── layout/
│   │   │   │   └── activity_main.xml    # 主佈局，包含 PlayerView
│   │   │   ├── values/
│   │   │   │   ├── strings.xml          # 字符串資源
│   │   │   │   └── colors.xml           # 顏色定義
│   │   │   └── mipmap/                  # 應用圖標
│   │   └── AndroidManifest.xml          # 應用清單
│   └── build.gradle                     # 模組構建配置
├── build.gradle                         # 專案構建配置
├── settings.gradle                      # Gradle 設定
└── gradle.properties                    # Gradle 屬性

```

## 功能特性

- **ExoPlayer 整合** - 支援多種影片格式的播放
- **檔案選擇器** - 從手機儲存空間選擇影片
- **全螢幕播放** - 沉浸式播放體驗
- **播放控制** - 播放/暫停、進度條、音量控制
- **橫向鎖定** - 應用固定為橫向模式

## 技術棧

- **語言**：Kotlin
- **最小 SDK**：21
- **目標 SDK**：34
- **播放器**：ExoPlayer 2.19.1
- **佈局**：ConstraintLayout

## 構建和執行

### 前置要求

- Android Studio 2023.1 或更新版本
- JDK 11 或更新版本
- Android SDK 34

### 步驟

1. **在 Android Studio 中開啟專案**
   ```bash
   cd /home/ubuntu/VRPlayerApp
   ```

2. **同步 Gradle**
   - 點擊 "Sync Now"

3. **執行應用**
   - 選擇目標設備或模擬器
   - 點擊 "Run" 或按 Shift+F10

4. **測試播放功能**
   - 點擊右下角的「選擇影片」按鈕
   - 從手機儲存空間選擇 MP4 檔案
   - 影片應開始播放

## 權限

應用需要以下權限：

- `INTERNET` - 用於未來的 Telegram 串流功能
- `READ_EXTERNAL_STORAGE` - 讀取手機檔案
- `WRITE_EXTERNAL_STORAGE` - 寫入手機檔案

## 下一步開發

- [ ] VR 雙眼渲染器（OpenGL）
- [ ] 畸變校正
- [ ] Telegram 串流整合
- [ ] Android TV 遙控器支援
- [ ] 進度條自訂
- [ ] 音量和亮度控制

## 開發者

由 Manus AI 協助開發

## 授權

MIT License
