---
# An instance of the Blank widget.
# Documentation: https://wowchemy.com/docs/getting-started/page-builder/
widget: blank

# Activate this widget? true/false
active: true

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 35

title: Shared Tasks in E-KAR
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





There are altogether `8` task settings: `2 shared tasks` * `2 task modes` * `2 languages`.

## E-KAR supports two shared tasks: 
- `Analogical QA`: The dataset can be used to train a model for analogical reasoning in the form of multiple-choice QA.
- `Explanation Generation`: The dataset can be used to generate free-text explanations to rationalize analogical reasoning.

## E-KAR supports two task modes: 
- `EASY mode`: where query explanation ($E_Q$) can be used as part of the input.
- `HARD mode`: no explanation is allowed as part of the input.

## E-KAR supports two languages:
- `Chinese version`: 1,655 problems and 8,275 sentences of explanations, sourced from Civil Service Exams of China with manually annotated explanations.
  - Train split: 1155
  - Validation split: 165
  - Blind test split: 335
- `English version`: 1,251 problems and 6,255 sentences of explanations, translated from Chinese version with culture-specific samples removed or rewritten.
  - Train split: 870
  - Validation split: 119
  - Blind test split: 262

