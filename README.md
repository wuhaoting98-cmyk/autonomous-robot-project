# Autonomous Robot Project

## Project Goal

基於 ROS2 建立自主移動機器人系統，
並透過 Discord 作為操作與監控介面。

## System Modules

| 模組 | Input | Output | Status |
|---|---|---|---|
| Camera | Camera Image | Image | 待確認 |
| IMU | 加速度、角速度 | IMU Data | 待確認 |
| Wheel Encoder | 輪速 | Wheel Odometry | 待確認 |
| VINS-Mono | Camera + IMU + Wheel Odometry | Robot Pose | 待研究 |
| EKF / Sensor Fusion | IMU + Wheel Odometry | Fused Odometry | 待研究 |
| YOLO | Camera Image | Obstacle Information | 待研究 |
| Hybrid A* | Pose + Goal + Map + Obstacles | Path | 待研究 |
| Pure Pursuit | Pose + Path | Steering / Speed | 待研究 |
| DeepRacer | Control Command | Vehicle Movement | 待確認 |
| Discord | User Command | Robot Command / Status | 待開發 |
| ROS2 | 各模組資料 | Topics / Messages | 核心通訊 |

## Current Progress

- [x] 整理各模組 Input / Output
- [x] 建立 GitHub 專案
- [ ] 建立 Ubuntu / ROS2 開發環境
- [ ] 確認 DeepRacer ROS2 通訊
- [ ] 建立 Discord ↔ ROS2 通訊
- [ ] 整合定位
- [ ] 整合障礙物感知
- [ ] 整合路徑規劃
- [ ] 整合車輛控制
