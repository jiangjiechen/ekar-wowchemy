---
# An instance of the Blank widget.
# Documentation: https://wowchemy.com/docs/getting-started/page-builder/
widget: blank

# Activate this widget? true/false
active: true

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 30

title: About E-KAR
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
The ability to recognize analogies is fundamental to human cognition. Existing benchmarks to test word analogy do not reveal the underneath process of analogical reasoning of neural models. 

Holding the belief that models capable of reasoning should be right for the right reasons, we propose a first-of-its-kind Explainable Knowledge-intensive Analogical Reasoning benchmark (E-KAR). 
Our benchmark consists of 1,655 (in **Chinese**) and 1,251 (in **English**) problems sourced from **the Civil Service Exams**, which require intensive background knowledge to solve. 
More importantly, we design a **free-text explanation scheme** to explain whether an analogy should be drawn, and manually annotate them for *each and every question and candidate answer*.


## Data Instance

> **Query**: 
> 
> - tea: teapot: teacup
> 
> **Candidate Answers**: 
> 
> - A) passenger: bus: taxi
>  
> - B) magazine: bookshelf: reading room
> 
> - C) talents: school : enterprise
> 
> - D) textbooks: bookstore: printing factory
>  
> **Answer**: C
> 
> **Explanation for Query**:
> 
> - $E_Q$: Both "teapot" and "teacup" are containers for holding "tea". After the "tea" is brewed in the "teapot", it is transported into the "teacup".
> 
> **Explanation for Candidate Answers**:
> 
> - $E_A$: "Passengers" do not need to be transported into "taxi" after taking a "bus". "Taxi" and "bus" are different ways of transportation.
> 
> - $E_B$: The "bookshelf" is in the "reading room".
> 
> - $E_C$: Both "school" and "enterprise" are organizations. After "talents" are educated in "school", they are transported into "enterprise".
> 
> - $E_D$: After "textbooks" are printed in the "printing factory", they are sold in a "bookstore". But the terms order is inconsistent with the query.

## How to Load the Dataset?

```python3
import datasets   # 🤗
ekar_zh = datasets.load_dataset('Jiangjie/ekar_chinese')
ekar_en = datasets.load_dataset('Jiangjie/ekar_english')
```

## Visualizing Analogical Reasoning

![ekar-example](/uploads/ekar-example.jpg)

