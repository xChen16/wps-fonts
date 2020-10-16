# WPS Linux Fonts
WPS for Linux字体缺失

## 安装方法


Clone the Git repository.
```
git clone https://github.com/xChen16/wps-fonts.git
```

拷贝字体到 usr/share/fonts
```
sudo cp -r wps-font/ /usr/share/fonts/wps-font-symbols
```
权限配置
```
cd /usr/share/fonts

sudo chmod 755 wps-font-symbols

cd /usr/share/fonts/wps-font-symbols

sudo chmod 644 *

```
生成字体缓存信息

```
cd /usr/share/fonts/wps-font-symbols

sudo mkfontdir

sudo mkfontscale

sudo fc-cache
```
### 重启WPS

