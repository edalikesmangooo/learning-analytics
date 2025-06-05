# Phase 1: Exploratory Analysis  
## From Initial Signals to Deep Structure: A Multi-Stage Exploratory Framework

Understanding how learners engage with collaborative, multiplayer game environments requires more than hypothesis testing—it demands open-ended discovery. This phase employed a four-stage exploratory process, beginning with behavioral signal validation and progressing toward spatial-temporal integration. Each stage built toward a richer understanding of player strategies, transitions, and learning patterns.

---

## Research Context & Motivation

This study examines collaborative gameplay in an informal learning environment (a museum-based computer science game exhibit). While collaborative interactions are central, individual behavior still plays a critical role in shaping how learners engage with content, make decisions, and influence group progress. Capturing and understanding these patterns at scale offers both theoretical and design value.

---

## Progressive Methodology

This phase used a progressive four-stage process:

1. **Detecting Behavioral Transitions** (change points)
2. **Validating Predictive Power** (behavioral feature modeling)
3. **Mapping Latent Behaviors** (spatial analysis)
4. **Integrating Temporal Patterns** (with spatial landscapes)

---

## Stage 1: Detecting Behavioral Transitions — Initial Change Points

### Research Question
Do meaningful behavioral shifts occur within collaborative learning sessions—and can we detect them?

### Approach & Data
- **Approach**: Aggregated event-key analysis using z-scores within fixed-length time windows  
- **Data**: 90 sessions of multiplayer gameplay (~1.5M interaction logs)  
- **Analysis**: Identified temporal windows with significant deviation from baseline behavior

### Key Findings
- **Mid-session variability**: Players often shift strategies after initial exploration
- **Recurrent inflection points**: Change points frequently aligned with moments of task re-engagement
- **Evidence**: 73% of sessions showed ≥1 statistically significant shift in engagement metrics

### Research Implications
The existence of temporal behavioral transitions provided a rationale for deeper modeling and spatial mapping of play styles.

---

## Stage 2: Validating Predictive Power — Behavioral Feature Modeling

### Research Question
Are the extracted behavioral features reliable indicators of success or engagement?

### Approach & Analysis
- **Modeling Technique**: Logistic regression and multinomial classifiers  
- **Features**: Time-binned action ratios, session duration, and goal-oriented behavior metrics  
- **Validation**: 5-fold cross-validation with stratified sampling

### Key Findings
- **Predictive Accuracy**: AUC 0.94 for predicting goal completion  
- **Important Features**: Navigation intensity, early planting behavior, and creature usage patterns  
- **Secondary Insight**: High variability in early-session indicators among lower-performing players

### Research Implications
These results validated the reliability of the derived features, justifying their use in downstream spatial mapping.

---

## Stage 3: Mapping Latent Behaviors — Spatial Playtracing

### Research Question
Can spatial representation of behavior uncover distinct learner strategies or modes of interaction?

### Approach & Analysis
- **Dimensionality Reduction**: t-SNE on standardized behavior feature vectors  
- **Spatial Encoding**: Grid-based discretization to visualize behavior "territories"  
- **Innovation**: Use of a unified coordinate space across sessions to compare player paths

### Key Findings
- **Behavioral Clusters**: Six stable clusters identified with distinct gameplay strategies  
- **Outcome Patterns**: High-performing sessions clustered around a narrow behavioral corridor  
- **Exploration Variability**: Some players explored broadly with limited task engagement

### Research Implications
The spatial landscape provided a novel lens for analyzing emergent strategies and guided targeted investigation into behavioral transitions.

---

## Stage 4: Integrating Temporal Patterns — Advanced Change Point Overlay

### Research Question
How do behavioral shifts align with spatial exploration patterns and learning progress?

### Approach & Analysis
- **Overlay Method**: Applied change point detection to players' trajectories in spatial space  
- **Integration Logic**: Linked time windows to corresponding spatial clusters  
- **Measured Effects**: Compared location shifts, engagement types, and task proximity across change windows

### Key Findings
- **Counter-Intuitive Insight**: Players with “focused” spatial movement had more meaningful change points than broad explorers  
- **Temporal-Spatial Coupling**: Strategic pivots often coincided with re-entry into task-focused zones  
- **Group-Level Divergence**: Lower-performing groups showed erratic or late-phase spatial movement

### Research Implications
These results challenged the assumption that broad exploration inherently benefits learning, highlighting the need for focused behavioral support.

---

## From Exploration to Focused Research Questions

This exploratory trajectory surfaced several core hypotheses about learning through gameplay.

### Generated Hypotheses

- **RQ1**: Do mid-session behavioral shifts predict successful task completion?  
- **RQ2**: Are there distinct player strategy profiles that correlate with learning outcomes?  
- **RQ3**: How does early navigation behavior influence long-term engagement?  
- **RQ4**: Can spatial movement patterns distinguish productive versus unproductive collaboration?

### Theoretical Framework

Findings align with progressive engagement models such as *explore → tinker → refine*, constructionist learning, and productive failure. The analysis highlights how shifting between modes of play—structured, exploratory, and goal-directed—supports or hinders learning depending on timing and context.

---

[← Back to Overview](README.md) | [Next: Hypothesis Generation →](2-hypothesis-generation.md)









### Coming Soon:
- EA1: Change Point Analysis - Detecting critical behavioral transitions
- EA2: Player Modeling - Understanding behavioral archetypes  
- EA3: Spatial Pathways (t-SNE + Grid) - Mapping behavioral landscapes
- From Exploration to Hypotheses

---
[← Back to Overview](README.md) | [Next: Hypothesis Generation →](2-hypothesis-generation.md)
