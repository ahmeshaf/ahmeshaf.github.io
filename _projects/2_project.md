---
layout: page
title: Event coreference resolution on figurative event phrases
description: Possible course project for incoming students to explore
img: assets/img/projects/analogies.png
importance: 2
category: nlp-course-project
---

Normal Example:
```
The Indian navy has <m> captured </m> 23 Somalian pirates .
```

Figurative Conversion:
```
The Indian navy's net of justice has <m> ensnared </m> 23 Somalian sea wolves.
```
- "net of justice" metaphorically describes the Indian navy's operations.
- "sea wolves" metaphorically represents the pirates, drawing a parallel with wolves which are often considered cunning and predatory creatures.

### Research Goals
- Reuse existing ECR datasets to augment with metaphorical version of the events.
- Create high-quality examples through multiple rounds of adjudications by also
  identifying standard and metaphorical versions of the events.
- Produce baseline results using existing methods. The goal here is produce
  a dataset that fail on simple heuristics and achieve a lower results on
  existing methods.
