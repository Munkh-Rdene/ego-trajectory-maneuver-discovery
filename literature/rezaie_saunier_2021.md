# Rezaie & Saunier (2021)
**Trajectory Clustering Performance Evaluation: If We Know the Answer, It’s Not Clustering**

## Citation
Rezaie, M., & Saunier, N. (2021). *Trajectory Clustering Performance Evaluation: If We Know the Answer, It’s Not Clustering*. arXiv:2112.01570.

## Core Idea
Trajectory clustering is inherently an **unsupervised** task. If labels are predefined or required for
evaluation, the problem shifts toward classification rather than discovery.

The authors emphasize that clustering outcomes depend jointly on:
- trajectory representation
- similarity / distance measure
- clustering algorithm
- evaluation metric

They refer to this combination as a **clustering setup**.

## Motivation
Most trajectory datasets do not have natural labels. Manual annotation is:
- costly
- subjective
- application-dependent

Therefore, both clustering **and evaluation** should ideally remain unsupervised.

## Key Contributions
- Comprehensive comparison of trajectory similarity measures
- Evaluation of multiple clustering algorithms
- Use of unsupervised evaluation metrics
- Proposal of OD-based reference clusters without manual labeling
- Demonstration that no single clustering setup dominates across datasets

## Key Insight
There is **no universally optimal** distance or clustering algorithm.
Good clustering depends on:
- data characteristics
- representation choices
- analysis goals

This supports exploratory, interpretation-driven analysis rather than metric optimization.

## Relevance to This Project
This paper provides methodological justification for:
- avoiding predefined maneuver labels
- focusing on interpretable trajectory representations
- treating clustering as exploratory pattern discovery
- prioritizing understanding over benchmark performance

The emphasis on representation choice aligns with this project’s focus on
normalized ego trajectories and simple geometric/kinematic features.

## Takeaway
Clustering should be used to **reveal structure**, not confirm assumptions.
Interpretability and context matter more than absolute clustering scores.
