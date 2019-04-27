# ShadowsocksR跨平台客户端（SSR 科學上網）

这是一个跨平台（支持Windows MacOS Linux系统）的`ShadowsocksR`客户端桌面应用，特別是Ubuntu科學上網必備`SSR`客戶端。
技術上主要使用的是`Vue` `electron` `javascript` 。
簡單到只需要懂點`html`，`css`，`JavaScript`的前端開發工程師就可以方便開發。
它功能丰富，而且這貨是开源的，可以按照你自己的想法來改造。


## 下载

下载地址见[Github release](https://github.com/erguotou520/electron-ssr/releases)，对应的操作系统下载的文件为

- Windows `electron-ssr-setup-x.x.x.exe`
- Mac `electron-ssr-x.x.x.dmg`
- Linux 优先建议下载`electron-ssr-x.x.x.AppImage`，直接双击运行。如果无法使用或者想直接下载自己系统专用包请看下一条
- Arch或者基于Arch的系统，下载`electron-ssr-x.x.x.pacman`
- RedHat系列的系统，下载`electron-ssr-x.x.x.rpm`
- Debian系列的系统，下载`electron-ssr-x.x.x.deb`
- 系统Linux系统或者通用Linux系统可下载`electron-ssr-x.x.x.tar.gz`（不会使用.tar.gz的请自行百度）
- ubuntu18.04 經過測試可以用deb包
## 配置文件位置

- Windows `C:\Users\{your username}\AppData\Roaming\electron-ssr\gui-config.json`
- Mac `~/Library/Application Support/electron-ssr/gui-config.json`
- Linux `~/.config/gui-config.json`

## 快捷键

加入快捷键本来是为了解决部分Linux发行版无法显示图标导致功能无法使用而加入的，当然其它系统也是可以使用的，同时支持在设置中进行开启/关闭以及更换按键的操作。

### 全局快捷键

- `CommandOrControl+Shift+W` 切换主窗口显隐
- `未设置` 切换系统代理

### 应用内快捷键
- `CommandOrControl+Shift+B` 切换是否显示操作菜单，仅Linux可用

## 已知Bug

- 部分Linux系统无法切换系统代理模式（本应用使用`gsetting`设置系统代理，所以有些Linux系统无法使用该功能），如果你知道如何实现，欢迎发issue告知。
- Windows系统切换全局代理不生效

## 应用截图

![](docs/assets/main.jpg)
![](docs/assets/settings.jpg)
![](docs/assets/ssr-settings.jpg)
![](docs/assets/subscribe.jpg)
![](docs/assets/tray.jpg)

## FAQ

[FAQ](./docs/FAQ.md)

## Issus

请在发issue前先查看FAQ里的说明能不能解决你的问题。
在发issue前请先在issue中搜索是否有同类issue，如果有请跟帖。
另外发Bug类issue请详细描述你的使用环境，包括但不限于操作系统、软件版本，操作步骤，报错日志等。


欢迎提出改修意见

## 开发和构建

``` bash
# 安裝依賴 
npm install

# 开发时
npm run dev

# 打包构建
npm run build

# 单元测试
npm run mocha

# 代码风格检查
npm run lint

```
## Ubuntu18.04 構建測試，建議使用yarn
``` js
# 安裝項目所有的依賴
yarn install 

# 開發測試
yarn run dev

# 打包測試
yarn run build
```

## 本項目原始fork來源
`electron-ssr`  

詳情请直接查看[release发布说明](https://github.com/erguotou520/electron-ssr/releases)

