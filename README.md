# Video Magic Eraser

《智能计算系统》课程项目，研究视频目标及关联阴影的联合移除。

第一阶段从用户点击开始，用 SAM 2.1 Tiny 传播目标掩码，以 OpenCV 先打通修复与 MP4 导出，再接入 ProPainter。

- 成员 A 负责分割与关联阴影，入口目录为 src/segmentation 和 src/shadow_detection。
- 成员 B 负责修复与时序，入口目录为 src/inpainting、src/optical_flow 和 src/temporal_consistency。
- 视频预处理、管线、接口与 Demo 联合完成。
- 环境盘点见 [第一阶段环境记录](docs/progress/phase1-environment.md)。
