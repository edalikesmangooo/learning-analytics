---
title: "EA2: Play Tracing"
layout: default
nav_order: 5
---

[← Back to Predictive Validation](EA1.5-predictive-modeling.md) | [Next: Decoding t-SNE →](EA2.5-pathway-analysis.md)

# 2. Play Tracing Analysis

## Overview

* **Goal**: 
To reveal how player behavior evolves during collaborative gameplay by visualizing learning trajectories through a continuous behavioral state space. This approach enables systematic analysis of temporal learning patterns that traditional discrete metrics cannot capture.

Play tracing unlocks:
- **Strategy evolution tracking**: Observe how collaborative strategies form, shift, or stabilize throughout gameplay sessions
- **Learning pathway discovery**: Identify distinct behavioral progression patterns that lead to different learning outcomes
- **Comparative trajectory analysis**: Compare diverse play patterns within a unified, temporally grounded behavioral space

* **Questions**: What distinct behavioral pathways emerge when player trajectories are visualized through dimensionality reduction? How do learning trajectories differ between successful and unsuccessful sessions?

---

## Methodology
Player's gameplay are segmented into behavioral states, a feature-based representations of player activity over discrete time windows, capturing elements such as action types, interaction patterns, and collaborative dynamics. These high-dimensional behavioral states are embedded into 2D space using t-SNE, preserving local similarities in behavioral patterns. The resulting trajectories allow researchers to observe how players transition between different behavioral modes and analyze the temporal shape and rhythm of collaborative learning processes.

* **States**: Validated behavioral-temporal features from change points & predictive modeling (add feature list table)
* **t-SNE process**: Dimensionality reduction to map high-dimensional behavioral states to 2D space
* **Data**: Random sampled 167 players
* **Trajectory construction**: Sessions represented as sequential paths through t-SNE space using time-bin progression

---

## Key Findings *(visual/exploratory analysis)*

### Behavioral Space Emergence

* t-SNE reveals distinct behavioral regions in 2D space
* Visual examples showing different areas of behavioral space
* *(Focus: What does the overall landscape look like?)*
<iframe src="assets/images/phase2-tsne-plot1-s1475-SetA.html" 
        width="100%" 
        height="500" 
        frameborder="0">
</iframe>

### Trajectory Path Comparison

* Full achievement vs limited progress sessions follow visibly different pathways
* Visual comparison of trajectory shapes and patterns
* *(Focus: Do paths look different between groups?)*
<iframe src="assets/images/phase2-tsne-plot4-s1488-SetB.html" 
        width="100%" 
        height="500" 
        frameborder="0">
</iframe>
### Success Distribution Patterns

* Learning outcomes show spatial clustering in certain t-SNE regions
* Color-coded visualization mapping success groups to behavioral space
* *(Focus: Are there "success zones" and "struggle zones"?)*
<iframe src="assets/images/phase2-unified_behavioral_space.html" 
        width="100%" 
        height="500" 
        frameborder="0">
</iframe>

<iframe src="assets/images/phase2-unified_trajectory_overlay.html" 
        width="100%" 
        height="500" 
        frameborder="0">
</iframe>

---

## Discussion

* **What it tells us**: Behavioral trajectories exist, they differ by outcome, and occupy distinct spatial regions
* **What it doesn't tell us**: 
  t-SNE gives us visual patterns but they're hard to interpret -
- "There are different behavioral regions" → But what do they mean?
- "Full achievement paths look different" → But how specifically?
- "Players move through space" → But what are they actually doing?

## Next Steps
To answer these questions, we turn to grid-based pathway analysis for systematic interpretation of behavioral regions and transition patterns.