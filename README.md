为了在树莓派4B上尝试使用不同的操作系统，但发现原有的Argon ONE用于控制电源按钮及风扇的脚本并不完全兼容。因此，我基于现有的脚本进行了相应的修改，并将这些修改后的脚本整合到了本项目中。这样一来，将来如果再遇到相同的操作系统时，就可以迅速地进行配置和使用。

本项目相关脚本专为 Argon ONE 在 Raspberry Pi 平台上使用，其功能在于控制电源按钮及风扇。该项目的目的是为了适配在 Raspberry Pi 上安装的各种操作系统类型。

|脚本名称| 来源                                                                         | 测试系统                             | 测试设备                   | 备注                                       |
|----|----------------------------------------------------------------------------|----------------------------------|------------------------|------------------------------------------|
|argon1.sh| [官网提供](https://download.argon40.com/argon1.sh)                             | 无                                | 无                      | 官方提供版本，仅搬运                               |
|argon1_centos.sh| [GitHub上tomjo/argonone-centos仓库](https://github.com/tomjo/argonone-centos) | CentOS 7 Kernel 5.4.56-v7l.1.el7 | Raspberry Pi 4 Model B | GitHub上tomjo/argonone-centos分享的脚本，仅搬运         |
|argon1_openeuler.sh| 无                                                                          | openEuler 24.03 (LTS)            | Raspberry Pi 4 Model B | 基于 GitHub上tomjo/argonone-centos分享的脚本改造而来 |


## 使用方法
`curl https://raw.githubusercontent.com/chaoyuejc/argon1-all/refs/heads/master/<对应脚本名> | bash`

### 例如:

#### 用于 Raspberry Pi OS 系统的脚本命令为：
`curl https://raw.githubusercontent.com/chaoyuejc/argon1-all/refs/heads/master/argon1.sh | bash`

#### 用于 CentOS 系统的脚本命令为：
`curl https://raw.githubusercontent.com/chaoyuejc/argon1-all/refs/heads/master/argon1_centos.sh | bash`


#### 用于 openEuler 系统的脚本命令为：
`curl https://raw.githubusercontent.com/chaoyuejc/argon1-all/refs/heads/master/argon1_openeuler.sh | bash`

## 异常问题
1. 问题： 在执行脚本时，使用pip3安装wheel的过程容易出现‘Read timed out.’的错误。
   解决方法： 命令行下先执行  pip install wheel  如果一次安装失败，可以多次尝试，因为是国外的网，速度比较慢，容易安装失败，安装成功后再重新执行脚本。



