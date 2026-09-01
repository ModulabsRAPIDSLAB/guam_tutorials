# GUAM Tutorials

**GUAM 문서 사이트 호스팅 저장소** · [English](#english)

## 사이트

**https://modulabsrapidslab.github.io/guam_tutorials/**

| 문서 | 한국어 | English |
|------|--------|---------|
| 소개 | [/ko/](https://modulabsrapidslab.github.io/guam_tutorials/ko/) | [/](https://modulabsrapidslab.github.io/guam_tutorials/) |
| 빠른 시작 | [보기](https://modulabsrapidslab.github.io/guam_tutorials/ko/tutorials/quickstart/) | [view](https://modulabsrapidslab.github.io/guam_tutorials/tutorials/quickstart/) |
| 벤치마크 실행 | [보기](https://modulabsrapidslab.github.io/guam_tutorials/ko/tutorials/benchmark/) | [view](https://modulabsrapidslab.github.io/guam_tutorials/tutorials/benchmark/) |
| TabularAutoML API | [보기](https://modulabsrapidslab.github.io/guam_tutorials/ko/reference/tabular-automl/) | [view](https://modulabsrapidslab.github.io/guam_tutorials/reference/tabular-automl/) |

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
| `main` | 이 README |
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

GUAM is a stacked-ensemble AutoML that ports the LightAutoML tabular architecture onto
NVIDIA RAPIDS (cuDF, cuPy, cuML), running the whole pipeline on the GPU.
Main repository: [ModulabsRAPIDSLAB/GUAM](https://github.com/ModulabsRAPIDSLAB/GUAM).

This repository holds build output only. The documentation sources live in `site-docs/` in
the GUAM repository; `gh-pages` is replaced wholesale on every deploy, so do not edit it
directly. Send documentation changes as pull requests against `site-docs/` in GUAM.
