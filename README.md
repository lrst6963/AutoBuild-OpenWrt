# AutoBuild-OpenWrt
[![LICENSE](https://img.shields.io/github/license/mashape/apistatus.svg?style=flat&logo=github&label=LICENSE)](https://github.com/esirplayground/AutoBuild-OpenWrt/blob/master/LICENSE)
![GitHub Stars](https://img.shields.io/github/stars/esirplayground/AutoBuild-OpenWrt.svg?style=flat&logo=appveyor&label=Stars&logo=github)
![GitHub Forks](https://img.shields.io/github/forks/esirplayground/AutoBuild-OpenWrt.svg?style=flat&logo=appveyor&label=Forks&logo=github)
![GitHub last commit](https://img.shields.io/github/last-commit/esirplayground/AutoBuild-OpenWrt?label=Latest%20Commit&logo=github)

Build OpenWrt firware [Lean's OpenWrt](https://github.com/coolsnowwolf/lede) using GitHub Actions  
Hereby thank P3TERX for his amazing job: https://github.com/P3TERX/Actions-OpenWrt/  
Hereby thank KFERMercer for his amazing job: https://github.com/KFERMercer/OpenWrt-CI  

## Usage | 使用

🔥🔥[Video Tutorial (in Mandrin) | 视频教程(国语)](https://youtu.be/9YO7nxNry-4)📺🎉

**1. Prerequisite | 必要条件**
  - Sign up for [GitHub Actions](https://github.com/features/actions/signup)
  > 注册[GitHub Actions](https://github.com/features/actions/signup)
  - Fork [this GitHub repository](https://github.com/lrst6963/AutoBuild-OpenWrt)
  > 复刻[这个 GitHub 存储库](https://github.com/lrst6963/AutoBuild-OpenWrt)
    
**2. Compile Firmware | 编译固件**
  - Click `[.github/workflows]` folder on the top of repo and you could see few workflow files, Each for one particular architecture(device).
  > 点击 `[.github/workflows]` 文件夹，你可以看到一些工作流文件，每个为一个特定的架构(设备)
  - Edit the workflow file you desire，uncomment push section 3 lines together and submit the commit.(Other 2 methods wait you to discover)
  > 编辑您想要的工作流文件，取消注释，将第3节推到一起，并提交更改。(其他两种方法等你去发现)
  - The build starts automatically. Progress can be viewed on the Actions page.
  > 生成启动。进度可以在 Actions 页面上查看
  - When the build is complete, click the `Artifacts` button in the upper right corner of the Actions page to download the binaries.
  > 当构建完成后，点击 Actions 页面右上角的‘ Artifacts’按钮来下载二进制文件
  - Mi_R3G 默认Web IP：`192.168.168.1` 密码：`password`
  - x86_64 默认Web IP：`192.168.1.1` 密码：`password`

### 使用PushPlus进行微信推送通知

1. 注册[PushPlus](https://www.pushplus.plus/)并复制页面中生成的 **Token**

2. **Fork** 我的`AutoBuild-OpenWrt`仓库,然后进入你的`AutoBuild-OpenWrt`仓库进行之后的设置

3. 点击上方菜单中的`Settings`,依次点击`Secrets`-`New repository secret`

4. 其中`Name`项填写`PUSHPLUS_TOKEN`,然后将你的 **Token** 粘贴到`Value`项,完成后点击`Add secert`

* 对应`.github/workflows`目录下的`yml`工作流文件里的`PUSHPLUS_TOKEN`名称（依据自己yml文件修改）

* 可通过[PushPlus](https://www.pushplus.plus/) 推送编译结果到微信



