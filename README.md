# GUAM Tutorials

**GUAM 문서 사이트 호스팅 저장소** · [English](#english)

## 사이트

**https://modulabsrapidslab.github.io/guam_tutorials/**

| 문서 | 한국어 | English |
|------|--------|---------|
| 소개 | [/ko/](https://modulabsrapidslab.github.io/guam_tutorials/ko/) | [/](https://modulabsrapidslab.github.io/guam_tutorials/) |
| 빠른 시작 | [보기](https://modulabsrapidslab.github.io/guam_tutorials/ko/tutorials/quickstart/) | [view](https://modulabsrapidslab.github.io/guam_tutorials/tutorials/quickstart/) |
| 벤치마크 실행 | [보기](https://modulabsrapidslab.github.io/guam_tutorials/ko/tutorials/benchmark/) | [view](https://modulabsrapidslab.github.io/guam_tutorials/tutorials/benchmark/) |
| Colab에서 벤치마크 실행 | [보기](https://modulabsrapidslab.github.io/guam_tutorials/ko/tutorials/colab-benchmark/) | [view](https://modulabsrapidslab.github.io/guam_tutorials/tutorials/colab-benchmark/) |
| 멀티-GPU | [보기](https://modulabsrapidslab.github.io/guam_tutorials/ko/guides/multi-gpu/) | [view](https://modulabsrapidslab.github.io/guam_tutorials/guides/multi-gpu/) |
| TabularAutoML API | [보기](https://modulabsrapidslab.github.io/guam_tutorials/ko/reference/tabular-automl/) | [view](https://modulabsrapidslab.github.io/guam_tutorials/reference/tabular-automl/) |

## 노트북

| 노트북 | 열기 |
|--------|------|
| OpenML × GUAM 벤치마크 — 설정 셀 하나 수정 후 모두 실행 | [Colab에서 열기](https://colab.research.google.com/github/ModulabsRAPIDSLAB/guam_tutorials/blob/main/notebooks/guam_openml_benchmark_colab.ipynb) |

사용법: [Colab에서 벤치마크 실행](https://modulabsrapidslab.github.io/guam_tutorials/ko/tutorials/colab-benchmark/)

## GUAM 이란

GPU-based Auto-ML for Robust Large Scale Computation. LightAutoML의 tabular AutoML
아키텍처를 NVIDIA RAPIDS(cuDF·cuPy·cuML)로 포팅한 Stacked Ensemble AutoML.
데이터 준비부터 앙상블까지 전 과정을 GPU 위에서 수행.

- 본체 저장소: [ModulabsRAPIDSLAB/GUAM](https://github.com/ModulabsRAPIDSLAB/GUAM)
- 라이선스: Apache-2.0
- 팀: 모두의연구소 RAPIDSLAB

## 이 저장소의 구성

이 저장소는 **빌드 산출물 전용**. 문서 원본은 GUAM 저장소의 `site-docs/` 에 있음.

| 브랜치 | 내용 |
|--------|------|
| `main` | 이 README |와 `notebooks/`(Colab 링크 대상 노트북)
| `gh-pages` | MkDocs 빌드 결과(HTML) — GitHub Pages가 서빙 |

```
GUAM/site-docs/*.md  →  mkdocs build  →  guam_tutorials:gh-pages  →  Pages
```

`gh-pages` 는 매 배포마다 통째로 교체되므로 직접 편집 금지. 문서 수정은 GUAM 저장소의
`site-docs/` 에서 PR로 진행.

## 로컬 미리보기

GUAM 저장소에서 실행.

```bash
uv sync --extra docs
uv run mkdocs serve
```

---

<a name="english"></a>

## English

**Hosting repository for the GUAM documentation site.**

Live site: **https://modulabsrapidslab.github.io/guam_tutorials/**
(English at `/`, Korean at `/ko/`.)

Notebook: [OpenML × GUAM benchmark — open in Colab](https://colab.research.google.com/github/ModulabsRAPIDSLAB/guam_tutorials/blob/main/notebooks/guam_openml_benchmark_colab.ipynb) · [how to use](https://modulabsrapidslab.github.io/guam_tutorials/tutorials/colab-benchmark/)

GUAM is a stacked-ensemble AutoML that ports the LightAutoML tabular architecture onto
NVIDIA RAPIDS (cuDF, cuPy, cuML), running the whole pipeline on the GPU.
Main repository: [ModulabsRAPIDSLAB/GUAM](https://github.com/ModulabsRAPIDSLAB/GUAM).

This repository holds build output and the public copy of the Colab notebooks. The documentation sources live in `site-docs/` in
the GUAM repository; `gh-pages` is replaced wholesale on every deploy, so do not edit it
directly. Send documentation changes as pull requests against `site-docs/` in GUAM.
