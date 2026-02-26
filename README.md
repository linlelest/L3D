# L3D 🎥 3D 影视级智能轨道制片平台 (PRO版)

[![GitHub license](https://img.shields.io/github/license/linlelest/L3D)](https://github.com/linlelest/L3D/blob/main/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/linlelest/L3D)](https://github.com/linlelest/L3D/stargazers)
[![Three.js](https://img.shields.io/badge/Powered%20by-Three.js-black)](https://threejs.org/)

> **L3D** 是一个基于 Web 的轻量级 3D 场景搭建与运镜录制工具。它无需安装庞大的专业软件，即可在浏览器中导入工业/通用模型，绘制复杂的摄像机轨迹，并录制高达 4K 分辨率的演示视频。

---

## ✨ 预览 / Gallery

| 场景搭建与导入 | 智能轨道绘制 |
| :---: | :---: |
| ![场景展示](https://github.com/linlelest/L3D/blob/main/ex_1.png) | ![轨道绘制](https://github.com/linlelest/L3D/blob/main/ex_2.png) |
| **功能描述：** 支持 STP/STL 导入及材质快速替换 | **功能描述：** 支持直线、曲线及多点贝塞尔曲线 |

| 运镜与锁焦 | 高清录制输出 |
| :---: | :---: |
| ![运镜效果](https://github.com/linlelest/L3D/blob/main/ex_3.gif) | ![录制预览](https://github.com/linlelest/L3D/blob/main/ex_3.gif) |
| **功能描述：** 智能物体锁焦与关键帧平滑过渡 | **功能描述：** 支持 H.264/H.265 编码及 4K 导出 |


---

## 🚀 核心功能

*   **🛠️ 强大的模型兼容性**：内置 OCCT CAD 内核，原生支持 **.STP / .STEP** 工业模型及 **.STL** 格式导入。
*   **✒️ 自由轨迹绘制**：
    *   支持自由手绘、两点直线、三点抛物线、**多点成弧**等多种布线方式。
    *   可视化调整控制点，实时预览路径。
*   **🎥 智能摄影机系统**：
    *   **自动锁焦**：设定区间让镜头强制追踪特定模型或空间向量。
    *   **平滑过渡**：可调节的镜头平滑度（Damping）。
    *   **朝向控制**：支持沿轨道前方、追踪最近物体、固定视角或自定义向量。
*   **⚡ 变速与时间轴**：
    *   在轨道任意位置添加 **加速 / 减速 / 停顿** 节点。
    *   自定义单圈时长（支持秒/分单位）。
*   **🎬 影视级导出**：
    *   支持 1080P (横/竖屏) 至 4K 分辨率。
    *   支持 H.264 / H.265 / AV1 编码录制（基于浏览器能力）。
    *   **MP4 / WebM** 格式直出。
*   **🎨 快捷外观**：一键模型调色、3D 立体文字生成（支持中英文）。

---

## 💻 快速开始

### 方式一：直接运行
1. 克隆本项目：
   ```bash
   git clone https://github.com/linlelest/L3D.git
   ```
2. 推荐使用 VS Code 安装 **Live Server** 插件，右键 `index.html` 选择 "Open with Live Server"。
3. 或者直接将文件部署到任意静态 Web 服务器。


#### CORS 插件说明 (重要)</span>**
由于浏览器安全策略，在线获取中文字体或加载本地纹理时可能会遇到跨域问题。
建议在 Chrome / Edge 浏览器中安装 "Allow CORS" 相关插件，以便完整体验中文字体生成功能。

[Edge版插件](https://microsoftedge.microsoft.com/addons/detail/allow-cors-accesscontro/bhjepjpgngghppolkjdhckmnfphffdag)
[Chrome版插件](https://chromewebstore.google.com/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf)

### 温馨提示：插件来自第三方，仅供参考，本人不提供任何安全性担保，任何因此插件给您造成的损失不由本人承担！

### 方式二：
[在线体验链接](https://sparkling-starship-9f3e98.netlify.app/)

---

## 🎮 操作指南

### 快捷键
*   `T`：移动模式 (Translate)
*   `R`：旋转模式 (Rotate)
*   `S`：缩放模式 (Scale)
*   `Del`：删除选中的模型或节点
*   `Esc`：停止录制/播放

### 鼠标操作
*   **左键**：选择模型 / 绘制轨迹
*   **右键**：平移视角
*   **滚轮**：指哪缩哪 (以鼠标为中心缩放)
*   **左键按住拖拽**：旋转视角

---

## 🛠️ 技术栈

*   [Three.js](https://threejs.org/) - 3D 渲染引擎
*   [occt-import-js](https://github.com/kovacsv/occt-import-js) - STEP/STP 文件解析
*   HTML5 Canvas & MediaRecorder API

---

## 🤝 贡献

欢迎提交 Issue 或 Pull Request！如果您有更好的想法，请随时联系。

## 📄 开源协议

MIT License
