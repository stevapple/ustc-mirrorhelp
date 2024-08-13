# WinGet

## 地址

<https://mirrors.ustc.edu.cn/winget-source>

## 说明

Windows Package Manager (aka. WinGet) 默认软件源

## 使用说明

!!! note

    修改 WinGet 软件源需要管理员权限，请以管理员身份运行终端。

=== "WinGet >= 1.8"

    用以下命令替换 `winget` 源：

    ```shell
    winget source remove winget
    winget source add winget https://mirrors.ustc.edu.cn/winget-source --trust-level trusted
    ```

=== "WinGet <= 1.7"

    用以下命令替换 `winget` 源：

    ```shell
    winget source remove winget
    winget source add winget https://mirrors.ustc.edu.cn/winget-source
    ```

    !!! note

        若出现 0x80073d1b : smartscreen reputation check failed.
        错误，请检查网络连接或暂时关闭 SmartScreen。

重置为官方地址：

    winget source reset winget

## 相关链接

GitHub

:   <https://github.com/microsoft/winget-cli>

Microsoft Store

:   <https://apps.microsoft.com/store/detail/%E5%BA%94%E7%94%A8%E5%AE%89%E8%A3%85%E7%A8%8B%E5%BA%8F/9NBLGGH4NNS1>

官方教程

:   <https://learn.microsoft.com/zh-cn/training/modules/explore-windows-package-manager-tool>

软件源仓库

:   <https://github.com/microsoft/winget-pkgs>
