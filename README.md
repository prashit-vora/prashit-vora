<img src="assets/intro.gif" alt="Hi, I'm Prashit. Systems programming, deep learning, reinforcement learning, and AI security." width="1000" />

**Systems programming · Machine learning · Security**

I'm a [research intern working on adversarial robustness and neural network certification with DeepPoly](https://github.com/jeetrex17/deeppoly).

I work with C, C++, Python, and Go, with interests in deep learning, reinforcement learning, and AI security. I contribute fixes to open-source systems—from memory leaks in an RTOS to storage and API security.

## Open Source Contributions

### Eclipse ThreadX

*Real-time systems · C · ARM*

Contributed to the real-time operating system formerly known as Microsoft Azure RTOS.

- **Fixed a kernel-stack memory leak** when deleting user-mode module threads. In a Cortex-M3 QEMU reproduction, the original code exhausted memory after **18 create/delete cycles**; the fix completed **all 64 test cycles**. [Merged fix ↗](https://github.com/eclipse-threadx/threadx/pull/692)
- **Added Linux build support for 3 ARM SMP targets:** Cortex-A5, A7, and A9, using GNU and Arm Toolchain for Embedded. Verified that all three GNU sample images linked, alongside **45/45 passing LLVM example builds**. Validation covered compilation and linking; hardware execution was not tested. [Merged contribution ↗](https://github.com/eclipse-threadx/threadx/pull/674)

### Litestream

*Go · SQLite · Replication*

**Fixed a retention configuration mismatch.** Enabled `l0-retention: 0` to disable automatic deletion of compacted L0 files, matching the engine's existing behavior. Added regression tests confirming that zero is accepted and negative values are rejected.

[Merged fix ↗](https://github.com/benbjohnson/litestream/pull/1425)

### GeoLens

*Python · File-path security · API error handling*

- **Hardened local-storage path handling** by validating list prefixes before filesystem access. Added regression coverage for traversal, absolute paths, null bytes, and related containment cases; the containment suite passed **87 tests**. [Merged fix ↗](https://github.com/geolens-io/geolens/pull/1307)
- **Prevented internal error details from leaking** through the dataset-deletion API. Unexpected failures return a generic server error while full details remain in server logs, with regression coverage for that behavior. [Merged fix ↗](https://github.com/geolens-io/geolens/pull/1358)

## Tech Stack

| Category | Technologies |
| :--- | :--- |
| **Languages** | ![C](https://img.shields.io/badge/C-2563EB?style=flat-square&logo=c&logoColor=white) ![C++](https://img.shields.io/badge/C%2B%2B-2563EB?style=flat-square&logo=cplusplus&logoColor=white) ![Python](https://img.shields.io/badge/Python-2563EB?style=flat-square&logo=python&logoColor=white) ![Go](https://img.shields.io/badge/Go-2563EB?style=flat-square&logo=go&logoColor=white) ![Java](https://img.shields.io/badge/Java-2563EB?style=flat-square&logo=openjdk&logoColor=white) ![SQL](https://img.shields.io/badge/SQL-2563EB?style=flat-square) |
| **ML & Libraries** | ![PyTorch](https://img.shields.io/badge/PyTorch-16803C?style=flat-square&logo=pytorch&logoColor=white) ![NumPy](https://img.shields.io/badge/NumPy-16803C?style=flat-square&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/Pandas-16803C?style=flat-square&logo=pandas&logoColor=white) |
| **Databases** | ![SQLite](https://img.shields.io/badge/SQLite-B45309?style=flat-square&logo=sqlite&logoColor=white) ![PostgreSQL](https://img.shields.io/badge/PostgreSQL-B45309?style=flat-square&logo=postgresql&logoColor=white) |
| **Tools & Environment** | ![Git](https://img.shields.io/badge/Git-0E7490?style=flat-square&logo=git&logoColor=white) ![Linux](https://img.shields.io/badge/Linux-0E7490?style=flat-square&logo=linux&logoColor=white) ![Neovim](https://img.shields.io/badge/Neovim-0E7490?style=flat-square&logo=neovim&logoColor=white) ![tmux](https://img.shields.io/badge/tmux-0E7490?style=flat-square&logo=tmux&logoColor=white) |

## Achievements

- **Security research:** Reported **4 approved vulnerabilities** through the Wispr Flow bug bounty program, earning **$1,000**.
- **Codeforces:** **1519 peak rating (Specialist)**.
- **100% completion / Platinum:** Sekiro, Black Myth: Wukong, and Elden Ring.
