---
layout: page
title: HAIC Benchmark Suite
description: Evaluating human-AI collaboration from interaction logs — platform and open-source library (HumAIne, Horizon Europe)
img:
importance: 1
category: research
github: https://github.com/gfragi/haic-libs
---

The **HAIC Benchmark Suite** is a domain-agnostic platform for evaluating the quality of human-AI collaboration, developed within the Horizon Europe project [HumAIne](https://cordis.europa.eu/project/id/101120218) (GA 101120218).

Instead of asking only "is the model accurate?", it asks how well people and AI work *together*. From structured interaction logs it computes a set of collaboration metrics:

- **Trust proxy** — how often humans accept, override or correct AI outputs
- **Human-centeredness / cognitive-load proxy** and **effort loss** — the cost of the collaboration to the human
- **Adaptability** and **interaction frequency**
- **Surrogate similarity** — how closely a simulated user reproduces real behaviour

**Components**

- [`haic-libs`](https://github.com/gfragi/haic-libs): open-source (MIT) Python library, published as two packages — `haic-logging` (instrumentation and decision-log export) and `haic-metrics` (evaluation engine, metric profiles, windowed evaluation)
- An evaluation platform with dashboards, Node-RED integration flows, questionnaire (SUS) integration and a living ontology of collaboration events
- A probabilistic **surrogate-user simulation** framework, fitted on real sessions, whose output is schema-identical to real logs, so the same pipeline evaluates both

**Validation** — real pilots across smart-city public services, smart ticketing, smart energy (2D vs XR interfaces), healthcare and a RAG chatbot, plus a cross-domain study with MSc student teams.

**Read more** — [Evaluating Human-AI Collaboration: A Review and Methodological Framework (arXiv:2407.19098)](https://arxiv.org/abs/2407.19098)
