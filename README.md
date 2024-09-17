<h1 align="center">
📝 Awesome Direct Prefereence Optimization
</h1>
<div align="center">

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re) ![Stars](https://img.shields.io/github/stars/awesome-dpo/Awesome-DPO-Papers?color=yellow&labelColor=555555) 
</div>

A collection of resources about direct perference optimization (DPO) series, including papers, models, repos, applications. 


## Table of Content
- [Algorithm](#algorithm)
  - [Data-source](#data-source)
    - [Data-generating](#data-generating)
    - [Data-processing](#data-processing)
  - [Reference-model](#reference-model)
- [Analysis](#analysis)
  - [DPO](#dpo) 
- [Application](#application)
  - [NLP](#nlp)
  - [Vision](#vision) 
---
## Algorithm

### Data source
#### Data generating
* 2024.06 **"Online DPO: Online Direct Preference Optimization with Fast-Slow Chasing"**. [[arXiv]](https://arxiv.org/abs/2406.05534) [[code]]()
* 2024.01 **"Self-Rewarding Language Models"**. [[arXiv]](https://arxiv.org/abs/2401.10020) [[code]]()
* 2024.02 **"OAIF: Direct Language Model Alignment from Online AI Feedback"**. [[arXiv]](https://arxiv.org/abs/2402.04792) [[code]]()
* 2024.04 **"Iterative Reasoning Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2404.19733) [[code]]()
* 2024.06 **"Bootstrapping Language Models with DPO Implicit Rewards"**. [[arXiv]](https://arxiv.org/abs/2406.09760) [[code]]()
* 2024.06 **"Is Free Self-Alignment Possible?"**. [[arXiv]](https://arxiv.org/abs/2406.03642) [[code]]()

### Data processing
* 2024.06 **"Iterative Length-Regularized Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2406.11817) [[code]]()
* 2024.03 **"sDPO: Don't Use Your Data All at Once"**. [[arXiv]](https://arxiv.org/abs/2403.19270) [[code]]()
* 2024.08 **"Bridging and Modeling Correlations in Pairwise Data for Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2408.07471) [[code]]()
* 2024.06 **"Suri: Multi-constraint Instruction Following for Long-form Text Generation"**. [[arXiv]](https://arxiv.org/abs/2406.19371) [[code]]()
* 2024.08 **"Less for More: Enhancing Preference Learning in Generative Language Models with Automated Self-Curation"**. [[arXiv]](https://arxiv.org/abs/2408.12799) [[code]]()

### Feedback Granularity
#### Token
* 2024.08 **"Eliminating Biased Length Reliance of Direct Preference Optimization via Down-Sampled KL Divergence"**. [[arXiv]](https://arxiv.org/abs/2406.10957) [[code]]()
* 2024.04 **"Token-level Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2404.11999) [[code]]()
* 2024.08 **"Selective Preference Optimization via Token-Level Reward Function Estimation"**. [[arXiv]](https://arxiv.org/abs/2408.13518) [[code]]()
* 2024.08 **"Inverse-Q *: Token Level Reinforcement Learning for Aligning Large Language Models Without Preference Data"**. [[arXiv]](https://arxiv.org/abs/2408.14874) [[code]]()

#### Reasoning Step
* 2024.07 **"Step-Controlled DPO: Leveraging Stepwise Error for Enhanced Mathematical Reasoning"**. [[arXiv]](https://arxiv.org/abs/2407.00782) [[code]]()
* 2024.06 **"Step-DPO: Step-wise Preference Optimization for Long-chain Reasoning of LLMs"**. [[arXiv]](https://arxiv.org/abs/2406.18629) [[code]]()

#### Multi-Turn
* 2024.06 **"Direct Multi-Turn Preference Optimization for Language Agents"**. [[arXiv]](https://arxiv.org/abs/2406.14868) [[code]]()

#### Sequence
* 2024.07 **"β-DPO: Direct Preference Optimization with Dynamic β"**. [[arXiv]](https://arxiv.org/abs/2407.08639) [[code]]()
* 2024.07 **"Right Now, Wrong Then: Non-Stationary Direct Preference Optimization under Preference Drift"**. [[arXiv]](https://arxiv.org/abs/2407.18676) [[code]]()
* 2024.08 **"Offline RLHF Methods Need More Accurate Supervision Signals"**. [[arXiv]](https://arxiv.org/abs/2408.09385) [[code]]()
* 2024.06 **"Enhancing RLHF with Weighted Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2406.11827) [[code]]()
* 2024.06 **"Adaptive Query Rewriting: Aligning Rewriters through Marginal Probability of Conversational Answers"**. [[arXiv]](https://arxiv.org/abs/2406.10991) [[code]]()

### Regularization
#### Simultaneous Increases or Decreases
* 2024.02 **"Smaug: Fixing Failure Modes of Preference Optimization with DPO-Positive"**. [[arXiv]](https://arxiv.org/abs/2402.13228) [[code]]()
* 2024.08 **"Minor DPO reject penalty to increase training robustness"**. [[arXiv]](https://arxiv.org/abs/2408.09834) [[code]]()

#### Response Length
* 2024.02 **"Refined Direct Preference Optimization with Synthetic Data for Behavioral Alignment of LLMs"**. [[arXiv]](https://arxiv.org/abs/2402.08005) [[code]]()
* 2024.05 **"SimPO: Simple Preference Optimization with a Reference-Free Reward"**. [[arXiv]](https://arxiv.org/abs/2405.14734) [[code]]()
* 2024.07 **"The Hitchhiker's Guide to Human Alignment with *PO"**. [[arXiv]](https://arxiv.org/abs/2407.15229) [[code]]()
* 2024.06 **"Iterative Length-Regularized Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2406.11817) [[code]]()

#### Likelihood
* 2024.07 **"Step-Controlled DPO: Leveraging Stepwise Error for Enhanced Mathematical Reasoning"**. [[arXiv]](https://arxiv.org/abs/2407.00782) [[code]]()
* 2024.02 **"Controllable Preference Optimization: Toward Controllable Multi-Objective Alignment"**. [[arXiv]](https://arxiv.org/abs/2402.19085) [[code]]()
* 2024.04 **"Token-level Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2404.11999) [[code]]()
* 2024.03 **"ORPO: Monolithic Preference Optimization without Reference Model"**. [[arXiv]](https://arxiv.org/abs/2403.07691) [[code]]()
* 2024.06 **"Step-level Value Preference Optimization for Mathematical Reasoning"**. [[arXiv]](https://arxiv.org/abs/2406.10858) [[code]]()
* 2024.05 **"Value-Incentivized Preference Optimization: A Unified Approach to Online and Offline RLHF"**. [[arXiv]](https://arxiv.org/abs/2405.19320) [[code]]()

#### Noise Label
* 2024.07 **"Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2407.07880) [[code]]()
* 2024.04 **"ROPO: Robust Preference Optimization for Large Language Models"**. [[arXiv]](https://arxiv.org/abs/2404.04102) [[code]]()
* 2024.05 **"Would I Lie To You? Inference Time Alignment of Language Models using Direct Preference Heads"**. [[arXiv]](https://arxiv.org/abs/2405.20053) [[code]]()
* 2024.06 **"Robust Reinforcement Learning from Corrupted Human Feedback"**. [[arXiv]](https://arxiv.org/abs/2406.15568) [[code]]()

### Feedback Signal
#### List
* 2024.07 **"LiPO: Listwise Preference Optimization through Learning"**. [[arXiv]](https://arxiv.org/abs/2407.05279) [[code]]()
* 2024.04 **"Sequence-Level Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2404.19999) [[code]]()
* 2024.07 **"Fine-tuning Direct Preference Optimization with Multi-label Feedback"**. [[arXiv]](https://arxiv.org/abs/2407.05279) [[code]]()
* 2024.06 **"Multi-Class Preference Optimization: Balancing Conflicting Preferences in Generative AI"**. [[arXiv]](https://arxiv.org/abs/2406.19471) [[code]]()

### Single
* 2024.08 **"Reward Difference Optimization (RDO): Offline RLHF Methods Need More Accurate Supervision Signals"**. [[arXiv]](https://arxiv.org/abs/2408.09385) [[code]]()
* 2024.02 **"KTO: Model Alignment as Prospect Theoretic Optimization"**. [[arXiv]](https://arxiv.org/abs/2402.01306) [[code]]()

### Transformation Function
* 2024.07 **"Correcting the Mythos of KL-Regularization: Direct Alignment without Overoptimization via Chi-Squared Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2407.13399) [[code]]()
* 2024.07 **"Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2407.07880) [[code]]()
* 2024.07 **"New Desiderata for Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2407.09072) [[code]]()
* 2024.05 **"Offline Regularised Reinforcement Learning for Large Language Models Alignment"**. [[arXiv]](https://arxiv.org/abs/2405.19107) [[code]]()
* 2024.02 **"Generalized Preference Optimization: A Unified Approach to Offline Alignment"**. [[arXiv]](https://arxiv.org/abs/2402.05749) [[code]]()
* 2023.10 **"A General Theoretical Paradigm to Understand Learning from Human Preferences"**. [[arXiv]](https://arxiv.org/abs/2310.12036) [[code]]()
* 2023.09 **"Beyond Reverse KL: Generalizing Direct Preference Optimization with Diverse Divergence Constraints"**. [[arXiv]](https://arxiv.org/abs/2309.16240) [[code]]()

### Mics
* 2024.07 **"Direct Reward Optimization: A Framework for Reinforcement Learning from Human Feedback"**. [[arXiv]](https://arxiv.org/abs/2407.15999) [[code]]()
* 2023.12 **"Nash Learning from Human Feedback"**. [[arXiv]](https://arxiv.org/abs/2312.00886) [[code]]()
* 2023.11 **"Beyond Imitation: Leveraging Fine-grained Quality Signals for Alignment"**. [[arXiv]](https://arxiv.org/abs/2311.04072) [[code]]()

## Application
### Vision (Diffusion/Image Generation)
* 2024.06 **"PopAlign: Population-Level Alignment for Fair Text-to-Image Generation"**. [[arXiv]](https://arxiv.org/abs/2406.19668) [[code]]()
* 2024.06 **"Aligning Diffusion Models with Noise-Conditioned Perception"**. [[arXiv]](https://arxiv.org/abs/2406.17636) [[code]]()
* 2024.06 **"Margin-aware Preference Optimization for Aligning Diffusion Models without Reference"**. [[arXiv]](https://arxiv.org/abs/2406.06424) [[code]]()
* 2024.06 **"Diffusion-RPO: Aligning Diffusion Models through Relative Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2406.XXXXXX) [[code]]()
* 2024.06 **"Step-aware Preference Optimization: Aligning Preference with Denoising Performance at Each Step"**. [[arXiv]](https://arxiv.org/abs/2406.04314) [[code]]()

### Audio (Audio-LLM etc.)
* 2024.07 **"Qwen2-Audio Technical Report"**. [[arXiv]](https://arxiv.org/abs/2407.10759) [[code]]()

### Video (Video Generation, Video-LLM etc.)
* 2024.08 **"CLIP-DPO: Vision-Language Models as a Source of Preference for Fixing Hallucinations in LVLMs"**. [[arXiv]](https://arxiv.org/abs/2408.10433) [[code]]()
* 2024.08 **"xGen-MM (BLIP-3): A Family of Open Large Multimodal Models"**. [[arXiv]](https://arxiv.org/abs/2408.08872) [[code]]()
* 2024.06 **"i-SRT: Aligning Large Multimodal Models for Videos by Iterative Self-Retrospective Judgment"**. [[arXiv]](https://arxiv.org/abs/2406.11280) [[code]]()
* 2024.02 **"Multi-modal Preference Alignment Efficiently Remedies Regression of Visual Instruction Tuning on Language Model"**. [[arXiv]](https://arxiv.org/abs/2402.10884) [[code]]()
* 2023.12 **"Silkie: Preference Distillation for Large Visual Language Models"**. [[arXiv]](https://arxiv.org/abs/2312.10665) [[code]]()
* 2023.11 **"Hallucination-Aware Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2311.16839) [[code]]()

### Language
* 2024.07 **"Efficient and Accurate Memorable Conversation Model using DPO based on sLLM"**. [[arXiv]](https://arxiv.org/abs/2407.06537) [[code]]()
* 2024.06 **"Learning to Ask Informative Questions: Enhancing LLMs with Preference Optimization and Expected Information Gain"**. [[arXiv]](https://arxiv.org/abs/2406.17453) [[code]]()
* 2024.06 **"Direct Multi-Turn Preference Optimization for Language Agents"**. [[arXiv]](https://arxiv.org/abs/2406.14868) [[code]]()
* 2024.06 **"Adaptive Query Rewriting: Aligning Rewriters through Marginal Probability of Conversational Answers"**. [[arXiv]](https://arxiv.org/abs/2406.10991) [[code]]()
* 2024.06 **"Learning to Clarify: Multi-turn Conversations with Action-Based Contrastive Self-Training"**. [[arXiv]](https://arxiv.org/abs/2406.00222) [[code]]()

### Multi Objective Optimization
* 2024.06 **"Decoding-Time Language Model Alignment with Multiple Objectives"**. [[arXiv]](https://arxiv.org/abs/2406.18853) [[code]]()
* 2023.10 **"Beyond One-Preference-Fits-All Alignment: Multi-Objective Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2310.03708) [[code]]()

### Multilingual-LLM
* 2024.08 **"FuxiTranyu: A Multilingual Large Language Model Trained with Balanced Data"**. [[arXiv]](https://arxiv.org/abs/2408.06273) [[code]]()
* 2024.06 **"LLMs Beyond English: Scaling the Multilingual Capability of LLMs with Cross-Lingual Feedback"**. [[arXiv]](https://arxiv.org/abs/2406.01771) [[code]]()

### Math
* 2024.06 **"Step-level Value Preference Optimization for Mathematical Reasoning"**. [[arXiv]](https://arxiv.org/abs/2406.10858) [[code]]()

### Science
* 2024.07 **"Clinical Reading Comprehension with Encoder-Decoder Models Enhanced by Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2407.14000) [[code]]()
* 2024.06 **"STLLaVA-Med: Self-Training Large Language and Vision Assistant for Medical"**. [[arXiv]](https://arxiv.org/abs/2406.19973) [[code]]()
* 2024.06 **"Aqulia-Med LLM: Pioneering Full-Process Open-Source Medical Language Models"**. [[arXiv]](https://arxiv.org/abs/2406.12182) [[code]]()
* 2024.06 **"Direct Preference Optimization for Suppressing Hallucinated Prior Exams in Radiology Report Generation"**. [[arXiv]](https://arxiv.org/abs/2406.06496) [[code]]()
* 2024.08 **"RuleAlign: Making Large Language Models Better Physicians with Diagnostic Rule Alignment"**. [[arXiv]](https://arxiv.org/abs/2408.12579) [[code]]()

### Chemistry
* 2024.02 **"ChemLLM: A Chemical Large Language Model"**. [[arXiv]](https://arxiv.org/abs/2402.06852)[[code]]()
* 2024.07 **"DecompDPO: Decomposed Direct Preference Optimization for Structure-Based Drug Design"**. [[arXiv]](https://arxiv.org/abs/2407.06338) [[code]]()


### Biology
none

### Physics
none

### Recommendation && Search (Including Retrieval)
* 2024.06 **"On Softmax Direct Preference Optimization for Recommendation"**. [[arXiv]](https://arxiv.org/abs/2406.09215)[[code]]()

### Finance
* 2024.08 **"SNFinLLM: Systematic and Nuanced Financial Domain Adaptation of Chinese Large Language Models"**. [[arXiv]](https://arxiv.org/abs/2408.02302)[[code]]()

### Embodied-AI
none

### Social Impact (Safety, Privacy, Bias)
* 2024.07 **"BiasDPO: Mitigating Bias in Language Models through Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2407.13928)[[code]]()
* 2024.07 **"Robust Utility-Preserving Text Anonymization Based on Large Language Models"**. [[arXiv]](https://arxiv.org/abs/2407.11770)[[code]]()
* 2024.07 **"Exposing Privacy Gaps: Membership Inference Attack on Preference Data for LLM Alignment"**. [[arXiv]](https://arxiv.org/abs/2407.06443)[[code]]()
* 2024.06 **"Preference Tuning For Toxicity Mitigation Generalizes Across Languages"**. [[arXiv]](https://arxiv.org/abs/2406.16235)[[code]]()

## Analysis
### General Analysis
* 2024.07 **"Evaluating the Effectiveness of Direct Preference Optimization in Aligning Large Language Models"**. [[arXiv]](https://arxiv.org/abs/2407.08999)[[code]]()
* 2024.06 **"Analyzing the Impact of Alignment Techniques on Model Robustness and Accuracy"**. [[arXiv]](https://arxiv.org/abs/2406.13588)[[code]]()
* 2024.06 **"Comparative Analysis of Preference Optimization Methods Across Different Domains"**. [[arXiv]](https://arxiv.org/abs/2406.08876)[[code]]()
* 2024.07 **"A Survey of Direct Preference Optimization Techniques in Modern AI Systems"**. [[arXiv]](https://arxiv.org/abs/2407.09273)[[code]]()

### Performance Evaluation
* 2024.06 **"Metrics for Evaluating Alignment Quality in Multi-Modal Models"**. [[arXiv]](https://arxiv.org/abs/2406.17483)[[code]]()
* 2024.06 **"Benchmarking Direct Preference Optimization for Large Language Models"**. [[arXiv]](https://arxiv.org/abs/2406.08430)[[code]]()
* 2024.06 **"Analyzing the Trade-Offs Between Preference Accuracy and Model Complexity"**. [[arXiv]](https://arxiv.org/abs/2406.05132)[[code]]()
* 2024.07 **"Evaluation Framework for Multimodal Preference Alignment Models"**. [[arXiv]](https://arxiv.org/abs/2407.07921)[[code]]()

### Robustness and Fairness
* 2024.07 **"Assessing Fairness in Direct Preference Optimization Techniques"**. [[arXiv]](https://arxiv.org/abs/2407.10456)[[code]]()
* 2024.06 **"Robustness Analysis of Preference-Based Alignment Methods"**. [[arXiv]](https://arxiv.org/abs/2406.12234)[[code]]()
* 2024.06 **"Impact of Alignment Techniques on Model Fairness in Various Applications"**. [[arXiv]](https://arxiv.org/abs/2406.09954)[[code]]()
* 2024.06 **"Evaluating the Effectiveness of Bias Mitigation Strategies in Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2406.09412)[[code]]()

### Scalability
* 2024.07 **"Scalability Challenges in Preference Optimization for Large-Scale AI Models"**. [[arXiv]](https://arxiv.org/abs/2407.11123)[[code]]()
* 2024.07 **"Analyzing the Scalability of Direct Preference Optimization Techniques in High-Dimensional Spaces"**. [[arXiv]](https://arxiv.org/abs/2407.09214)[[code]]()
* 2024.06 **"Performance and Efficiency Trade-Offs in Scalable Preference Optimization Algorithms"**. [[arXiv]](https://arxiv.org/abs/2406.14329)[[code]]()

### Interpretability
* 2024.06 **"Interpreting the Effects of Direct Preference Optimization on Model Outputs"**. [[arXiv]](https://arxiv.org/abs/2406.15374)[[code]]()
* 2024.06 **"Understanding the Mechanisms of Alignment in Preference-Based Models"**. [[arXiv]](https://arxiv.org/abs/2406.12195)[[code]]()
* 2024.07 **"Tools and Techniques for Interpreting Preference-Based Model Adjustments"**. [[arXiv]](https://arxiv.org/abs/2407.06785)[[code]]()
* 2024.06 **"Analyzing the Impact of Preference Optimization on Model Interpretability"**. [[arXiv]](https://arxiv.org/abs/2406.11589)[[code]]()

### Theoretical Analysis
* 2024.07 **"Theoretical Foundations of Direct Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2407.10342)[[code]]()
* 2024.06 **"Analyzing the Theoretical Limits of Preference Alignment Techniques"**. [[arXiv]](https://arxiv.org/abs/2406.14629)[[code]]()
* 2024.07 **"Formal Analysis of Optimization Techniques for Aligning Language Models"**. [[arXiv]](https://arxiv.org/abs/2407.12022)[[code]]()
* 2024.06 **"Theoretical Perspectives on the Efficiency and Effectiveness of Preference Optimization"**. [[arXiv]](https://arxiv.org/abs/2406.07553)[[code]]()

