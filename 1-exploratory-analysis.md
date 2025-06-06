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
How can we systematically identify and characterize behavioral transitions in collaborative CS learning gameplay using computational methods grounded in learning theory?

### Specific Exploratory Questions
1. **Change Point Detection**: Do z-score-based methods effectively capture explore-refine-tinker learning transitions predicted by CS education theory?

2. **Feature Validation**: Which behavioral indicators extracted from change points show predictive value for learning outcomes?

3. **Pattern Discovery**: What distinct behavioral pathways emerge when player trajectories are analyzed through dimensionality reduction?

4. **Pathway Interpretation**: How do computationally-discovered clusters map to interpretable play states and learning progressions?

5. **Method Validation**: Do pathway-based behavioral patterns show consistent change point signatures when re-analyzed?

---
## 1.3. Progressive Methodology
The exploratory analysis employed a **validate-then-elaborate** strategy to systematically moving from initial behavioral validation to sophisticated pattern discovery.

### Phase 1: Proof of Concept
**Goal**: Establish that z-score detected change points capture behaviorally meaningful signals

**Methods**:
- Apply theory-driven z-score detection (explore-refine-tinker transitions)
- Extract basic behavioral features from detected change points
- Test predictive validity: Do change point features predict learning success?

**Validation Logic**: Before investing in complex pattern discovery, we first verify that our fundamental approach (z-score change detection) identifies changes that actually matter for learning outcomes.

*Addresses exploratory questions 1 & 2*

### Phase 2: Pattern Discovery  
**Goal**: Characterize what the validated changes represent

**Methods**:
- Extract rich behavioral features from **validated** change points
- Apply t-SNE for dimensionality reduction and clustering
- Grid-based pathway analysis to interpret clusters

**Discovery Logic**: Now that we know change detection works, what are the actual behavioral patterns?

*Addresses exploratory questions 3 & 4*

### Phase 3: Pattern Validation
**Goal**: Validate discovered patterns are statistically robust

**Methods**:
- Re-apply change detection to pathway transitions
- Statistical testing of complete analytical framework

**Validation Logic**: Do our discovered behavioral patterns represent genuine, replicable phenomena?

*Addresses exploratory question 5*


[← Back to Research Overview](README.md) | [Next: Hypothesis Generation →](2-hypothesis-generation.md)

---

## Quick Navigation to Detailed Analyses
- [Phase 1: Change Point Detection](phases/phase1-change-points.md)
- [Phase 2: Predictive Modeling](phases/phase2-predictive-modeling.md) 
- [Phase 3: Spatial Behavioral Mapping](phases/phase3-spatial-mapping.md)
- [Phase 4: Focused Exploration Discovery](phases/phase4-focused-exploration.md)
