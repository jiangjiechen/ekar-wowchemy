---
# An instance of the Blank widget.
# Documentation: https://wowchemy.com/docs/getting-started/page-builder/
widget: blank

# Activate this widget? true/false
active: true

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 40

title: Leaderboard
subtitle:

design:
  columns: "1"
  background:
    image: 
    image_darken: 1.0
    image_parallax: true
    image_position: center
    image_size: cover
    text_color_light: 
  spacing:
    padding: ["20px", "0", "20px", "0"]
---

Please submit and evaluate your results on the test sets at the publicly available [E-KAR leaderboard](https://eval.ai/web/challenges/challenge-page/1671/overview) hosted at EvalAI.

Note that the leaderboard only evaluates Analogical QA and Rationalized Analogical QA tasks, in order to avoid using unreliable automatic metrics for evaluating text generation (i.e., explanations).
See the [E-KAR leaderboard](https://eval.ai/web/challenges/challenge-page/1671/overview) for participation details.



## Baseline Results


![results](/uploads/results.jpg)

Table 1: <i>Accuracy results on previous analogy tasks and the QA task in E-KAR (<b>v1.0 -> v1.1</b>). E-KAR (H/E) denotes HARD or EASY mode of analogical QA. Method† is not tuned. PLM-b or PLM-l denote base or large version, respectively.</i>