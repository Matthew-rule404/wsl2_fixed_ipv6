# wsl2_fixed_ipv6
wsl2 use IPv6 fixed address


■Windows 11でIPv6固定アドレスを利用する
前提となる技術セット
1. PowerShell
2. WSL2 - Windows Subsystem for Linux
　　利用するバージョン　2.5.9

```
(base) PS C:\Users\masato> wsl --version
WSL バージョン: 2.5.9.0
カーネル バージョン: 6.6.87.2-1
WSLg バージョン: 1.0.66
MSRDC バージョン: 1.2.6074
Direct3D バージョン: 1.611.1-81528511
DXCore バージョン: 10.0.26100.1-240331-1435.ge-release
Windows バージョン: 10.0.26100.4652
(base) PS C:\Users\masato>
```

4. Ubuntu
    利用するバージョン　24.04 LTS
　　※その他バージョンにおいても利用可能であると考えられるが未検証


バージョンを確認（os-releaseを確認する方法）
```
$ cat /etc/os-release
PRETTY_NAME="Ubuntu 24.04.2 LTS"
NAME="Ubuntu"
VERSION_ID="24.04"
VERSION="24.04.2 LTS (Noble Numbat)"
VERSION_CODENAME=noble
ID=ubuntu
ID_LIKE=debian
HOME_URL="https://www.ubuntu.com/"
SUPPORT_URL="https://help.ubuntu.com/"
BUG_REPORT_URL="https://bugs.launchpad.net/ubuntu/"
PRIVACY_POLICY_URL="https://www.ubuntu.com/legal/terms-and-policies/privacy-policy"
UBUNTU_CODENAME=noble
LOGO=ubuntu-logo
```

バージョンを確認（issueを確認する方法）
```
$ cat /etc/issue
Ubuntu 24.04.2 LTS \n \l
```

カーネルバージョンを確認する
```
$ uname -r
6.6.87.2-microsoft-standard-WSL2
```

アーキテクチャを確認する
```
$ arch
x86_64
```

5. Hyper-V
   利用するバージョン
```
> (Get-Item "C:\Windows\System32\vmms.exe").VersionInfo.ProductVersion
10.0.26100.2308
```
   
7. ansible
8. ネットワーク全般


■Ubuntu 24.04 LTS
1. SSH接続サーバー側設定
　　秘密鍵認証の設定
2. 　
3. WSL2 - Windows Subsystem for Linux
　　利用するバージョン　2.5.9


