<p align="right">
  <strong>简体中文</strong> · <a href="./README.EN.md">English</a>
</p>

<h1 align="center">Yuxuan Luo · Tomorin</h1>

<p align="center">
  <strong>生物技术与生命科学 · 生物信息学 · 深度学习</strong>
</p>

<p align="center">
  <a href="https://github.com/Oblivionis028">@Oblivionis028</a> ·
  <a href="https://orcid.org/0009-0005-3544-1492">ORCID: 0009-0005-3544-1492</a>
</p>

<p align="center">
  <a href="https://github.com/biopython/biopython/pull/5382"><img src="https://img.shields.io/badge/Biopython-Contributor-2E8B57?style=flat-square" alt="Biopython 贡献者" /></a>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" alt="R" />
  <img src="https://img.shields.io/badge/MATLAB-FF8000?style=flat-square" alt="MATLAB" />
  <img src="https://img.shields.io/badge/YOLO-00FFFF?style=flat-square&logo=yolo&logoColor=black" alt="YOLO" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />
</p>

我围绕生命科学中的具体问题，编写生物信息学流程、开发动物行为分析工具，也关注科研过程中的可复现性与证据核查。

## 开源贡献 · Biopython

**2026 年 10 月，我的首个 Biopython 代码贡献 [PR #5382](https://github.com/biopython/biopython/pull/5382) 已合并至 `master`。**

[Biopython](https://github.com/biopython/biopython) 是用于生物学计算的 Python 开源工具库。这次贡献修复了 `import Bio` 在部分环境中错误提示用户“正在源码目录中导入 Biopython”的问题。

- **问题定位：** `Bio` 包父目录中存在 `pyproject.toml`，不足以证明用户正在源码目录中运行；原先依赖 `biopython.egg-link` 的检测也不适配现代可编辑安装。
- **代码修改：** 移除不可靠的源码目录判断及相应的导入时警告，保留 `BiopythonWarning` 及其子类，供其他模块继续使用。
- **测试验证：** 完成本地复现与测试；合并提交的 [CI 运行](https://github.com/biopython/biopython/actions/runs/39313448320) 中 **39/39 个任务成功**，其中包含 Linux、Windows、macOS 和 PyPy 的测试任务。

贡献以 **Yuxuan Luo** 记入 [CONTRIB.rst](https://github.com/biopython/biopython/blob/f68b896031088a8ad11ae49f5e903d49228fd61f/CONTRIB.rst#L389)，并在 [NEWS.rst](https://github.com/biopython/biopython/blob/f68b896031088a8ad11ae49f5e903d49228fd61f/NEWS.rst#L31) 中标注为首次贡献。

[相关问题 #5294](https://github.com/biopython/biopython/issues/5294) · [合并提交 f68b896](https://github.com/biopython/biopython/commit/f68b896031088a8ad11ae49f5e903d49228fd61f)

## 精选项目

| 项目 | 技术与工具 | 简介 |
| --- | --- | --- |
| [鱼类跟踪与三维行为分析](https://github.com/Oblivionis028/ocellaris-fish-tracking-yolo-bytetrack) | Python · YOLO26s · ByteTrack · Ultralytics · DLT | 面向小丑鱼实验视频，涵盖鱼体与反射识别、多目标跟踪、双视角三维轨迹重建及行为指标提取。 |
| [共线性与 Ka/Ks 分析流程](https://github.com/Oblivionis028/bioinfo-collinearity-kaks-pipeline) | Python · Bash · DIAMOND · MCScanX · TBtools-II · gffread | 可复用的生物信息学流程，覆盖共线性分析的输入准备、目标基因对筛选、CDS 提取与基础质检，并衔接 Ka/Ks 估算。 |
| [文献证据综合](https://github.com/Oblivionis028/literature-evidence-synthesis-skill) | Python · Codex Skill · PDF | 面向不同学科的文献阅读工具，支持 PDF 页码级证据复核、与研究设计对应的质量评价、证据矩阵及跨文献综合报告。 |

## GitHub 活动

<p align="center">
  <img src="https://raw.githubusercontent.com/Oblivionis028/Oblivionis028/main/metrics.plugin.isocalendar.svg" alt="Yuxuan Luo 的 GitHub 等距提交日历" />
</p>
