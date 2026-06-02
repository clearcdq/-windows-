# Windows 漏洞利用集合

![License](https://img.shields.io/badge/License-MIT-blue.svg) ![Language](https://img.shields.io/badge/Language-Multiple-brightgreen) ![Status](https://img.shields.io/badge/Status-Active-success)

> 🚀 **免责声明**：本项目所涉及的技术、思路和工具仅供学习使用，任何人不得将其用于非法用途或未授权渗透测试，违者后果自行承担。

## 📋 项目概述

本仓库收集了常见的 **Windows 系统漏洞** 的分析资料、POC 代码和利用方法。包括系统提权漏洞、远程代码执行漏洞、信息泄露漏洞等多种类型。

## 🎯 主要内容

- 📚 **Windows 系统漏洞分析** - 详细的漏洞说明和原理
- 🛠️ **POC/EXP 代码** - 可复现的漏洞利用代码
- 📖 **技术文档** - 漏洞利用方法和防护建议
- 🔐 **安全加固脚本** - 常见端口封禁和系统加固脚本

## 📂 项目结构

```
-windows-/
├── README.md                 # 项目说明
├── exploits/                 # 漏洞利用代码
│   ├── local-privilege-escalation/   # 本地提权漏洞
│   ├── rce/                          # 远程代码执行漏洞
│   └── info-disclosure/              # 信息泄露漏洞
├── analysis/                 # 漏洞分析文档
├── tools/                    # 辅助工具和脚本
└── docs/                     # 参考文档和资源
```

## 🚀 快速开始

### 前置要求

- Windows 操作系统（7/8/10/11）
- 编译工具（Visual Studio 或 MinGW）
- Python 3.x（部分脚本需要）

### 使用示例

```bash
# 克隆仓库
git clone https://github.com/clearcdq/-windows-.git
cd -windows-

# 编译 C/C++ 漏洞利用程序
gcc exploit.c -o exploit.exe

# 运行测试
./exploit.exe
```

## 📚 涵盖的漏洞类型

| 漏洞类型 | 示例 CVE | 影响版本 | 难度 |
|--------|---------|--------|------|
| 本地提权 | CVE-2021-1732 | Win7-Win11 | ⭐⭐⭐ |
| 远程代码执行 | CVE-2021-44228 | Win Server | ⭐⭐⭐⭐ |
| 信息泄露 | CVE-2021-21224 | Win10 | ⭐⭐ |
| 权限提升 | CVE-2021-1647 | Win7-Win10 | ⭐⭐⭐ |
| 蓝屏漏洞 | CVE-2021-34481 | Win10-Win11 | ⭐⭐ |

## 🔧 工具和资源

### 相关工具

- [Metasploit Framework](https://www.metasploit.com/) - 渗透测试框架
- [Exploit Database](https://www.exploit-db.com/) - 公开漏洞集合
- [NVD - National Vulnerability Database](https://nvd.nist.gov/) - 官方漏洞数据库

### 参考资源

- [Microsoft Security Updates](https://portal.msrc.microsoft.com/)
- [OWASP Top 10](https://owasp.org/www-project-top-ten/)

## 📝 文献和参考

1. Windows Internals Book
2. Defcon Talks - Windows Exploitation
3. Blackhat Conference Presentations

## ⚠️ 安全建议

为防止系统被攻击，建议采取以下措施：

1. **及时更新补丁** - 定期安装 Windows 安全更新
2. **最小权限原则** - 使用最低必要的权限运行程序
3. **防火墙配置** - 封禁危险端口（RDP 3389、SMB 445 等）
4. **安全软件** - 安装信誉良好的杀毒软件
5. **监控审计** - 启用系统日志记录和审计

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

### 贡献方式

1. Fork 本仓库
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 开启 Pull Request

## 📞 联系方式

- **GitHub Issues** - 提交问题和建议
- **Email** - clearcdq@gmail.com

## 📄 许可证

本项目采用 **MIT 许可证**，详见 [LICENSE](LICENSE) 文件。

## 🙏 致谢

感谢所有贡献者和安全研究人员的支持！

---

**最后更新**: 2026年6月  
**维护者**: [@clearcdq](https://github.com/clearcdq)
