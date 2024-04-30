---
title: "Content suppresses style: dimensionality collapse in contrastive learning"
collection: publications
permalink: /publication/2022-Content
date: 2022-12-12
venue: 'NeurIPS 2022 Workshop: Self-Supervised Learning-Theory and Practice'
---
Contrastive learning is a highly successful yet simple self-supervised learning technique that minimizes the representational distance of similar (positive) while maximizing it for dissimilar (negative) samples. Despite its success, our theoretical understanding of contrastive learning is still incomplete. Most importantly, it is unclear why the inferred representation faces a dimensionality collapse after SimCLR training and why downstream performance improves by removing the feature encoder's last layers (projector). We show that collapse might be induced by an inductive bias of the InfoNCE loss for features that vary little within a positive pair (content) while suppressing more strongly-varying features (style). When at least one content variable is present, we prove that a low-rank projector reduces downstream task performance while simultaneously minimizing the InfoNCE objective. This result elucidates a potential reason why removing the projector could lead to better downstream performance. Subsequently, we propose a simple strategy leveraging adaptive temperature factors in the loss to equalize content and style latents, mitigating dimensionality collapse. Finally, we validate our theoretical findings on controlled synthetic data and natural images.