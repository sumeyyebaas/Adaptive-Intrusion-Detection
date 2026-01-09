# Adaptive Intrusion Detection System (IDS)

This repository contains the implementation and experimental setup for the research paper: 
**"Adaptive Intrusion Detection for Evolving RPL IoT Attacks Using Incremental Learning"**.

## Abstract
The Routing Protocol for Low-power and Lossy Networks (RPL) is standard for IoT but vulnerable to routing-layer attacks. Traditional ML classifiers fail against zero-day attacks unless fully retrained. This study investigates **Incremental Learning** as an adaptive strategy to maintain resilient detection while mitigating **catastrophic forgetting** and reducing training time.

## Repository Structure
* **`datasets/`**: RPL-specific attack datasets.
    * `DecreasedRankAttack.csv`: Rank-based routing manipulation data.
    * `HelloFloodAttack.csv`: Resource exhaustion and neighbor table flooding data.
    * `VersionNumberAttack.csv`: Global repair triggering and overhead attacks.
* **`codes/`**: 
    * `incremental_learning.ipynb`: Evaluation of model adaptation to novel RPL attacks.
    * `individual_model_training.ipynb`: Baseline performance analysis.

## Research Scope
* **Target Protocol**: RPL (IPv6 Routing Protocol for Low-Power and Lossy Networks).
* **Model Families**: Ensemble models (**XGBoost, LightGBM, CatBoost**) and **Deep Learning**.
* **Key Investigations**: 
    * Detection performance on new attack classes.
    * Mitigation of catastrophic forgetting.
    * Training time efficiency.

## Citation
 @misc{bas2025adaptiveintrusiondetectionevolving,
      title={Adaptive Intrusion Detection for Evolving RPL IoT Attacks Using Incremental Learning}, 
      author={Sumeyye Bas and Kiymet Kaya and Elif Ak and Sule Gunduz Oguducu},
      year={2025},
      eprint={2511.11464},
      archivePrefix={arXiv},
      primaryClass={cs.CR},
      url={https://arxiv.org/abs/2511.11464}, 
}
