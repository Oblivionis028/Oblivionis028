<p align="right">
  <a href="./README.md">简体中文</a> · <strong>English</strong>
</p>

<h1 align="center">Yuxuan Luo · Tomorin</h1>

<p align="center">
  <strong>Biotechnology &amp; Life Sciences · Bioinformatics · Deep Learning</strong>
</p>

<p align="center">
  <a href="https://github.com/Oblivionis028">@Oblivionis028</a> ·
  <a href="https://orcid.org/0009-0005-3544-1492">ORCID: 0009-0005-3544-1492</a>
</p>

<p align="center">
  <a href="https://github.com/biopython/biopython/pull/5382"><img src="https://img.shields.io/badge/Biopython-Contributor-2E8B57?style=flat-square" alt="Biopython contributor" /></a>
  <img src="https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/R-276DC3?style=flat-square&logo=r&logoColor=white" alt="R" />
  <img src="https://img.shields.io/badge/MATLAB-FF8000?style=flat-square" alt="MATLAB" />
  <img src="https://img.shields.io/badge/YOLO-00FFFF?style=flat-square&logo=yolo&logoColor=black" alt="YOLO" />
  <img src="https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black" alt="Linux" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />
</p>

I build bioinformatics workflows and animal behavior analysis tools around practical questions in the life sciences, with an emphasis on reproducibility and verifiable evidence.

## Open Source · Biopython

**My first code contribution to Biopython, [PR #5382](https://github.com/biopython/biopython/pull/5382), was merged into `master` in October 2026.**

[Biopython](https://github.com/biopython/biopython) is an open-source collection of Python tools for biological computation. This contribution addressed a warning that incorrectly suggested users were importing Biopython from inside its source tree in some environments.

- **Diagnosis:** A `pyproject.toml` in the parent directory of the `Bio` package does not reliably identify a source-tree import. The existing detection logic also relied on `biopython.egg-link`, which modern editable installs no longer use.
- **Change:** Removed the unreliable source-tree detection and its import-time warning, while preserving `BiopythonWarning` and its subclasses for use by other modules.
- **Validation:** Reproduced the issue and tested the change locally. The [CI run on the merged commit](https://github.com/biopython/biopython/actions/runs/39313448320) completed with **39/39 jobs successful**, including test jobs on Linux, Windows, macOS, and PyPy.

Credited as **Yuxuan Luo** in [CONTRIB.rst](https://github.com/biopython/biopython/blob/f68b896031088a8ad11ae49f5e903d49228fd61f/CONTRIB.rst#L389) and acknowledged as a first-time contributor in [NEWS.rst](https://github.com/biopython/biopython/blob/f68b896031088a8ad11ae49f5e903d49228fd61f/NEWS.rst#L31).

[Related issue #5294](https://github.com/biopython/biopython/issues/5294) · [Merged commit f68b896](https://github.com/biopython/biopython/commit/f68b896031088a8ad11ae49f5e903d49228fd61f)

## Featured Projects

| Project | Technologies & Tools | Description |
| --- | --- | --- |
| [Fish Tracking & 3D Behavior Analysis](https://github.com/Oblivionis028/ocellaris-fish-tracking-yolo-bytetrack) | Python · YOLO26s · ByteTrack · Ultralytics · DLT | A workflow for experimental clownfish videos, covering fish/reflection detection, multi-object tracking, dual-view 3D trajectory reconstruction, and behavioral metric extraction. |
| [Collinearity & Ka/Ks Analysis Pipeline](https://github.com/Oblivionis028/bioinfo-collinearity-kaks-pipeline) | Python · Bash · DIAMOND · MCScanX · TBtools-II · gffread | A reusable bioinformatics workflow for collinearity input preparation, target gene-pair filtering, CDS extraction, and basic quality checks, with guidance for subsequent Ka/Ks estimation. |
| [Literature Evidence Synthesis](https://github.com/Oblivionis028/literature-evidence-synthesis-skill) | Python · Codex Skill · PDF | A literature-review tool for multiple research fields, supporting PDF page-level evidence verification, study-design-specific appraisal, evidence matrices, and cross-paper synthesis reports. |

## GitHub Activity

<p align="center">
  <img src="https://raw.githubusercontent.com/Oblivionis028/Oblivionis028/main/metrics.plugin.isocalendar.svg" alt="Yuxuan Luo's GitHub isometric contribution calendar" />
</p>
