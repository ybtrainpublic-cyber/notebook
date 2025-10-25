# Jupyter Notebook

![Github Actions Status](https://github.com/jupyter/notebook/workflows/Build/badge.svg)
[![Documentation Status](https://readthedocs.org/projects/jupyter-notebook/badge/?version=latest)](https://jupyter-notebook.readthedocs.io/en/latest/?badge=latest)
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jupyter/notebook/main?urlpath=tree)
[![Gitpod](https://img.shields.io/badge/gitpod_editor-open-blue.svg)](https://gitpod.io/#https://github.com/jupyter/notebook)
<p align="center">
  <img src="https://raw.githubusercontent.com/jupyter/notebook/main/docs/source/_static/notebook_logo.png" alt="Jupyter Notebook Logo" width="150"/>
</p>

The Jupyter notebook is a web-based notebook environment for interactive
computing.
**Jupyter Notebook**은 웹 기반의 대화형 컴퓨팅 플랫폼입니다. 노트북 문서를 통해 라이브 코드, 수식, 시각화, 설명 텍스트를 함께 작성하고 공유할 수 있습니다.

![Jupyter notebook example](docs/resources/running_code_med.png 'Jupyter notebook example')
이 저장소는 **Jupyter Notebook 7** 및 이후 버전을 위한 것입니다. Notebook 7은 [JupyterLab](https://github.com/jupyterlab/jupyterlab)을 기반으로 구축되어, 기존의 클래식한 노트북 사용자 경험을 유지하면서도 더욱 현대적이고 유연한 아키텍처를 제공합니다.

## Maintained versions
## 주요 특징

We maintain the **two most recently released major versions of Jupyter Notebook**,
Classic Notebook v6 and Notebook v7. Notebook v5 is no longer maintained.
All Notebook v5 users are strongly advised to upgrade to Classic Notebook v6 as soon as possible.
*   **웹 기반 인터페이스**: 브라우저에서 코드를 작성하고 실행할 수 있습니다.
*   **다양한 언어 지원**: Python, R, Julia 등 수십 개의 프로그래밍 언어를 지원합니다.
*   **데이터 시각화**: Matplotlib, Plotly, Bokeh 등 다양한 라이브러리와 통합하여 데이터를 시각화할 수 있습니다.
*   **Markdown 지원**: 서식 있는 텍스트와 LaTeX 수식을 사용하여 풍부한 문서를 작성할 수 있습니다.
*   **확장성**: JupyterLab 확장 기능을 통해 IDE와 유사한 기능을 추가할 수 있습니다.

Upgrading to Notebook v7 may require more work, if you use custom extensions, as extensions written
for Notebook v5 or Classic Notebook v6 are not compatible with Notebook v7.
## 설치

### Notebook v7
Python 3.9 이상 버전이 필요합니다.

The newest major version of Notebook is based on:
`pip`를 사용하여 Jupyter Notebook을 설치할 수 있습니다:

- JupyterLab components for the frontend
- Jupyter Server for the Python server
```bash
pip install notebook
```

This represents a significant change to the `jupyter/notebook` code base.
또는 `conda`를 사용하는 경우:

To learn more about Notebook v7: https://jupyter.org/enhancement-proposals/79-notebook-v7/notebook-v7.html

### Classic Notebook v6

Maintenance and security-related issues [only](https://github.com/jupyter/notebook-team-compass/issues/5#issuecomment-1085254000) are now being addressed in the [`6.5.x`](https://github.com/jupyter/notebook/tree/6.5.x) branch.
It depends on [`nbclassic`](https://github.com/jupyter/nbclassic) for the HTML/JavaScript/CSS assets.

New features and continuous improvement is now focused on Notebook v7 (see section above).

If you have an open pull request with a new feature or if you were planning to open one, we encourage switching over to the Jupyter Server and JupyterLab architecture, and distribute it as a server extension and / or JupyterLab prebuilt extension. That way your new feature will also be compatible with the new Notebook v7.

## Jupyter notebook, the language-agnostic evolution of IPython notebook

Jupyter notebook is a language-agnostic HTML notebook application for
Project Jupyter. In 2015, Jupyter notebook was released as a part of
The Big Split™ of the IPython codebase. IPython 3 was the last major monolithic
release containing both language-agnostic code, such as the _IPython notebook_,
and language specific code, such as the _IPython kernel for Python_. As
computing spans across many languages, Project Jupyter will continue to develop the
language-agnostic **Jupyter notebook** in this repo and with the help of the
community develop language specific kernels which are found in their own
discrete repos.

- [The Big Split™ announcement](https://blog.jupyter.org/the-big-split-9d7b88a031a7)
- [Jupyter Ascending blog post](https://blog.jupyter.org/jupyter-ascending-1bf5b362d97e)

## Installation

You can find the installation documentation for the
[Jupyter platform, on ReadTheDocs](https://jupyter.readthedocs.io/en/latest/install.html).
The documentation for advanced usage of Jupyter notebook can be found
[here](https://jupyter-notebook.readthedocs.io/en/latest/).

For a local installation, make sure you have
[pip installed](https://pip.readthedocs.io/en/stable/installing/) and run:

```bash
pip install notebook
conda install -c conda-forge notebook
```

## Usage - Running Jupyter notebook
## 실행

### Running in a local installation
터미널에서 다음 명령어를 실행하여 Jupyter Notebook을 시작하세요:

Launch with:

```bash
jupyter notebook
```

### Running in a remote installation
이 명령은 웹 브라우저에서 Jupyter Notebook 인터페이스를 자동으로 엽니다.

You need some configuration before starting Jupyter notebook remotely. See [Running a notebook server](https://jupyter-server.readthedocs.io/en/latest/operators/public-server.html).
## JupyterLab 또는 클래식 Notebook (v6) 사용하기

## Development Installation
### JupyterLab

See [`CONTRIBUTING.md`](CONTRIBUTING.md) for how to set up a local development installation.
JupyterLab은 Jupyter의 차세대 사용자 인터페이스입니다. Notebook 7과 함께 자동으로 설치되며, URL의 `/tree`를 `/lab`으로 변경하여 언제든지 JupyterLab으로 전환할 수 있습니다.

## Contributing
### 클래식 Notebook (v6)

If you are interested in contributing to the project, see [`CONTRIBUTING.md`](CONTRIBUTING.md).
이전 버전(6.x)의 클래식 Notebook 환경을 선호하신다면, `nbclassic` 패키지를 설치하여 사용할 수 있습니다.

## Community Guidelines and Code of Conduct
```bash
pip install nbclassic
```

This repository is a Jupyter project and follows the Jupyter
[Community Guides and Code of Conduct](https://jupyter.readthedocs.io/en/latest/community/content-community.html).
설치 후 `jupyter nbclassic` 명령어로 실행할 수 있습니다.

## Resources
## 기여

- [Project Jupyter website](https://jupyter.org)
- [Online Demo at jupyter.org/try](https://jupyter.org/try)
- [Documentation for Jupyter notebook](https://jupyter-notebook.readthedocs.io/en/latest/)
- [Korean Version of Installation](https://github.com/ChungJooHo/Jupyter_Kor_doc/)
- [Documentation for Project Jupyter](https://jupyter.readthedocs.io/en/latest/index.html)
- [Issues](https://github.com/jupyter/notebook/issues)
- [Technical support - Jupyter Google Group](https://discourse.jupyter.org/)
Jupyter Notebook 개발에 기여하고 싶으신가요? 언제나 환영입니다! 자세한 내용은 기여 가이드(CONTRIBUTING.md)를 참고해 주세요.

## About the Jupyter Development Team
## 변경 사항

The Jupyter Development Team is the set of all contributors to the Jupyter project.
This includes all of the Jupyter subprojects.
각 릴리스의 자세한 변경 사항은 CHANGELOG.md 파일에서 확인할 수 있습니다.

The core team that coordinates development on GitHub can be found here:
https://github.com/jupyter/.
## 라이선스

## Our Copyright Policy
Jupyter Notebook은 BSD 3-Clause 라이선스에 따라 배포됩니다.

Jupyter uses a shared copyright model. Each contributor maintains copyright
over their contributions to Jupyter. But, it is important to note that these
contributions are typically only changes to the repositories. Thus, the Jupyter
source code, in its entirety is not the copyright of any single person or
institution. Instead, it is the collective copyright of the entire Jupyter
Development Team. If individual contributors want to maintain a record of what
changes/contributions they have specific copyright on, they should indicate
their copyright in the commit message of the change, when they commit the
change to one of the Jupyter repositories.
---

With this in mind, the following banner should be used in any source code file
to indicate the copyright and license terms:

```
# Copyright (c) Jupyter Development Team.
# Distributed under the terms of the Modified BSD License.
```
더 궁금한 점이 있으시면 언제든지 질문해 주세요!
