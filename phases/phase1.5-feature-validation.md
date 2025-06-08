# Predictive Modeling

## Motivation
Change point analysis revealed correlational patterns between behavioral transitions and learning success. To understand the multidimensional nature of player behavior and predict learning outcomes, we move beyond event-level anomaly detection toward comprehensive player state modeling. The findings from change point analysis revealed two important dimensions that could inform predictive modeling: temporal patterns (when behavioral shifts occur during gameplay progression) and behavioral patterns (which types of player actions emerge as significant transitions). However, observational correlation does not guarantee predictive validity.

**Question:** Do these temporal and behavioral factors really have predictive power that can guide effective player state discovery?

## Methodology

### Feature extraction from change point insights:
*(add diagram if time)*
- **Temporal aspects:** time bin distribution, session duration
- **Behavioral aspects:** event types and frequencies (player actions)

### Supervised learning validation:
- **Data:** 1,296 sessions with extracted temporal + behavioral features
- **Methods:** Logistic regression, MultinomialNB (LR showed superior AUC)
- **Target:** Learning outcome prediction (AllOrbsFilled success/unsuccessful)

## Key Findings
*(images for each)*

### Strong Predictive Performance:
- **AUC:** 0.952 - Excellent discrimination between success/failure
- **87% accuracy** with balanced precision (80-93%) and recall (82-93%)

### Feature Importance Rankings:
- **Planting activities** emerge as strongest success predictors across all gameplay phases (coefficients 3.17-4.87)
- **Navigation** shows phase-dependent effects: positive early game, negative late game
- **Programming activities** show negative associations, potentially indicating struggle patterns

### Interaction Effects:
The same behavioral actions show different predictive power depending on timing—planting late in sessions is more predictive than planting early, confirming that behavioral context matters for learning outcomes.

## Next Steps

### Transition to Player State Discovery:
With validated predictive power established, these behavioral-temporal features provide a robust foundation for t-SNE analysis to discover distinct player states and learning trajectories during collaborative gameplay.

### Future Methodological Refinements:
Disentangle phase effects from behavioral effects through separate feature engineering (behavioral totals vs. temporal patterns vs. interaction terms) to understand whether timing or action type drives predictive power.
