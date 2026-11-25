# 第一阶段环境记录

检测日期 2026-11-25。

| 项目 | 实测结果 |
| --- | --- |
| CPU | Intel Core i9-14900HX |
| GPU | NVIDIA GeForce RTX 5070 Laptop GPU，计算能力 12.0，Windows 驱动 621.24，显存 8151 MiB |
| WSL | Ubuntu 为 WSL2，发行版 Ubuntu 26.04 LTS，可通过 nvidia-smi 识别 GPU |
| WSL 内存 | 15 GiB 内存，4 GiB 交换空间 |
| 系统 Python | WSL 为 3.14.4，系统解释器未发现 pip 或 torch |
| Git | Windows 2.55.0.windows.3，WSL 2.53.0 |
| 存储 | Windows D 盘约 1047 GiB 可用 |

第一阶段候选仍为隔离的 Python 3.10 和 PyTorch cu128。WSL 的 nvidia-smi 通过只能确认驱动可见，CUDA 张量和模型推理还需实际验证。WSL 的 PATH 未找到 ffmpeg、ffprobe、nvcc 或 uv，亦未发现 /usr/local/cuda。安装媒体工具后需验证 FFmpeg 编解码。

