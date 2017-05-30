# macOS的工具/软件一键安装

## 目标
- **可控** homebrew安装路经不合心意，也不喜欢一键打包安装的方式，想要控制所有的安装细节
- **最新** 可随机更新到真正的最新版本，是的，只有官网发布的或者git仓库才是最新的。为什么要最新? 更好更快更安全(有什么理由不用Python3.6.1而用Python2.7.*)
- **云端友好** 可以自己选择安装位置，这样我不需要安装到系统，而是安装到一个放在云盘的用户级权限的目录，所有的电脑都可以用同一份。
- **干净** 绿色安装，删掉目录即可还原，不对系统作修改，也不依赖系统。
- **快速安装** 换机器后可以快速安装/云盘同步得到同样环境
- **对开发友好** 自定制编译参数，方便得到dlib等额外开发所需

## Features

1. 统一安装路经并尽量减少对系统的修改，只有普通用户权限下执行软件安装，方便卸载
2. 可随时检查更新，实现自动从官网下载安装最新版(需要HTML页面解释抓取链接)

## 安装路经
* 安装目录全部设为./bin/{package_name}/
* 添加bin/和bin/{package}/bin到PATH
