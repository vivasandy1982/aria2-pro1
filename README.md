
# Aria2－Pro 最強版本 快速部署安裝
<p align="center">
	<img src="/service/whk.jpg" />
</p>

[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat-square&label=LICENSE)](https://github.com/P3TERX/aria2.sh/blob/master/LICENSE)
[![GitHub Stars](https://img.shields.io/github/stars/P3TERX/aria2.sh.svg?style=flat-square&label=Stars)](https://github.com/P3TERX/aria2.sh/stargazers)
[![GitHub Forks](https://img.shields.io/github/forks/P3TERX/aria2.sh.svg?style=flat-square&label=Forks)](https://github.com/P3TERX/aria2.sh/fork)

## 原創項目地址

https://github.com/P3TERX/aria2.sh

## 系统要求

Ubuntu 18.04.3 (LTS) x64

## 下载安装
-----------------------------------------------------------------------------------
	新手專區
新手不會 git clone語言請走此步驟
請把該更新的更新完畢,以免奇怪問題發生導致無法安裝
安裝環境使用 Ubuntu 18.04.3 (LTS) x64
請勿安裝其他版本,新版測試並沒有比較穩定,追新者要嘗試也是可以
#
sudo apt-get update 
#
sudo apt-get dist-upgrade	
#更新完成後重啟伺服器
reboot
1
#
wget https://github.com/vivasandy1982/aria2-pro1/blob/master/aria2-pro1-master.zip
#
apt install unzip
#
unzip aria2-pro1-master.zip
#
cd aria2-pro1-master
#執行快速部署腳本
chmod +x aria2.sh && ./aria2.sh
#剩餘步驟請參照以下使用說明
-------------------------------------------------------------------------------------

執行下面的代碼下載並運行腳本，出現腳本操作表單時輸入 `1` 開始安裝。

--------------------------原創者安裝---------------------------------------------------------
```shell
wget -N git.io/aria2.sh && chmod +x aria2.sh && ./aria2.sh
```
--------------------------原創者安裝---------------------------------------------------------


## 使用說明

* 進入腳本表單開始執行
  
  ```
  ./aria2.sh
  ```

* 選擇你要執行的項目
  
  ```
  Aria2完美版本 快速部署腳本 [v2.0.8]
  -- hack.chat --白帽珊蒂
  
  1. 升級腳本
  ————————————
  1. 安装 Aria2
  2. 更新 Aria2
  3. 移除 Aria2
  ————————————
  4. 啟動 Aria2
  5. 停止 Aria2
  6. 重啟 Aria2
  ————————————
  7. 修改 配置
  8. 查看 配置
  9. 查看 日志
  10. 清空 日誌
  ————————————
  11. 手動更新 BT-Tracker
  12. 自動更新 BT-Tracker
  ————————————
  
  目前狀態: 已安装 并 執行中
  
  請輸入數字 [0-12]:
  ```

## 其他操作

啟動：`/etc/init.d/aria2 start`

停止：`/etc/init.d/aria2 stop`

重啟：`/etc/init.d/aria2 restart`

查看狀態：`/etc/init.d/aria2 status`

配置文件：`/root/.aria2/aria2.conf` （配置文件包含中文解釋，但是一些系统可能不支持顯示中文）

令牌金鑰：隨機產生（可以自己修改 7. 修改 配置文件）

默認下載目錄：`/root/Download`

## 附加功能

整合了 [Aria2 完美配置](https://github.com/P3TERX/aria2_perfect_config)，在安装 Aria2 的过程中会下载這套配置方案，包含了配置文件、附加功能脚本等文件，用於運作 Aria2 功能的增强和擴展。

增强功能：

* 提升BT下载率和下载速度
* 下载完成删除残留的`.aria2`后缀名文件
* 下载错误或取消下载删除未完成的文件

新功能：

* [OneDrive、Google Drive 等運端硬碟下載](https://p3terx.com/archives/offline-download-of-onedrive-gdrive.html)
* [百度雲端硬碟到 OneDrive 、Google Drive 等其他雲端硬碟](https://p3terx.com/archives/baidunetdisk-transfer-to-onedrive-and-google-drive.html)

--------------------------2019/12 bbr加速四合一暴力魔改最新版本(修正後穩定版）------------------------------------
#
執行腳本後請注意不要每個都安裝,請參照以下對應順序
#
cd aria2-pro1-master
#
安裝過程中有yes選yes,總之一直enter直走就對了
#
wget -N --no-check-certificate "http://shell.p1e.cn/BBR/4for1tcp.sh" && chmod +x 4for1tcp.sh && ./4for1tcp.sh
#
安裝魔改版本請照右側表單數字依序安裝 1.4.5.6
#
安裝過程中遇到提示畫面並且選項反白停留在yes的選項時請注意,提示畫面最後一行英文是>>>>>abort kernel removal??<<<<<<<<
#
請選擇no跳出之後隨即會提示重啟伺服器,選擇yes
#
安裝完順序６之後請先重啟伺服器
#          
reboot
#
執行腳本指令看是否bbr與魔改加速是否正常啟動
#
wget -N --no-check-certificate "http://shell.p1e.cn/BBR/4for1tcp.sh" && chmod +x 4for1tcp.sh && ./4for1tcp.sh
#
顯示bbr與魔改都成功啟動後選擇10優化配置,接者會提示重啟伺服器請選擇y
#
檢查你的aria2是否正常運作
#
/etc/init.d/aria2 status
-----------------------------------------------------------------------------------------------------------------
------------------------wireguard ipv4 ipv6 合併加速--------------------------------------------------------------







## 更新日誌

### 2019-11-23 v2.0.8

- 修改 Trackers 來源([XIU2/TrackersListCollection](https://github.com/XIU2/TrackersListCollection))

<details>
<summary>歷史紀錄</summary>

### 2019-10-12 v2.0.7

- 修复 Aria2 版本更新时因未獲取 CPU 架構導致版本下载錯誤且無法啟動的 bug

### 2019-09-30 v2.0.6

- 獲取 DHT（IPv6）文件

### 2019-06-08 v2.0.5

- 增加 清空日誌 功能
- 調整 部分文案

### 2018-12-25 v2.0.4

- 強化參數調整

### 2018-12-24 v2.0.3

- 增加 重置/更新 Aria2 完美配置 選項
- 強化 修改配置文件下載路徑時同步修改附加功能脚本中的下載路徑

### 2018-12-8 v2.0.2

- 修复 附加功能脚本没有執行權限的 bug

### 2018-12-7 v2.0.1

- 修复 設置下載文件夾提示不存在的 bug
- 解鎖 更新 BT-Tracker伺服器 選項

### 2018-12-7 v2.0.0α

- 整合 [Aria2 完美配置](https://github.com/P3TERX/aria2_perfect_config)

### 2018-10-18 v1.1.10

- 取自[一个逗比写的逗比脚本](https://github.com/P3TERX/doubi_backup)
- 感谢 Toyo 大佬

</details>




