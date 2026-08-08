# RPS-ARC-AGI-3

RPS ARC-AGI 3 Solutions Technical Report

[PDF](https://iamjasonfeng.github.io/RPS-ARC-AGI-3/rps_arc_agi_3_solutions_technical_report.pdf)

Abstract

This paper documents three of my ARC-AGI-3 solutions: Gorilla-1.1, Sandwich, and Tiger. The solutions are based on
Regressive Plasticity Schedule (RPS), a post-training method I created. Gorilla-1.1 applies RPS during post-training
through a three-stage multimodal DPO curriculum with lower learning rates in later stages. Sandwich applies RPS at
test time through an Explore-to-Stable proposal tournament. Tiger applies RPS at test time to within-level working
memory, cross-level memory, and occasional surprise proposals. I built all three solutions on the Tufa Labs Duck
harness and used Qwen3.6-27B as their underlying model. I present this as a technical methods report: I document the
approaches and released artifacts, but I do not claim that any method is superior to Tufa, to another existing system,
or to either of the other methods described here. ARC-AGI-3 agent trajectories are stochastic, and as of this writing I
have not been able to perform enough independent competition runs under the one-submission-per-day limit to
support a reliable quantitative comparison. Evaluation is ongoing, and readers can visit the linked Kaggle notebooks,
where Kaggle automatically displays each notebook's best competition score.
