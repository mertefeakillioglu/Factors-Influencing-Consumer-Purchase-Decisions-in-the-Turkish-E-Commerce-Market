
🏆 Best Performing Configurations and Results

During the experimentation phase, multiple model configurations, hyperparameter settings, and class structure variations were tested using Optuna and cross-validation.

For the purpose of clarity, interpretability, and alignment with behavioural discussion, the dissertation reports models that provided the most stable and behaviourally meaningful explanations, rather than the configurations that achieved the absolute highest numerical performance metrics.

The best-performing configurations in terms of raw predictive metrics (accuracy, F1-score, ROC-AUC, balanced accuracy, etc.) are provided in this repository through additional result files and visual outputs.

These results are included here to ensure:

Transparency of the full experimentation process

Evidence that model selection was not based solely on performance scores

Demonstration of the trade-off between predictive performance and interpretability

Availability of the highest-performing experimental outputs for reference

This reflects the methodological decision described in Chapter 3, where model selection prioritised explainability consistency and behavioural interpretability over marginal improvements in accuracy.

By including these best-performing outputs, this repository presents both:

The models reported in the dissertation for their interpretability value

The highest-performing experimental configurations for full methodological transparency

🧪 Additional Analytical Outputs Beyond Thesis Figures

During the modelling and explainability stages, a large number of SHAP, LIME, and evaluation visuals were generated to test alternative class structures, model behaviours, and interpretability stability.

For clarity and reporting focus, not all of these visuals were included as figures in the dissertation. However, they are intentionally provided in this repository to ensure:

Full transparency of the modelling workflow

Evidence of extensive experimentation and validation

Demonstration of robustness checks performed before selecting the final reported models

Clear traceability between code execution and analytical reasoning

These outputs should be understood as supporting analytical evidence, documenting the depth of the experimentation phase and illustrating how the final models and figures in Chapter 4 were selected after evaluating multiple explainability scenarios.

This is consistent with the methodological statement in Chapter 3, where alternative configurations and interpretability outputs are acknowledged as part of the model selection process.

By including these additional visuals, this repository serves not only as a replication environment for the dissertation but also as a transparent record of the complete analytical exploration.

🔍 LIME Analysis Files — outputs/lime/

These files contain local, case-level explanations that show how the model arrives at a prediction for a single respondent.
They are referenced in Section 4.3 – Local Explanation and Error Analysis.

File	Explanation
lime_high_binary.png	Shows how positive perception signals combine to produce a high-intention prediction in binary modelling.
lime_low_binary.png	Shows how weak or negative perception signals produce a low-intention prediction.
lime_misclassified_binary.png	Used for error analysis to demonstrate how mixed perception signals can lead to incorrect classification.
lime_all_classes_3class.png	Overview of explanation patterns across Low–Mid–High intention levels.
lime_class_0_3class.png	Detailed explanation for a Low intention respondent in 3-class modelling.
lime_class_1_3class.png	Explanation for a Mid intention respondent showing mixed perception drivers.
lime_class_2_3class.png	Explanation for a High intention respondent in 3-class modelling.
lime_all_classes_multiclass.png	Overview of explanations across Very Low–Low–Medium–High intention levels.
lime_class_0_multiclass.png	Explanation for a Very Low intention respondent.
lime_class_1_multiclass.png	Explanation for a Low intention respondent.
lime_class_2_multiclass.png	Explanation for a Medium intention respondent.
lime_class_3_multiclass.png	Explanation for a High intention respondent.
🌐 SHAP Analysis Files — outputs/shap/

These files contain global and class-level explainability visuals referenced in Section 4.2 – SHAP Analysis.

File	Explanation
shap_importance_binary.png	Global feature importance for binary classification.
shap_importance_multiclass.png	Feature importance across four intention levels.
shap_importance_3class.png	Feature importance validation under merged class structure.
shap_summary_binary.png	Distribution of feature effects pushing predictions high or low.
shap_summary_multiclass.png	Distribution of feature effects across four classes.
shap_summary_3class.png	Distribution of feature effects in simplified class structure.
shap_dependence_binary.png	Nonlinear relationships between key predictors and intention (binary).
shap_dependence_multiclass.png	Interaction differences across intention levels.
shap_dependence_3class.png	Stability of nonlinear behaviour in 3-class modelling.
shap_per_class_multiclass.png	Feature dominance for each intention level.
shap_per_class_3class.png	Per-class feature dominance for Low–Mid–High grouping.
shap_waterfall_binary.png	Individual case explanation in binary model.
shap_waterfall_multiclass.png	Individual case explanation in multiclass model.
shap_waterfall_3class.png	Individual case explanation in 3-class model.
📈 Model Performance & Matrix Files — outputs/results/

These files provide the numerical evidence of model performance referenced in Section 4.1 – Model Performance.

File	Explanation
binary_results.csv	Performance metrics for binary models (accuracy, F1, ROC-AUC, etc.).
multiclass_results.csv	Performance metrics for four-class models.
multiclass_3class_results.csv	Performance metrics for three-class validation models.
confusion_matrices_3class.png	Confusion matrix visualisation for 3-class classification.

Together, these files ensure complete transparency between model evaluation, explainability outputs, and the discussion presented in the dissertation.
