# detect_box_ws

ROS 2 箱体检测与定位工作空间。以下概述基于当前本地保存的远程分支提交记录：

| 远程分支 | 主要内容 |
| --- | --- |
| `origin/main` | 基于 RealSense D435 和 AprilTag 的箱体位姿检测，包含服务接口和实机自启脚本。 |
| `origin/develop` | 使用 YOLO-World 检测箱体，结合深度点云和内壁约束估计箱体中心；包含 Jetson NX 自启部署及服务接口调整。 |
| `origin/docker` | 在开发版本基础上提供基于 RGB-D 话题的仿真检测、Docker 镜像和 Compose 部署，镜像发布至阿里云仓库。 |
| `origin/yolo26` | 在开发版本基础上采用 YOLOE-26 实例分割和掩膜点云定位，提供环境配置和自启部署，ROS Domain ID 为 21。 |
| `origin/22` | 基于 `yolo26`，增加 22 号机器的自启和 CycloneDDS 配置，ROS Domain ID 为 22。 |

各分支的具体构建和运行方法请查看对应分支中的说明文档。
