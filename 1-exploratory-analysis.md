---
title: "Exploratory Analysis"
layout: default
nav_order: 2
---
# 1. Exploratory Analysis: From Proof-of-Concept to Sophisticated Behavioral Understanding

## 1.1. Research Context & Motivation
Rainbow Agents is a two-player collaborative game designed to support learning of core computer science concepts such as loops, conditionals, and randomness. As an interactive exhibit, it was deployed at two U.S. science museums to explore informal, socially embedded learning through gameplay.

While museums are studied as unique learning environments, little research has examined how collaborative digital games, particularly those focused on computer science, operate in such settings. This study addresses that gap through large-scale behavioral analysis.

Our investigation was motivated by two fundamental questions:

**Individual & Collaborative Learning Dynamics**: When and how do critical behavioral shifts occur during both individual learning and collaborative interaction within gameplay?

**Computational Detection Methods**: What analytical approaches can reliably detect and characterize distinct behavioral patterns that emerge during these sessions?

The deployment yielded over 1.5 million interaction logs from 1,300+ sessions involving more than 3,000 players.

_Note: Exploratory analyses used strategic subsampling to manage computational load; specific sample sizes are detailed in each phase._

---
## 1.2. Primary Exploratory Question
How can we systematically identify and characterize behavioral transitions in collaborative CS learning gameplay using data-driven computational methods?

### Specific Exploratory Questions
1. **Change Point Detection**: Do z-score-based methods effectively capture meaningful behavioral transitions during collaborative CS learning?
2. **Feature Validation**: Which behavioral indicators extracted from change points show predictive value for learning outcomes, and how can these guide player state modeling?
3. **Player State Discovery**: What distinct behavioral states emerge when validated change point features are analyzed through dimensionality reduction?
4. **State Interpretation**: How do computationally-discovered player states map to interpretable learning behaviors and engagement patterns?
5. **Pattern Validation**: Do discovered behavioral states show consistent signatures when re-analyzed through change point detection?

---
## 1.3. Progressive Methodology
The exploratory analysis employed a **validate-then-elaborate** strategy to systematically moving from initial behavioral validation to sophisticated pattern discovery.

### [Phase 1: Proof of Concept](EA1-change-points.md)
**Goal**: Establish that z-score detected change points capture behaviorally meaningful signals


**Methods**:
- Apply event-level z-score detection (threshold = 2.0) using event rarity statistics
- Calculate behavioral shift density across temporal phases (0-4)
- Test predictive validity: Do change point patterns predict learning success?

**Validation Logic**: Before investing in complex pattern discovery, we first verify that our fundamental approach (z-score change detection) identifies changes that actually captures learning engagement.

*Addresses exploratory questions 1*


### [Phase 1.5: Predictive Validation](EA1.5-predictive-modeling.md) 
**Goal**: Test predictive validity of change point features
**Methods**: Logistic regression, MultinomialNB on temporal & events predictors
**Output**: Validated features for player state modeling

### Phase 2: Pattern Discovery (t-SNE)
**Goal**:  Discover distinct behavioral pathways by analyzing player trajectories through dimensionality reduction

### Phase 3: Pathway Interpretation (Grid-based Pathway Analysis)
**Goal**: Interpret t-SNE clusters as meaningful play states and learning progressions through grid-based pathway analysis

### Phase 4: Method Validation
**Goal**: Do pathway-based behavioral patterns show consistent change point signatures when re-analyzed?






[← Back to Research Overview](README.md) | [Next: Predictive Validation →](EA1.5-predictive-modeling.md)

---

## Quick Navigation to Detailed Analyses
- [EA1: Change Point Detection](EA1-change-points.md)
- [EA1.5: Predictive Validation](EA1.5-predictive-modeling.md) 
- [EA2: Spatial Behavioral Mapping](EA2-spatial-mapping.md)

