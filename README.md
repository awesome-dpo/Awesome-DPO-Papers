<h1 align="center">
📝 Awesome Direct Prefereence Optimization
</h1>
<div align="center">

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) 
![Updated](https://img.shields.io/badge/Updated-July_2024-blue)
![Stars](https://img.shields.io/github/stars/awesome-dpo/Awesome-DPO-Papers?color=yellow&labelColor=555555) 
</div>

## 📚 Overview

A collection of resources about direct perference optimization (DPO) series, including papers, models, repos, applications. 


<p align="center">
  <img src="dpo.jpg" width="640">
</p>



## 💡Table of Content
- 🧠[Algorithms](#algorithms)
  - [Data Source](#data-source)
    <!-- - [Offline](#offline) -->
    - [Data Processing](#data-processing)
    - [Self-Rewarding](#self-rewarding)
    - [Data Generation](#data-generation)
  - [Feedback Granularity](#feedback-granularity)
    - [Token Level](#token-level)
    - [Reasoning Step Level](#reasoning-step-level)
    - [Sequence Level](#sequence-level)
  - [Regularization](#regularization)
    - [Response Length](#response-length)
    - [Likelihood](#likelihood)
    - [Noise Label](#noise-label)
  - [Feedback Signal](#feedback-signal)
    - [Point-wised Feedback](#point-wised-feedback)
    <!-- - [Pair-wised Feedback](#pair-wised-feedback) -->
    - [List-wised Feedback](#list-wised-feedback)
  - [Reference Model](#reference-model)
    <!-- - [Reference Model Invariant](#reference-model-invariant) -->
    - [Reference Model Free](#reference-model-free)
    - [Reference Model Variant](#reference-model-variant)
  - [Transformation Function](#transformation-function)

- 🧐[Analysis](#analysis)
  - [Comparison between DPO and PPO](#comparison-between-dpo-and-ppo) 
  - [Hyperparameter Tunning](#hyperparameter-tuning) 
  - [Theoretical Analysis](#theoretical-analysis) 

- 🎯[Application](#application)
  - [Vision & Video](#vision--video)
  - [Audio](#audio)
  - [Multimodal-LLM](#multimodal-llm)
  - [Language](#language)
    - [Conversation](#conversation)
    - [Multilingual-LLM](#multilingual-llm)
    - [Long-LLM](#long-llm)
    - [Technical Reports of LLMs](#technical-reports-of-llms)
  - [Math](#math)
  - [Code](#code)
  - [Science](#science)
    - [Medical Health](#medical-health)
    - [Chemistry](#chemistry)
    - [Biology](#biology)
  - [Recommendation and Search](#recommendation-and-search)
  - [Finance](#finance)
  - [Embodied-AI](#embodied-ai)
  - [Social Impact (Safety, Privacy, Bias)](#social-impact-safety-privacy-bias)
---

## 🧠Algorithms

### Data Source
<!-- #### Offline -->
#### Data Processing
* 2024.02 **"Controllable Preference Optimization: Toward Controllable Multi-Objective Alignment"**. [[Paper]](https://arxiv.org/abs/2402.19085) [[Code]](https://github.com/OpenBMB/CPO)
* 2024.03 **"sDPO: Don't Use Your Data All at Once"**. [[Paper]](https://arxiv.org/abs/2403.19270)
* 2024.08 **"Bridging and Modeling Correlations in Pairwise Data for Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2408.07471) [[Code]](https://github.com/YJiangcm/BMC)
* 2024.06 **"Suri: Multi-constraint Instruction Following for Long-form Text Generation"**. [[Paper]](https://arxiv.org/abs/2406.19371) [[Code]](https://github.com/chtmp223/suri)
* 2024.08 **"Less for More: Enhancing Preference Learning in Generative Language Models with Automated Self-Curation"**. [[Paper]](https://arxiv.org/abs/2408.12799) [[Code]](https://github.com/Self-Curation/Project)
* 2024.06 **"OPTune: Efficient Online Preference Tuning"**. [[Paper]](https://arxiv.org/abs/2406.07657)
---
#### Self-Rewarding
* 2024.01 **"Self-Rewarding Language Models"**. [[Paper]](https://arxiv.org/abs/2401.10020) [[Code]](https://github.com/Oxen-AI/Self-Rewarding-Language-Models)
* 2024.02 **"OAIF: Direct Language Model Alignment from Online AI Feedback"**. [[Paper]](https://arxiv.org/abs/2402.04792) [[Code]](https://hyunyoung2.github.io/2024/09/02/OAIF/)
* 2024.04 **"Iterative Reasoning Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2404.19733)
* 2024.06 **"Bootstrapping Language Models with DPO Implicit Rewards"**. [[Paper]](https://arxiv.org/abs/2406.09760) [[Code]](https://github.com/sail-sg/dice)
* 2024.06 **"Is Free Self-Alignment Possible?"**. [[Paper]](https://arxiv.org/abs/2406.03642)
---

#### Data Generation
* 2024.06 **"Online DPO: Online Direct Preference Optimization with Fast-Slow Chasing"**. [[Paper]](https://arxiv.org/abs/2406.05534)
* 2024.06 **"Iterative Length-Regularized Direct Preference Optimization: A Case Study on Improving 7B Language Models to GPT-4 Level"**. [[Paper]](https://arxiv.org/abs/2406.11817)
* 2024.04 **"Preference Fine-Tuning of LLMs Should Leverage Suboptimal, On-Policy Data"**. [[Paper]](https://arxiv.org/abs/2404.14367) [[Code]](https://understanding-rlhf.github.io/)
* 2024.06 **"Show, Don't Tell: Aligning Language Models with Demonstrated Feedback"**. [[Paper]](https://arxiv.org/abs/2406.00888) [[Code]](https://github.com/SALT-NLP/demonstrated-feedback)
* 2024.06 **"BPO: Staying Close to the Behavior LLM Creates Better Online LLM Alignment"**. [[Paper]](https://arxiv.org/abs/2406.12168) [[Code]](https://github.com/xu1998hz/BPO)
* 2024.07 **"Iterative Nash Policy Optimization: Aligning LLMs with General Preferences via No-Regret Learning"**. [[Paper]](https://arxiv.org/abs/2407.00617)
* 2024.02 **"RS-DPO: A Hybrid Rejection Sampling and Direct Preference Optimization Method for Alignment of Large Language Models"**. [[Paper]](https://arxiv.org/abs/2402.10038)
* 2024.05 **"D2PO: Discriminator-Guided DPO with Response Evaluation Models"**. [[Paper]](https://arxiv.org/abs/2405.01511) [[Code]](https://github.com/PrasannS/d2po)
* 2024.09 **"TSO: Self-Training with Scaled Preference Optimization"**. [[Paper]](https://www.arxiv.org/abs/2409.02118)
---
### Feedback Granularity
#### Token Level
* 2024.08 **"Bridging and Modeling Correlations in Pairwise Data for Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2408.07471) [[Code]](https://github.com/YJiangcm/BMC)
* 2024.06 **"Eliminating Biased Length Reliance of Direct Preference Optimization via Down-Sampled KL Divergence"**. [[Paper]](https://arxiv.org/abs/2406.10957) [[Code]](https://github.com/LuJunru/SamPO)
* 2024.04 **"Token-level Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2404.11999) [[Code]](https://github.com/Vance0124/Token-level-Direct-Preference-Optimization)
* 2024.08 **"Selective Preference Optimization via Token-Level Reward Function Estimation"**. [[Paper]](https://arxiv.org/abs/2408.13518)
* 2024.08 **"Inverse-Q *: Token Level Reinforcement Learning for Aligning Large Language Models Without Preference Data"**. [[Paper]](https://arxiv.org/abs/2408.14874)
---
#### Reasoning Step Level
* 2024.07 **"Step-Controlled DPO: Leveraging Stepwise Error for Enhanced Mathematical Reasoning"**. [[Paper]](https://arxiv.org/abs/2407.00782) [[Code]](https://github.com/mathllm/Step-Controlled_DPO)
* 2024.06 **"Step-DPO: Step-wise Preference Optimization for Long-chain Reasoning of LLMs"**. [[Paper]](https://arxiv.org/abs/2406.18629) [[Code]](https://github.com/dvlab-research/Step-DPO)
---
#### Sequence Level
* 2024.07 **"β-DPO: Direct Preference Optimization with Dynamic β"**. [[Paper]](https://arxiv.org/abs/2407.08639) [[Code]](https://github.com/junkangwu/beta-DPO)
* 2024.07 **"Right Now, Wrong Then: Non-Stationary Direct Preference Optimization under Preference Drift"**. [[Paper]](https://arxiv.org/abs/2407.18676)
* 2024.08 **"Offline RLHF Methods Need More Accurate Supervision Signals"**. [[Paper]](https://arxiv.org/abs/2408.09385)
* 2024.06 **"WPO: Enhancing RLHF with Weighted Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2406.11827) [[Code]](https://github.com/wzhouad/WPO)
* 2024.06 **"Adaptive Query Rewriting: Aligning Rewriters through Marginal Probability of Conversational Answers"**. [[Paper]](https://arxiv.org/abs/2406.10991)
---
### Regularization
#### Response Length
* 2024.02 **"Refined Direct Preference Optimization with Synthetic Data for Behavioral Alignment of LLMs"**. [[Paper]](https://arxiv.org/abs/2402.08005) [[Code]](https://github.com/vicgalle/refined-dpo/)
* 2024.05 **"SimPO: Simple Preference Optimization with a Reference-Free Reward"**. [[Paper]](https://arxiv.org/abs/2405.14734) [[Code]](https://github.com/princeton-nlp/SimPO)
* 2024.07 **"The Hitchhiker's Guide to Human Alignment with *PO"**. [[Paper]](https://arxiv.org/abs/2407.15229)
* 2024.06 **"Iterative Length-Regularized Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2406.11817)
* 2024.09 **"Length Desensitization in Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2409.06411)
---
#### Likelihood
<!-- * 2024.07 **"Step-Controlled DPO: Leveraging Stepwise Error for Enhanced Mathematical Reasoning"**. [[Paper]](https://arxiv.org/abs/2407.00782) [[Code]]() -->
* 2024.02 **"Controllable Preference Optimization: Toward Controllable Multi-Objective Alignment"**. [[Paper]](https://arxiv.org/abs/2402.19085) [[Code]](https://github.com/OpenBMB/CPO)
* 2024.04 **"Token-level Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2404.11999) [[Code]](https://github.com/Vance0124/Token-level-Direct-Preference-Optimization)
* 2024.06 **"Step-level Value Preference Optimization for Mathematical Reasoning"**. [[Paper]](https://arxiv.org/abs/2406.10858) [[Code]](https://github.com/MARIO-Math-Reasoning/Super_MARIO)
* 2024.03 **"ORPO: Monolithic Preference Optimization without Reference Model"**. [[Paper]](https://arxiv.org/abs/2403.07691) [[Code]](https://github.com/xfactlab/orpo)
* 2024.05 **"Value-Incentivized Preference Optimization: A Unified Approach to Online and Offline RLHF"**. [[Paper]](https://arxiv.org/abs/2405.19320)
* 2024.05 **"Direct Alignment of Language Models via Quality-Aware Self-Refinement"**. [[Paper]](https://arxiv.org/abs/2405.21040)
---
#### Noise Label
* 2024.07 **"Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.07880) [[Code]](https://github.com/junkangwu/Dr_DPO)
* 2024.04 **"ROPO: Robust Preference Optimization for Large Language Models"**. [[Paper]](https://arxiv.org/abs/2404.04102)
* 2024.05 **"Would I Lie To You? Inference Time Alignment of Language Models using Direct Preference Heads"**. [[Paper]](https://arxiv.org/abs/2405.20053)
* 2024.06 **"Robust Reinforcement Learning from Corrupted Human Feedback"**. [[Paper]](https://arxiv.org/abs/2406.15568)
---
### Feedback Signal
#### Point-wised Feedback
* 2024.02 **"KTO: Model Alignment as Prospect Theoretic Optimization"**. [[Paper]](https://arxiv.org/abs/2402.01306) [[Code]](https://github.com/ContextualAI/HALOs)
* 2024.08 **"Reward Difference Optimization (RDO): Offline RLHF Methods Need More Accurate Supervision Signals"**. [[Paper]](https://arxiv.org/abs/2408.09385)
* 2024.05 **"Offline Regularised Reinforcement Learning for Large Language Models Alignment"**. [[Paper]](https://arxiv.org/abs/2405.19107)
---
<!-- #### Pair-wised Feedback -->
#### List-wised Feedback
* 2024.02 **"LiPO: Listwise Preference Optimization through Learning-to-Rank"**. [[Paper]](https://arxiv.org/abs/2402.01878)
---
### Reference Model
<!-- #### Reference Model Invariant -->
#### Reference Model Free
* 2024.05 **"SimPO: Simple Preference Optimization with a Reference-Free Reward"**. [[Paper]](https://arxiv.org/abs/2405.14734) [[Code]](https://github.com/princeton-nlp/SimPO)
* 2024.05 **"Soft Preference Optimization: Aligning Language Models to Expert Distributions"**. [[Paper]](https://arxiv.org/abs/2405.00747v4)
* 2024.03 **"ORPO: Monolithic Preference Optimization without Reference Model"**. [[Paper]](https://arxiv.org/abs/2403.07691) [[Code]](https://github.com/xfactlab/orpo)
* 2024.01 **"Contrastive Preference Optimization: Pushing the Boundaries of LLM Performance in Machine Translation"**. [[Paper]](https://arxiv.org/abs/2401.08417) [[Code]](https://github.com/fe1ixxu/ALMA)
---
#### Reference Model Variant
* 2024.03 **"sDPO: Don't Use Your Data All at Once"**. [[Paper]](https://arxiv.org/abs/2403.19270)
* 2024.04 **"Direct Nash Optimization: Teaching Language Models to Self-Improve with General Preferences"**. [[Paper]](https://arxiv.org/abs/2404.03715)
* 2024.04 **"Iterative Reasoning Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2404.19733)
---
### Transformation Function
* 2024.02 **"Generalized Preference Optimization: A Unified Approach to Offline Alignment"**. [[Paper]](https://arxiv.org/abs/2402.05749)
* 2023.09 **"Beyond Reverse KL: Generalizing Direct Preference Optimization with Diverse Divergence Constraints"**. [[Paper]](https://arxiv.org/abs/2309.16240)
* 2023.10 **"A General Theoretical Paradigm to Understand Learning from Human Preferences"**. [[Paper]](https://arxiv.org/abs/2310.12036)
* 2024.05 **"Offline Regularised Reinforcement Learning for Large Language Models Alignment"**. [[Paper]](https://arxiv.org/abs/2405.19107)
* 2024.07 **"Correcting the Mythos of KL-Regularization: Direct Alignment without Overoptimization via Chi-Squared Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.13399)
* 2024.07 **"Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.07880) [[Code]](https://github.com/junkangwu/Dr_DPO)
* 2024.07 **"New Desiderata for Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.09072)
---

## 🧐Analysis
### Comparison between DPO and PPO
* 2024.06 **"Unpacking DPO and PPO: Disentangling Best Practices for Learning from Preference Feedback"**. [[Paper]](https://arxiv.org/abs/2406.09279)[[Code]](https://github.com/hamishivi/EasyLM)
* 2024.04 **"Is DPO Superior to PPO for LLM Alignment? A Comprehensive Study"**. [[Paper]](https://arxiv.org/abs/2404.10719)[[Code]](https://github.com/openpsi-project/ReaLHF)
* 2023.12 **"Policy Optimization in RLHF: The Impact of Out-of-preference Data"**. [[Paper]](https://arxiv.org/abs/2312.10584)[[Code]](https://github.com/liziniu/policy_optimization)
* 2024.06 **"3D-Properties: Identifying Challenges in DPO and Charting a Path Forward"**. [[Paper]](https://arxiv.org/abs/2406.07327)
* 2024.05 **"Understanding the performance gap between online and offline alignment algorithms"**. [[Paper]](https://arxiv.org/abs/2405.08448)
* 2024.04 **"DPO Meets PPO: Reinforced Token Optimization for RLHF"**. [[Paper]](https://arxiv.org/abs/2404.18922)[[Code]](https://github.com/zkshan2002/RTO)
* 2024.09 **"On the Limited Generalization Capability of the Implicit Reward Model Induced by Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2409.03650)
---
### Hyperparameter Tuning
* 2024.08 **"Minor DPO reject penalty to increase training robustness"**. [[Paper]](https://arxiv.org/abs/2408.09834)
* 2024.07 **"Understanding Reference Policies in Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.13709)[[Code]](https://github.com/yale-nlp/refdpo)
* 2024.02 **"Generalized Preference Optimization: A Unified Approach to Offline Alignment"**. [[Paper]](https://arxiv.org/abs/2402.05749)
* 2024.06 **"Scaling Laws for Reward Model Overoptimization in Direct Alignment Algorithms"**. [[Paper]](https://arxiv.org/abs/2406.02900)
* 2024.06 **"Discovering Preference Optimization Algorithms with and for Large Language Models"**. [[Paper]](https://arxiv.org/abs/2406.08414)[[Code]](https://github.com/SakanaAI/DiscoPOP)
---
### Theoretical Analysis
* 2024.08 **"On the Generalization of Preference Learning with DPO"**. [[Paper]](https://arxiv.org/abs/2408.03459)
* 2024.07 **"Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.07880)[[Code]](https://github.com/junkangwu/Dr_DPO)
* 2024.03 **"Provably Robust DPO: Aligning Language Models with Noisy Feedback"**. [[Paper]](https://arxiv.org/abs/2403.00409)
* 2024.07 **"New Desiderata for Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.09072)
* 2024.06 **"Distributional Preference Alignment of LLMs via Optimal Transport"**. [[Paper]](https://arxiv.org/abs/2406.05882)
* 2025.02 **"Reveal the Mystery of DPO: The Connection between DPO and RL Algorithms"**. [[Paper]](https://arxiv.org/abs/2502.03095)

---

## 🎯Application
### Vision & Video
* 2024.06 **"PopAlign: Population-Level Alignment for Fair Text-to-Image Generation"**. [[Paper]](https://arxiv.org/abs/2406.19668)
* 2024.06 **"Aligning Diffusion Models with Noise-Conditioned Perception"**. [[Paper]](https://arxiv.org/abs/2406.17636)
* 2024.06 **"Margin-aware Preference Optimization for Aligning Diffusion Models without Reference"**. [[Paper]](https://arxiv.org/abs/2406.06424) [[Code]](https://mapo-t2i.github.io)
* 2024.06 **"Diffusion-RPO: Aligning Diffusion Models through Relative Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2406.06382) [[Code]](https://github.com/yigu1008/Diffusion-RPO)
* 2024.06 **"Step-aware Preference Optimization: Aligning Preference with Denoising Performance at Each Step"**. [[Paper]](https://arxiv.org/abs/2406.04314) [[Code]](https://github.com/RockeyCoss/SPO)
* 2024 **"Diffusion Model Alignment Using Direct Preference Optimization"**. [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/html/Wallace_Diffusion_Model_Alignment_Using_Direct_Preference_Optimization_CVPR_2024_paper.html)
* 2024 **"Using Human Feedback to Fine-tune Diffusion Models without Any Reward Model"**. [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/html/Yang_Using_Human_Feedback_to_Fine-tune_Diffusion_Models_without_Any_Reward_CVPR_2024_paper.html) [[Code]](https://github.com/yk7333/D3PO)
* 2024.04 **"Aligning Diffusion Models by Optimizing Human Utility"**. [[Paper]](https://arxiv.org/abs/2404.04465) [[Code]](https://github.com/jacklishufan/diffusion-kto)
* 2024.02 **"A Dense Reward View on Aligning Text-to-Image Diffusion with Preference"**. [[Paper]](https://arxiv.org/abs/2402.08265) [[Code]](https://github.com/Shentao-YANG/Dense_Reward_T2I)
* 2024.05 **"MoDiPO: text-to-motion alignment via AI-feedback-driven Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2405.03803)
* 2024.05 **"Curriculum Direct Preference Optimization for Diffusion and Consistency Models"**. [[Paper]](https://arxiv.org/abs/2405.13637) [[Code]](https://github.com/CroitoruAlin/Curriculum-DPO)
* 2024.03 **"AGFSync: Leveraging AI-Generated Feedback for Preference Optimization in Text-to-Image Generation"**. [[Paper]](https://arxiv.org/abs/2403.13352) [[Code]](https://anjingkun.github.io/AGFSync)
* 2024.05 **"Boost Your Own Human Image Generation Model via Direct Preference Optimization with AI Feedback"**. [[Paper]](https://arxiv.org/abs/2405.20216)
* 2024.03 **"Fast High-Resolution Image Synthesis with Latent Adversarial Diffusion Distillation"**. [[Paper]](https://arxiv.org/abs/2403.12015)
* 2024.04 **"Direct Preference Optimization of Video Large Multimodal Models from Language Model Reward"**. [[Paper]](https://arxiv.org/abs/2404.01258) [[Code]](https://github.com/RifleZhang/LLaVA-Hound-DPO)
* 2024.06 **"ISR-DPO: Aligning Large Multimodal Models for Videos by Iterative Self-Retrospective DPO"**. [[Paper]](https://arxiv.org/abs/2406.11280) [[Code]](https://github.com/snumprlab/ISR-DPO)
* 2024.07 **"Aligning Diffusion Behaviors with Q-functions for Efficient Continuous Control"**. [[Paper]](https://arxiv.org/abs/2407.09024) [[Code]](https://github.com/thu-ml/Efficient-Diffusion-Alignment)
* 2024.09 **"Pixel-Space Post-Training of Latent Diffusion Models"**. [[Paper]](https://arxiv.org/abs/2409.17565)
---
### Audio
* 2024.07 **"Qwen2-Audio Technical Report"**. [[Paper]](https://arxiv.org/abs/2407.10759) [[Code]](https://github.com/QwenLM/Qwen2-Audio)
* 2024.03 **"CAT: Enhancing Multimodal Large Language Model to Answer Questions in Dynamic Audio-Visual Scenarios"**. [[Paper]](https://arxiv.org/abs/2403.04640) [[Code]](https://github.com/rikeilong/Bay-CAT)
* 2024.04 **"Tango 2: Aligning Diffusion-based Text-to-Audio Generations through Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2404.09956) [[Code]](https://github.com/declare-lab/tango)
* 2024.04 **"SpeechAlign: Aligning Speech Generation to Human Preferences"**. [[Paper]](https://arxiv.org/abs/2404.05600) [[Code]](https://0nutation.github.io/SpeechAlign.github.io/)
* 2024.07 **"Robust Zero-Shot Text-to-Speech Synthesis with Reverse Inference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.02243) [[Code]](https://yuchen005.github.io/RIO-TTS-demos/)
* 2024.06 **"Enhancing Zero-shot Text-to-Speech Synthesis with Human Feedback"**. [[Paper]](https://arxiv.org/abs/2406.00654)
---
### Multimodal-LLM
* 2024.04 **"Self-Supervised Visual Preference Alignment"**. [[Paper]](https://arxiv.org/abs/2404.10501) [[Code]](https://github.com/Kevinz-code/SeVa)
* 2023.12 **"Silkie: Preference Distillation for Large Visual Language Models"**. [[Paper]](https://arxiv.org/abs/2312.10665) [[Code]](https://vlf-silkie.github.io)
* 2024.02 **"Multi-modal Preference Alignment Remedies Degradation of Visual Instruction Tuning on Language Models"**. [[Paper]](https://arxiv.org/abs/2402.10884) [[Code]](https://github.com/findalexli/mllm-dpo)
* 2023.11 **"Beyond Hallucinations: Enhancing LVLMs through Hallucination-Aware Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2311.16839) [[Code]](https://opendatalab.github.io/HA-DPO/)
* 2024.08 **"CLIP-DPO: Vision-Language Models as a Source of Preference for Fixing Hallucinations in LVLMs"**. [[Paper]](https://arxiv.org/abs/2408.10433)
* 2024.08 **"xGen-MM (BLIP-3): A Family of Open Large Multimodal Models"**. [[Paper]](https://arxiv.org/abs/2408.08872) [[Code]](https://www.salesforceairesearch.com/opensource/xGen-MM/index.html)
* 2024 **"Safe-CLIP: Removing NSFW Concepts from Vision-and-Language Models"**. [[Paper]](https://iris.unimore.it/retrieve/d3462409-6992-4422-b4aa-c6fbc8982cee/2024_ECCV_Safe_CLIP_CameraReady.pdf)
* 2024.02 **"Aligning Modalities in Vision Large Language Models via Preference Fine-tuning"**. [[Paper]](https://arxiv.org/abs/2402.11411) [[Code]](https://github.com/YiyangZhou/POVID)
* 2024.05 **"Calibrated Self-Rewarding Vision Language Models"**. [[Paper]](https://arxiv.org/abs/2405.14622) [[Code]](https://github.com/YiyangZhou/CSR)
* 2024.06 **"i-SRT: Aligning Large Multimodal Models for Videos by Iterative Self-Retrospective Judgment"**. [[Paper]](https://arxiv.org/abs/2406.11280) [[Code]](https:
//github.com/snumprlab/ISR-DPO)
* 2024.05 **"Enhancing Visual-Language Modality Alignment in Large Vision Language Models via Self-Improvement"**. [[Paper]](https://arxiv.org/abs/2405.15973)
* 2024.05 **"Enhancing Large Vision Language Models with Self-Training on Image Comprehension"**. [[Paper]](https://arxiv.org/abs/2405.19716) [[Code]](https://stic-lvlm.github.io)
* 2024.06 **"STLLaVA-Med: Self-Training Large Language and Vision Assistant for Medical Question-Answering"**. [[Paper]](https://arxiv.org/abs/2406.19973) [[Code]](https://github.com/heliossun/STLLaVA-Med)
* 2024.03 **"Strengthening Multimodal Large Language Model with Bootstrapped Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2403.08730)
* 2024 **"CityLLaVA: Efficient Fine-Tuning for VLMs in City Scenario"**. [[Paper]](https://openaccess.thecvf.com/content/CVPR2024W/AICity/html/Duan_CityLLaVA_Efficient_Fine-Tuning_for_VLMs_in_City_Scenario_CVPRW_2024_paper.html) [[Code]](https://github.com/alibaba/AICITY2024_Track2_AliOpenTrek_CityLLaVA)
* 2024.03 **"CAT: Enhancing Multimodal Large Language Model to Answer Questions in Dynamic Audio-Visual Scenarios"**. [[Paper]](https://arxiv.org/abs/2403.04640) [[Code]](https://github.com/rikeilong/Bay-CAT)
* 2024 **"Detecting and Preventing Hallucinations in Large Vision Language Models"**. [[Paper]](https://ojs.aaai.org/index.php/AAAI/article/view/29771) [[Code]](https://github.com/hendryx-scale/mhal-detect)
* 2024 **"Multi-Modal Hallucination Control by Visual Information Grounding"**. [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/html/Favero_Multi-Modal_Hallucination_Control_by_Visual_Information_Grounding_CVPR_2024_paper.html)
* 2024.05 **"NoiseBoost: Alleviating Hallucination with Noise Perturbation for Multimodal Large Language Models"**. [[Paper]](https://arxiv.org/abs/2405.20081) [[Code]](https://kaiwu5.github.io/noiseboost)
* 2024 **"RLHF-V: Towards Trustworthy MLLMs via Behavior Alignment from Fine-grained Correctional Human Feedback"**. [[Paper]](https://openaccess.thecvf.com/content/CVPR2024/html/Yu_RLHF-V_Towards_Trustworthy_MLLMs_via_Behavior_Alignment_from_Fine-grained_Correctional_CVPR_2024_paper.html)
* 2024.05 **"RLAIF-V: Open-Source AI Feedback Leads to Super GPT-4V Trustworthiness"**. [[Paper]](https://arxiv.org/abs/2405.17220) [[Code]](https://github.com/RLHF-V/RLAIF-V)
* 2024.08 **"MiniCPM-V: A GPT-4V Level MLLM on Your Phone"**. [[Paper]](https://arxiv.org/abs/2408.01800) [[Code]](https://github.com/OpenBMB/MiniCPM-o)
* 2024.04 **"Detecting and Mitigating Hallucination in Large Vision Language Models via Fine-Grained AI Feedback"**. [[Paper]](https://arxiv.org/abs/2404.14233) [[Code]](https://github.com/Mr-Loevan/HSA-DPO)
* 2024.08 **"Mitigating Multilingual Hallucination in Large Vision-Language Models"**. [[Paper]](https://arxiv.org/abs/2408.00550) [[Code]](https://github.com/ssmisya/MHR)
* 2024.08 **"LLaVA-MoD: Making LLaVA Tiny via MoE Knowledge Distillation"**. [[Paper]](https://arxiv.org/abs/2408.15881) [[Code]](https://github.com/shufangxun/LLaVA-MoD)
* 2024.08 **"EPO: Hierarchical LLM Agents with Environment Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2408.16090) [[Code]](https://github.com/kevinz8866/EPO)
* 2024.05 **"Automated Multi-level Preference for MLLMs"**. [[Paper]](https://arxiv.org/abs/2405.11165) [[Code]](https://github.com/takomc/amp)
* 2024.05 **"Alleviating Hallucinations in Large Vision-Language Models through Hallucination-Induced Optimization"**. [[Paper]](https://arxiv.org/abs/2405.15356) [[Code]](https://github.com/BT-C/HIO)
* 2024.06 **"mDPO: Conditional Preference Optimization for Multimodal Large Language Models"**. [[Paper]](https://arxiv.org/abs/2406.11839) [[Code]](https://feiwang96.github.io/mDPO)
* 2024.07 **"InternLM-XComposer-2.5: A Versatile Large Vision Language Model Supporting Long-Contextual Input and Output"**. [[Paper]](https://arxiv.org/abs/2407.03320) [[Code]](https://github.com/InternLM/InternLM-XComposer)
---
### Language
#### Conversation
* 2024.07 **"Efficient and Accurate Memorable Conversation Model using DPO based on sLLM"**. [[Paper]](https://arxiv.org/abs/2407.06537)
* 2024.06 **"Learning to Ask Informative Questions: Enhancing LLMs with Preference Optimization and Expected Information Gain"**. [[Paper]](https://arxiv.org/abs/2406.17453) [[Code]](https://github.com/dmazzaccara/LearningToAsk)
* 2024.06 **"Direct Multi-Turn Preference Optimization for Language Agents"**. [[Paper]](https://arxiv.org/abs/2406.14868) [[Code]](https://github.com/swt-user/DMPO)
* 2024.06 **"Adaptive Query Rewriting: Aligning Rewriters through Marginal Probability of Conversational Answers"**. [[Paper]](https://arxiv.org/abs/2406.10991)
* 2024.06 **"Learning to Clarify: Multi-turn Conversations with Action-Based Contrastive Self-Training"**. [[Paper]](https://arxiv.org/abs/2406.00222)
* 2024.02 **"Plan-Grounded Large Language Models for Dual Goal Conversational Settings"**. [[Paper]](https://arxiv.org/abs/2402.01053) [[Code]](https://huggingface.co/dmgcsilva/PlanLLM)
* 2024.07 **"Improving Conversational Abilities of Quantized Large Language Models via Direct Preference Alignment"**. [[Paper]](https://arxiv.org/abs/2407.03051)
* 2024.02 **"Ask Optimal Questions: Aligning Large Language Models with Retriever's Preference in Conversational Search"**. [[Paper]](https://arxiv.org/abs/2402.11827)
* 2024 **"Advancing Open-Domain Conversational Agents - Designing an Engaging System for Natural Multi-Turn Dialogue"**. [[Paper]](https://aclanthology.org/2024.scichat-1.8/)
* 2024.06 **"Alignment For Performance Improvement in Conversation Bots"**. [[Paper]](https://arxiv.org/abs/2406.18954)
* 2024.02 **"Compress to Impress: Unleashing the Potential of Compressive Memory in Real-World Long-Term Conversations"**. [[Paper]](https://arxiv.org/abs/2402.11975) [[Code]](https://github.com/nuochenpku/COMEDY)
* 2024 **"UNIWIZ: A Unified Large Language Model Orchestrated Wizard for Safe Knowledge Grounded Conversations"**. [[Paper]](https://aclanthology.org/2024.findings-acl.102.pdf) [[Code]](https://github.com/souvikdgp16/protoai_uniwiz)
---
#### Multilingual-LLM
* 2024.08 **"FuxiTranyu: A Multilingual Large Language Model Trained with Balanced Data"**. [[Paper]](https://arxiv.org/abs/2408.06273) [[Code]](https://github.com/tjunlp-lab/FuxiTranyu)
* 2024.06 **"LLMs Beyond English: Scaling the Multilingual Capability of LLMs with Cross-Lingual Feedback"**. [[Paper]](https://arxiv.org/abs/2406.01771) [[Code]](https://github.com/boschresearch/ACL24-MLLM)
* 2024.06 **"Preference Tuning For Toxicity Mitigation Generalizes Across Languages"**. [[Paper]](https://arxiv.org/abs/2406.16235) [[Code]](https://github.com/BatsResearch/cross-lingual-detox)
* 2024.01 **"MAPO: Advancing Multilingual Reasoning through Multilingual Alignment-as-Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2401.06838) [[Code]](https://github.com/NJUNLP/MAPO)
* 2024.07 **"RLHF Can Speak Many Languages: Unlocking Multilingual Preference Optimization for LLMs"**. [[Paper]](https://arxiv.org/abs/2407.02552)
* 2024.06 **"The Multilingual Alignment Prism: Aligning Global and Local Preferences to Reduce Harm"**. [[Paper]](https://arxiv.org/abs/2406.18682)
* 2024.04 **"Compass: Large Multilingual Language Model for South-east Asia"**. [[Paper]](https://arxiv.org/abs/2404.09220)
* 2024.08 **"Mitigating Multilingual Hallucination in Large Vision-Language Models"**. [[Paper]](https://arxiv.org/abs/2408.00550) [[Code]](https://github.com/ssmisya/MHR)
* 2024.02 **"Unintended Impacts of LLM Alignment on Global Representation"**. [[Paper]](https://arxiv.org/abs/2402.15018) [[Code]](https://github.com/SALT-NLP/unintended-impacts-of-alignment)
* 2024.07 **"Adapting LLMs to Hebrew: Unveiling DictaLM 2.0 with Enhanced Vocabulary and Instruction Capabilities"**. [[Paper]](https://arxiv.org/abs/2407.07080)
* 2024.01 **"Contrastive Preference Optimization: Pushing the Boundaries of LLM Performance in Machine Translation"**. [[Paper]](https://arxiv.org/abs/2401.08417) [[Code]](https://github.com/fe1ixxu/ALMA)
* 2024.05 **"Word Alignment as Preference for Machine Translation"**. [[Paper]](https://arxiv.org/abs/2405.09223)
* 2023.12 **"SeaLLMs -- Large Language Models for Southeast Asia"**. [[Paper]](https://arxiv.org/abs/2312.00738) [[Code]](https://damo-nlp-sg.github.io/SeaLLMs)
---
#### Long-LLM
* 2024.08 **"LongWriter: Unleashing 10,000+ Word Generation from Long Context LLMs"**. [[Paper]](https://arxiv.org/abs/2408.07055) [[Code]](https://github.com/THUDM/LongWriter)
---
#### Technical Reports of LLMs
* 2024.07 **"Apple Intelligence Foundation Language Models"**. [[Paper]](https://arxiv.org/abs/2407.21075)
* 2024.01 **"H2O-Danube-1.8B Technical Report"**. [[Paper]](https://arxiv.org/abs/2401.16818) [[Code]](https://github.com/h2oai/h2o-llmstudio)
* 2023.12 **"SeaLLMs -- Large Language Models for Southeast Asia"**. [[Paper]](https://arxiv.org/abs/2312.00738) [[Code]](https://damo-nlp-sg.github.io/SeaLLMs)
* 2024.07 **"The Llama 3 Herd of Models"**. [[Paper]](https://arxiv.org/abs/2407.21783) [[Code]](https://llama.meta.com/)
* 2024.06 **"THaLLE: Text Hyperlocally Augmented Large Language Extension -- Technical Report"**. [[Paper]](https://arxiv.org/abs/2406.07505)
* 2024.07 **"Qwen2 Technical Report"**. [[Paper]](https://arxiv.org/abs/2407.10671) [[Code]](https://github.com/QwenLM/Qwen2)
* 2024.04 **"MiniCPM: Unveiling the Potential of Small Language Models with Scalable Training Strategies"**. [[Paper]](https://arxiv.org/abs/2404.06395) [[Code]](https://github.com/OpenBMB/MiniCPM)
* 2024.01 **"DeepSeek LLM: Scaling Open-Source Language Models with Longtermism"**. [[Paper]](https://arxiv.org/abs/2401.02954)
* 2024.08 **"HERMES 3 TECHNICAL REPORT"**. [[Paper]](https://venturebeat.com/wp-content/uploads/2024/08/Hermes-3-Technical-Report.pdf) [[Code]](https://github.com/NousResearch/Hermes-Function-Calling)
* 2024.04 **"Phi-3 Technical Report: A Highly Capable Language Model Locally on Your Phone"**. [[Paper]](https://arxiv.org/abs/2404.14219)
* 2024.06 **"Nemotron-4 340B Technical Report"**. [[Paper]](https://arxiv.org/abs/2406.11704) [[Code]](https://github.com/NVIDIA/NeMo-Aligner)
---
### Math
* 2024.06 **"Step-level Value Preference Optimization for Mathematical Reasoning"**. [[Paper]](https://arxiv.org/abs/2406.10858) [[Code]](https://github.com/MARIO-Math-Reasoning/Super_MARIO)
* 2024.08 **"SIaM: Self-Improving Code-Assisted Mathematical Reasoning of Large Language Models"**. [[Paper]](https://arxiv.org/abs/2408.15565) [[Code]](https://github.com/tencent-ailab/siam)
* 2024.07 **"Step-Controlled DPO: Leveraging Stepwise Error for Enhanced Mathematical Reasoning"**. [[Paper]](https://arxiv.org/abs/2407.00782) [[Code]](https://github.com/mathllm/Step-Controlled_DPO)
* 2024.06 **"Step-DPO: Step-wise Preference Optimization for Long-chain Reasoning of LLMs"**. [[Paper]](https://arxiv.org/abs/2406.18629) [[Code]](https://github.com/dvlab-research/Step-DPO)
* 2024.09 **"Building Math Agents with Multi-Turn Iterative Preference Learning"**. [[Paper]](https://arxiv.org/abs/2409.02392)
* 2024.02 **"Orca-Math: Unlocking the potential of SLMs in Grade School Math"**. [[Paper]](https://arxiv.org/abs/2402.14830)
* 2024.04 **"ChatGLM-Math: Improving Math Problem-Solving in Large Language Models with a Self-Critique Pipeline"**. [[Paper]](https://arxiv.org/abs/2404.02893) [[Code]](https://github.com/THUDM/ChatGLM-Math)
* 2024.04 **"Iterative Reasoning Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2404.19733)
* 2024.06 **"RL on Incorrect Synthetic Data Scales the Efficiency of LLM Math Reasoning by Eight-Fold"**. [[Paper]](https://arxiv.org/abs/2406.14532) [[Code]](https://github.com/ars22/scaling-LLM-math-synthetic-data)
* 2024.05 **"Improving Automated Distractor Generation for Math Multiple-choice Questions with Overgenerate-and-rank"**. [[Paper]](https://arxiv.org/abs/2405.05144) [[Code]](https://github.com/umass-ml4ed/distractor-ranking-BEA)
* 2024.04 **"Self-Explore: Enhancing Mathematical Reasoning in Language Models with Fine-grained Rewards"**. [[Paper]](https://arxiv.org/abs/2404.10346) [[Code]](https://github.com/hbin0701/Self-Explore)
* 2024.03 **"Brain-Inspired Two-Stage Approach: Enhancing Mathematical Reasoning by Imitating Human Thought Processes"**. [[Paper]](https://arxiv.org/abs/2403.00800) [[Code]](https://github.com/cyzhh/Brain)
* 2024.02 **"V-STaR: Training Verifiers for Self-Taught Reasoners"**. [[Paper]](https://arxiv.org/abs/2402.06457)
---
### Code
* 2024.03 **"CodeUltraFeedback: An LLM-as-a-Judge Dataset for Aligning Large Language Models to Coding Preferences"**. [[Paper]](https://arxiv.org/abs/2403.09032) [[Code]](https://github.com/martin-wey/CodeUltraFeedback)
* 2024.06 **"UICoder: Finetuning Large Language Models to Generate User Interface Code through Automated Feedback"**. [[Paper]](https://arxiv.org/abs/2406.07739)
* 2024.06 **"Code-Optimise: Self-Generated Preference Data for Correctness and Efficiency"**. [[Paper]](https://arxiv.org/abs/2406.12502) [[Code]](https://github.com/huawei-noah/HEBO/tree/Code_Optimise)
* 2024.06 **"PLUM : Improving Code LMs with Execution-Guided On-Policy Preference Learning Driven By Synthetic Test Cases"**. [[Paper]](http://arxiv.org/abs/2406.06887)
* 2024.04 **"Performance-Aligned LLMs for Generating Fast Code"**. [[Paper]](https://arxiv.org/abs/2404.18864)
---
### Science
#### Medical Health
* 2024.07 **"Clinical Reading Comprehension with Encoder-Decoder Models Enhanced by Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.14000)
* 2024.06 **"STLLaVA-Med: Self-Training Large Language and Vision Assistant for Medical Question-Answering"**. [[Paper]](https://arxiv.org/abs/2406.19973) [[Code]](https://github.com/heliossun/STLLaVA-Med)
* 2024.06 **"Aqulia-Med LLM: Pioneering Full-Process Open-Source Medical Language Models"**. [[Paper]](https://arxiv.org/abs/2406.12182) [[Code]](https://huggingface.co/BAAI/AquilaMed-RL)
* 2024.06 **"Direct Preference Optimization for Suppressing Hallucinated Prior Exams in Radiology Report Generation"**. [[Paper]](https://arxiv.org/abs/2406.06496)
* 2024.08 **"RuleAlign: Making Large Language Models Better Physicians with Diagnostic Rule Alignment"**. [[Paper]](https://arxiv.org/abs/2408.12579)
* 2023.10 **"Qilin-Med: Multi-stage Knowledge Injection Advanced Medical Large Language Model"**. [[Paper]](https://arxiv.org/abs/2310.09089)
* 2024.06 **"UltraMedical: Building Specialized Generalists in Biomedicine"**. [[Paper]](https://arxiv.org/abs/2406.03949) [[Code]](https://github.com/TsinghuaC3I/UltraMedical)
* 2024.05 **"OLAPH: Improving Factuality in Biomedical Long-form Question Answering"**. [[Paper]](https://arxiv.org/abs/2405.12701) [[Code]](https://github.com/dmis-lab/OLAPH)
* 2024.05 **"Aloe: A Family of Fine-tuned Open Healthcare LLMs"**. [[Paper]](https://arxiv.org/abs/2405.01886)
* 2024.08 **"Med42-v2: A Suite of Clinical LLMs"**. [[Paper]](https://arxiv.org/abs/2408.06142) [[Code]](https://huggingface.co/m42-health)
* 2024.04 **"Hippocrates: An Open-Source Framework for Advancing Large Language Models in Healthcare"**. [[Paper]](https://arxiv.org/abs/2404.16621) [[Code]](https://cyberiada.github.io/Hippocrates/)
* 2024.05 **"PediatricsGPT: Large Language Models as Chinese Medical Assistants for Pediatric Applications"**. [[Paper]](https://arxiv.org/abs/2405.19266) [[Code]](https://github.com/ydk122024/PediatricsGPT)
---
#### Chemistry
* 2024.07 **"DecompDPO: Decomposed Direct Preference Optimization for Structure-Based Drug Design"**. [[Paper]](https://arxiv.org/abs/2407.06338)
* 2024.02 **"ChemLLM: A Chemical Large Language Model"**. [[Paper]](https://arxiv.org/abs/2402.06852)[[Code]](https://huggingface.co/AI4Chem)
* 2024.07 **"Aligning Target-Aware Molecule Diffusion Models with Exact Energy Optimization"**. [[Paper]](https://arxiv.org/abs/2407.01648)[[Code]](https://github.com/MinkaiXu/AliDiff)
* 2024.05 **"Less for More: Enhanced Feedback-aligned Mixed LLMs for Molecule Caption Generation and Fine-Grained NLI Evaluation"**. [[Paper]](https://arxiv.org/abs/2405.13984)
* 2024.05 **"Energy Rank Alignment: Using Preference Optimization to Search Chemical Space at Scale"**. [[Paper]](https://arxiv.org/abs/2405.12961)
* 2024.09 **"SmileyLlama: Modifying Large Language Models for Directed Chemical Space Exploration"**. [[Paper]](https://arxiv.org/abs/2409.02231)
* 2023.10 **"Preference Optimization for Molecular Language Models"**. [[Paper]](https://arxiv.org/abs/2310.12304)
---
#### Biology
* 2024.03 **"Preference optimization of protein language models as a multi-objective binder design paradigm"**. [[Paper]](https://arxiv.org/abs/2403.04187v1)
* 2024 **"Extrapolative protein design through triplet-based preference learning"**. [[Paper]](https://www.amazon.science/publications/extrapolative-protein-design-through-triplet-based-preference-learning)
* 2024.03 **"Antigen-Specific Antibody Design via Direct Energy-based Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2403.16576)
* 2024.05 **"Aligning protein generative models with experimental fitness via Direct Preference Optimization"**. [[Paper]](https://www.biorxiv.org/content/10.1101/2024.05.20.595026v1)[[Code]](https://github.com/evo-design/protein-dpo)
* 2024.06 **"MSAGPT: Neural Prompting Protein Structure Prediction via MSA Generative Pre-Training"**. [[Paper]](https://arxiv.org/abs/2406.05347)[[Code]](https://github.com/THUDM/MSAGPT)
* 2024 **"Saama Technologies at BioLaySumm: Abstract based fine-tuned models with LoRA"**. [[Paper]](https://aclanthology.org/2024.bionlp-1.72.pdf)
---
### Recommendation and Search
* 2024.06 **"Supportiveness-based Knowledge Rewriting for Retrieval-augmented Language Modeling"**. [[Paper]](https://arxiv.org/abs/2406.08116)
---
### Finance
* 2024.08 **"SNFinLLM: Systematic and Nuanced Financial Domain Adaptation of Chinese Large Language Models"**. [[Paper]](https://arxiv.org/abs/2408.02302)
* 2024.06 **"THaLLE: Text Hyperlocally Augmented Large Language Extension - Technical Report"**. [[Paper]](https://arxiv.org/pdf/2406.07505)
* 2024.02 **"FinTral: A Family of GPT-4 Level Multimodal Financial Large Language Models"**. [[Paper]](https://arxiv.org/abs/2402.10986)[[Code]](https://github.com/UBC-NLP/fintral)
---
### Embodied-AI
* 2023.11 **"Embodied Multi-Modal Agent trained by an LLM from a Parallel TextWorld"**. [[Paper]](https://arxiv.org/abs/2311.16714)[[Code]](https://github.com/stevenyangyj/Emma-Alfworld)
* 2024.04 **"Do We Really Need a Complex Agent System? Distill Embodied Agent into a Single Model"**. [[Paper]](https://arxiv.org/abs/2404.04619)
* 2024.06 **"Learning Reward and Policy Jointly from Demonstration and Preference Improves Alignment"**. [[Paper]](https://arxiv.org/abs/2406.06874)
---
### Social Impact (Safety, Privacy, Bias)
* 2024.07 **"BiasDPO: Mitigating Bias in Language Models through Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.13928)[[Code]](https://huggingface.co/datasets/ahmedallam/BiasDPO)
* 2024.07 **"Robust Utility-Preserving Text Anonymization Based on Large Language Models"**. [[Paper]](https://arxiv.org/abs/2407.11770)[[Code]](https://github.com/UKPLab/arxiv2024-rupta)
* 2024.07 **"Exposing Privacy Gaps: Membership Inference Attack on Preference Data for LLM Alignment"**. [[Paper]](https://arxiv.org/abs/2407.06443)
* 2024.06 **"Preference Tuning For Toxicity Mitigation Generalizes Across Languages"**. [[Paper]](https://arxiv.org/abs/2406.16235)
* 2024.11 **"AI-TA: Towards an Intelligent Question-Answer Teaching Assistant using Open-Source LLMs"**. [[Paper]](https://arxiv.org/abs/2311.02775)[[Code]](https://github.com/aita-ai4ed/AITA)
---
## 📜 License
This project is licensed under the [MIT License](LICENSE).

<!-- 
## Analysis
### General Analysis
* 2024.07 **"Evaluating the Effectiveness of Direct Preference Optimization in Aligning Large Language Models"**. [[Paper]](https://arxiv.org/abs/2407.08999)[[Code]]()
* 2024.06 **"Analyzing the Impact of Alignment Techniques on Model Robustness and Accuracy"**. [[Paper]](https://arxiv.org/abs/2406.13588)[[Code]]()
* 2024.06 **"Comparative Analysis of Preference Optimization Methods Across Different Domains"**. [[Paper]](https://arxiv.org/abs/2406.08876)[[Code]]()
* 2024.07 **"A Survey of Direct Preference Optimization Techniques in Modern AI Systems"**. [[Paper]](https://arxiv.org/abs/2407.09273)[[Code]]()

### Performance Evaluation
* 2024.06 **"Metrics for Evaluating Alignment Quality in Multi-Modal Models"**. [[Paper]](https://arxiv.org/abs/2406.17483)[[Code]]()
* 2024.06 **"Benchmarking Direct Preference Optimization for Large Language Models"**. [[Paper]](https://arxiv.org/abs/2406.08430)[[Code]]()
* 2024.06 **"Analyzing the Trade-Offs Between Preference Accuracy and Model Complexity"**. [[Paper]](https://arxiv.org/abs/2406.05132)[[Code]]()
* 2024.07 **"Evaluation Framework for Multimodal Preference Alignment Models"**. [[Paper]](https://arxiv.org/abs/2407.07921)[[Code]]()

### Robustness and Fairness
* 2024.07 **"Assessing Fairness in Direct Preference Optimization Techniques"**. [[Paper]](https://arxiv.org/abs/2407.10456)[[Code]]()
* 2024.06 **"Robustness Analysis of Preference-Based Alignment Methods"**. [[Paper]](https://arxiv.org/abs/2406.12234)[[Code]]()
* 2024.06 **"Impact of Alignment Techniques on Model Fairness in Various Applications"**. [[Paper]](https://arxiv.org/abs/2406.09954)[[Code]]()
* 2024.06 **"Evaluating the Effectiveness of Bias Mitigation Strategies in Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2406.09412)[[Code]]()

### Scalability
* 2024.07 **"Scalability Challenges in Preference Optimization for Large-Scale AI Models"**. [[Paper]](https://arxiv.org/abs/2407.11123)[[Code]]()
* 2024.07 **"Analyzing the Scalability of Direct Preference Optimization Techniques in High-Dimensional Spaces"**. [[Paper]](https://arxiv.org/abs/2407.09214)[[Code]]()
* 2024.06 **"Performance and Efficiency Trade-Offs in Scalable Preference Optimization Algorithms"**. [[Paper]](https://arxiv.org/abs/2406.14329)[[Code]]()

### Interpretability
* 2024.06 **"Interpreting the Effects of Direct Preference Optimization on Model Outputs"**. [[Paper]](https://arxiv.org/abs/2406.15374)[[Code]]()
* 2024.06 **"Understanding the Mechanisms of Alignment in Preference-Based Models"**. [[Paper]](https://arxiv.org/abs/2406.12195)[[Code]]()
* 2024.07 **"Tools and Techniques for Interpreting Preference-Based Model Adjustments"**. [[Paper]](https://arxiv.org/abs/2407.06785)[[Code]]()
* 2024.06 **"Analyzing the Impact of Preference Optimization on Model Interpretability"**. [[Paper]](https://arxiv.org/abs/2406.11589)[[Code]]()

### Theoretical Analysis
* 2024.07 **"Theoretical Foundations of Direct Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2407.10342)[[Code]]()
* 2024.06 **"Analyzing the Theoretical Limits of Preference Alignment Techniques"**. [[Paper]](https://arxiv.org/abs/2406.14629)[[Code]]()
* 2024.07 **"Formal Analysis of Optimization Techniques for Aligning Language Models"**. [[Paper]](https://arxiv.org/abs/2407.12022)[[Code]]()
* 2024.06 **"Theoretical Perspectives on the Efficiency and Effectiveness of Preference Optimization"**. [[Paper]](https://arxiv.org/abs/2406.07553)[[Code]]()
 -->
