为了在树莓派4B上尝试使用不同的操作系统，但发现原有的Argon ONE用于控制电源按钮及风扇的脚本并不完全兼容。因此，我基于现有的脚本进行了相应的修改，并将这些修改后的脚本整合到了本项目中。这样一来，将来如果再遇到相同的操作系统时，就可以迅速地进行配置和使用。

本项目相关脚本专为 Argon ONE 在 Raspberry Pi 平台上使用，其功能在于控制电源按钮及风扇。该项目的目的是为了适配在 Raspberry Pi 上安装的各种操作系统类型。

|脚本名称| 来源                                                                         | 测试系统                             | 测试设备                   | 备注                                       |
|----|----------------------------------------------------------------------------|----------------------------------|------------------------|------------------------------------------|
|argon1.sh| [官网提供](https://download.argon40.com/argon1.sh)                             | 无                                | 无                      | 官方提供版本，仅搬运                               |
|argon1_centos.sh| [GitHub上tomjo/argonone-centos仓库](https://github.com/tomjo/argonone-centos) | CentOS 7 Kernel 5.4.56-v7l.1.el7 | Raspberry Pi 4 Model B | GitHub上tomjo/argonone-centos分享的脚本，仅搬运         |
|argon1_openeuler.sh| 无                                                                          | openEuler 24.03 (LTS)            | Raspberry Pi 4 Model B | 基于 GitHub上tomjo/argonone-centos分享的脚本改造而来 |

