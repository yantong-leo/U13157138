# U13157138
# 在無人機上以 ROS2 技術實現 YOLOv5 物件偵測
## Requirements
### 硬體與軟體環境

- **硬體平台**：Raspberry Pi 5
- **作業系統**：Raspberry Pi OS Full (64-bit)
    - 基於 Debian Bookworm (Debian 12)
    - 發布日期：2025-05-13
    - 映像檔大小：約 3.0 GB
### 本地端的電腦
* **Install ROS2**
    * 安裝 ROS2 到本地端電腦，安裝步驟請參考 [ROS2 官方網站安裝教學](https://docs.ros.org/en/kilted/Installation/Alternatives/Ubuntu-Development-Setup.html)
    * 本專案在本地端電腦使用的 ROS2 版本為 kilted
* **System setup

    * Set locale

Make sure you have a locale which supports UTF-8. If you are in a minimal environment (such as a docker container), the locale may be something minimal like POSIX.

```bash
locale  # check for UTF-8

sudo apt update && sudo apt install locales
sudo locale-gen en_US en_US.UTF-8
sudo update-locale LC_ALL=en_US.UTF-8 LANG=en_US.UTF-8
export LANG=en_US.UTF-8

locale  # verify settings
* **Install ROS2-v4l2-camera Package**
    * 安裝 ROS2 的 [ROS2-v4l2-camera](https://index.ros.org/r/v4l2_camera/) 包到本地端，版本為 kitled


```bash
sudo apt install ros-foxy-v4l2-camera
```
## 參考來源

本專案部分內容參考自以下 GitHub 倉庫：

- [U07157135/ROS2-with-YOLOv5](https://github.com/U07157135/ROS2-with-YOLOv5)
- https://docs.ros.org/en/kilted/Installation/Alternatives/Ubuntu-Development-Setup.html
