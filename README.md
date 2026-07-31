<div align="center">

# 🔥 OnePlus Kernels (KernelSU / ReSukiSU + SUSFS)

[![ReSukiSU](https://img.shields.io/badge/ReSukiSU-Supported-green)](https://github.com/ReSukiSU/ReSukiSU)
[![KernelSU](https://img.shields.io/badge/KernelSU-Supported-green)](https://kernelsu.org/)
[![SUSFS](https://img.shields.io/badge/SUSFS-Integrated-orange?logo=gitlab)](https://gitlab.com/simonpunk/susfs4ksu)

</div>

This is a personal fork of [WildKernels/OnePlus_KernelSU_SUSFS](https://github.com/WildKernels/OnePlus_KernelSU_SUSFS), with the root manager switched from KernelSU-Next to **ReSukiSU**, plus a handful of additional features ported over from other community projects (see [Credits & Upstream Projects](#-credits--upstream-projects) below).

---

## ⚠️ Disclaimer

Flashing this kernel will not void your warranty, but there is always a risk of bricking your device. Please make sure to:
- 💾 Back up your data
- 🧠 Understand the risks before proceeding

- I am **not responsible** for bricked devices, damaged hardware, or any issues that arise from using this kernel.

- **Please** do thorough research and fully understand the features added in this kernel before flashing it!

- By flashing this kernel, **YOU** are choosing to make these modifications. If something goes wrong, **do not blame me**!

<div align="center">
  
# **🚨 Proceed at your own risk!**

</div>

---

## 🔗 Additional Resources

- 🩹 [Kernel Patches](https://github.com/WildKernels/kernel_patches)
- ⚡ [Kernel Flasher](https://github.com/fatalcoder524/KernelFlasher)

---

## 📱 Device Compatibility

- Please verify the device compatibility before flashing here: [Compatibility_Info](https://github.com/WildKernels/OnePlus_KernelSU_SUSFS/blob/main/compatibility.md).

---

## ✨ Features

- 🔐 **KernelSU / ReSukiSU**: A root solution for Android GKI devices that works in kernel mode and grants root permission to userspace applications directly in kernel space
- 🥷 **SUSFS**: An addon root hiding kernel patches and userspace module for KernelSU
- 🛡️ **BBG**: LSM-based Baseband Guard security to protect critical device partitions. abl/efisp can be added to whitelist for efisp exploit devices.
- 🛠️ **HMBIRD SCX**: Scheduler extensions for SM8750/MT6991 devices
- 🖧 **BBRv1**: Improved TCP congestion control
- 🖧 **BBRv3**: Improved TCP congestion control
- 🚦 **CAKE and PIE qdisc Support**: Better Net Schedulers
- ✅ **LTO**: Link Time Optimisation enabled
- 🚀 **Optimisation patches**: Memory, I/O, CPU scheduler, network and other general tunings
- 🌐 **TTL Target Support**: Network packet manipulation
- 🧱 **IP Set & IPv6 NAT Support**: Advanced firewall capabilities and IPv6 NAT Support
- ⚡️ **TMPFS XATTR / POSIX ACL**: Extended TMPFS support for meta modules and Mountify
- </> **Unicode Bypass Fix**: Prevent path traversal and other detections using non-printable Unicode codepoints [Experimental]
- 🖥️ **Droidspaces Support**: Support Portable Linux containers to run full Linux environments.
- 🔃 **NTSync**: Provide high-performance, low-latency synchronization primitives compatible with the Windows NT kernel API
- 🔃 **LZ4 Update**: Replaces the in-kernel LZ4 implementation with a newer upstream version, ported from Numbersf/Action-Build

---

## 📋 Installation Instructions

For GKI installation, please follow the official guide:

📖 **[KernelSU Installation Guide](https://kernelsu.org/guide/installation.html)**

You can also find Installation instructions in the release notes.

---

## 🌟 Credits & Upstream Projects

**This fork wouldn't exist without these projects. Huge thanks to everyone below! ❤️**

<div align="center">

| 🔧 **Project** | 👨‍💻 **Author** | 🔗 **Link** | 📝 **Used for** |
|:---------------:|:----------------:|:-----------:|:-----------------|
| **WildKernels/OnePlus_KernelSU_SUSFS** | WildKernels | [![GitHub](https://img.shields.io/badge/GitHub-WildKernels-blue?style=flat-square&logo=github)](https://github.com/WildKernels/OnePlus_KernelSU_SUSFS) | Upstream base this fork builds on |
| **ReSukiSU** | ReSukiSU | [![GitHub](https://img.shields.io/badge/GitHub-ReSukiSU-blue?style=flat-square&logo=github)](https://github.com/ReSukiSU/ReSukiSU) | The root manager this fork uses |
| **huangdihd/OnePlus_ReSukiSU_SUSFS** | huangdihd | [![GitHub](https://img.shields.io/badge/GitHub-huangdihd-blue?style=flat-square&logo=github)](https://github.com/huangdihd/OnePlus_ReSukiSU_SUSFS) | Reference implementation for the KernelSU-Next → ReSukiSU swap |
| **Numbersf/Action-Build** (ReSukiSU branch) | Numbersf | [![GitHub](https://img.shields.io/badge/GitHub-Numbersf-blue?style=flat-square&logo=github)](https://github.com/Numbersf/Action-Build/tree/ReSukiSU) | LZ4 update & `PatchFakePatches.kts` SUBLEVEL-aware SUSFS compatibility shims |
| **KernelSU** | tiann | [![GitHub](https://img.shields.io/badge/GitHub-tiann-blue?style=flat-square&logo=github)](https://github.com/tiann/KernelSU) | Original KernelSU implementation |
| **SUSFS** | simonpunk | [![GitLab](https://img.shields.io/badge/GitLab-simonpunk-orange?style=flat-square&logo=gitlab)](https://gitlab.com/simonpunk/susfs4ksu.git) | Root hiding kernel patches |
| **SUSFS Module** | sidex15 | [![GitHub](https://img.shields.io/badge/GitHub-sidex15-blue?style=flat-square&logo=github)](https://github.com/sidex15) | SUSFS userspace module |
| **Baseband Guard** | vc-teahouse | [![GitHub](https://img.shields.io/badge/GitHub-vc--teahouse-blue?style=flat-square&logo=github)](https://github.com/vc-teahouse/Baseband-guard.git) | BBG partition protection |
| **Droidspaces** | ravindu644 | [![GitHub](https://img.shields.io/badge/GitHub-ravindu644-blue?style=flat-square&logo=github)](https://github.com/ravindu644/Droidspaces-OSS.git) | Portable Linux container support |

</div>

*If you contributed something used here and aren't listed, please let me know so I can credit you properly.* 🙏

---

## 💬 Support

If you encounter any issues or need help, feel free to:
- 🐛 Open an issue in this repository

