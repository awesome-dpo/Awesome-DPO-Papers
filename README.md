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
* `2024.06` **"Online DPO: Online Direct Preference Optimization with Fast-Slow Chasing"**. [[arXiv]](https://arxiv.org/abs/2406.05534) [[code]]()
* `2024.01` **"Self-Rewarding Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2401.10020)
* `2024.02` **"OAIF: Direct Language Model Alignment from Online AI Feedback"**. arXiv. [Paper](https://arxiv.org/abs/2402.04792)
* `2024.04` **"Iterative Reasoning Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2404.19733)
* `2024.06` **"Bootstrapping Language Models with DPO Implicit Rewards"**. arXiv. [Paper](https://arxiv.org/abs/2406.09760)
* `2024.06` **"Is Free Self-Alignment Possible?"**. arXiv. [Paper](https://arxiv.org/abs/2406.03642)
#### Data processing
7. `2024.06` **"Iterative Length-Regularized Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2406.11817)

8. `2024.03` **"sDPO: Don't Use Your Data All at Once"**. arXiv. [Paper](https://arxiv.org/abs/2403.19270)

9. `2024.08` **"Bridging and Modeling Correlations in Pairwise Data for Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2408.07471)

10. `2024.06` **"Suri: Multi-constraint Instruction Following for Long-form Text Generation"**. arXiv. [Paper](https://arxiv.org/abs/2406.19371)

11. `2024.08` **"Less for More: Enhancing Preference Learning in Generative Language Models with Automated Self-Curation"**. arXiv. [Paper](https://arxiv.org/abs/2408.12799)
### Feedback Granularity
#### Token
12. `2024.08` **"Eliminating Biased Length Reliance of Direct Preference Optimization via Down-Sampled KL Divergence"**. arXiv. [Paper](https://arxiv.org/abs/2406.10957)

13. `2024.04` **"Token-level Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2404.11999)

14. `2024.08` **"Selective Preference Optimization via Token-Level Reward Function Estimation"**. arXiv. [Paper](https://arxiv.org/abs/2408.13518)

15. `2024.08` **"Inverse-Q *: Token Level Reinforcement Learning for Aligning Large Language Models Without Preference Data"**. arXiv. [Paper](https://arxiv.org/abs/2408.14874)
#### Reasoning Step

16. `2024.07` **"Step-Controlled DPO: Leveraging Stepwise Error for Enhanced Mathematical Reasoning"**. arXiv. [Paper](https://arxiv.org/abs/2407.00782)
17. 
18. `2024.06` **"Step-DPO: Step-wise Preference Optimization for Long-chain Reasoning of LLMs"**. arXiv. [Paper](https://arxiv.org/abs/2406.18629)
#### Multi-Turn
18. `2024.06` **"Direct Multi-Turn Preference Optimization for Language Agents"**. arXiv. [Paper](https://arxiv.org/abs/2406.14868)
#### Sequence
19. `2024.07` **"β-DPO: Direct Preference Optimization with Dynamic β"**. arXiv. [Paper](https://arxiv.org/abs/2407.08639)

20. `2024.07` **"Right Now, Wrong Then: Non-Stationary Direct Preference Optimization under Preference Drift"**. arXiv. [Paper](https://arxiv.org/abs/2407.18676)

21. `2024.08` **"Offline RLHF Methods Need More Accurate Supervision Signals"**. arXiv. [Paper](https://arxiv.org/abs/2408.09385)

22. `2024.06` **"Enhancing RLHF with Weighted Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2406.11827)

23. `2024.06` **"Adaptive Query Rewriting: Aligning Rewriters through Marginal Probability of Conversational Answers"**. arXiv. [Paper](https://arxiv.org/abs/2406.10991)
### Regularization
#### Simultaneous Increases or Decreases
24. `2024.02` **"Smaug: Fixing Failure Modes of Preference Optimization with DPO-Positive"**. arXiv. [Paper](https://arxiv.org/abs/2402.13228)

25. `2024.08` **"Minor DPO reject penalty to increase training robustness"**. arXiv. [Paper](https://arxiv.org/abs/2408.09834)
### Response Length

26. `2024.02` **"Refined Direct Preference Optimization with Synthetic Data for Behavioral Alignment of LLMs"**. arXiv. [Paper](https://arxiv.org/abs/2402.08005)

27. `2024.05` **"SimPO: Simple Preference Optimization with a Reference-Free Reward"**. arXiv. [Paper](https://arxiv.org/abs/2405.14734)

28. `2024.07` **"The Hitchhiker's Guide to Human Alignment with *PO"**. arXiv. [Paper](https://arxiv.org/abs/2407.15229)

29. `2024.06` **"Iterative Length-Regularized Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2406.11817)
#### Likelihood
30. `2024.07` **"Step-Controlled DPO: Leveraging Stepwise Error for Enhanced Mathematical Reasoning"**. arXiv. [Paper](https://arxiv.org/abs/2407.00782)
31. `2024.02` **"Controllable Preference Optimization: Toward Controllable Multi-Objective Alignment"**. arXiv. [Paper](https://arxiv.org/abs/2402.19085)

32. `2024.04` **"Token-level Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2404.11999)

33. `2024.03` **"ORPO: Monolithic Preference Optimization without Reference Model"**. arXiv. [Paper](https://arxiv.org/abs/2403.07691)

34. `2024.06` **"Step-level Value Preference Optimization for Mathematical Reasoning"**. arXiv. [Paper](https://arxiv.org/abs/2406.10858)

35. `2024.05` **"Value-Incentivized Preference Optimization: A Unified Approach to Online and Offline RLHF"**. arXiv. [Paper](https://arxiv.org/abs/2405.19320)
#### Noise Label
36. `2024.07` **"Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2407.07880)

37. `2024.04` **"ROPO: Robust Preference Optimization for Large Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2404.04102)

38. `2024.05` **"Would I Lie To You? Inference Time Alignment of Language Models using Direct Preference Heads"**. arXiv. [Paper](https://arxiv.org/abs/2405.20053)

39. `2024.06` **"Robust Reinforcement Learning from Corrupted Human Feedback"**. arXiv. [Paper](https://arxiv.org/abs/2406.15568)
### Feedback Signal
#### List
40. `2024.07` **"LiPO: Listwise Preference Optimization through Learning"**. arXiv. [Paper](https://arxiv.org/abs/2407.05279)

41. `2024.04` **"Sequence-Level Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2404.19999)

42. `2024.07` **"Fine-tuning Direct Preference Optimization with Multi-label Feedback"**. arXiv. [Paper](https://arxiv.org/abs/2407.05279)

43. `2024.06` **"Multi-Class Preference Optimization Using Probabilistic Ranking"**. arXiv. [Paper](https://arxiv.org/abs/2406.05129)

44. `2024.08` **"Soft Preference Ordering and Fine-Tuning Techniques"**. arXiv. [Paper](https://arxiv.org/abs/2408.12022)
#### Single
45. `2024.02` **"KTO: Model Alignment as Prospect Theoretic Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2402.01306)

46. `2024.08` **"Reward Difference Optimization (RDO): Offline RLHF Methods Need More Accurate Supervision Signals"**. arXiv. [Paper](https://arxiv.org/abs/2408.09385)
### Transformation Function
47. `2024.02` **"Generalized Preference Optimization: A Unified Approach to Offline Alignment"**. arXiv. [Paper](https://arxiv.org/abs/2402.05749)

48. `2023.09` **"Beyond Reverse KL: Generalizing Direct Preference Optimization with Diverse Divergence Constraints"**. arXiv. [Paper](https://arxiv.org/abs/2309.16240)

49. `2023.10` **"A General Theoretical Paradigm to Understand Learning from Human Preferences"**. arXiv. [Paper](https://arxiv.org/abs/2310.12036)

50. `2024.05` **"Offline Regularised Reinforcement Learning for Large Language Models Alignment"**. arXiv. [Paper](https://arxiv.org/abs/2405.19107)

51. `2024.07` **"Correcting the Mythos of KL-Regularization: Direct Alignment without Overoptimization via Chi-Squared Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2407.13399)

52. `2024.07` **"Towards Robust Alignment of Language Models: Distributionally Robustifying Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2407.07880)

53. `2024.07` **"New Desiderata for Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2407.09072)
#### Mics
54. `2023.12` **"Nash Learning from Human Feedback"**. arXiv. [Paper](https://arxiv.org/abs/2312.00886)

55. `2023.11` **"Beyond Imitation: Leveraging Fine-grained Quality Signals for Alignment"**. arXiv. [Paper](https://arxiv.org/abs/2311.04072)

56. `2024.07` **"Direct Reward Optimization: A Framework for Reinforcement Learning from Human Feedback"**. arXiv. [Paper](https://arxiv.org/abs/2407.15999)
## Application
### Vision (Diffusion/Image Generation)
1. `2024.06` **"PopAlign: Population-Level Alignment for Fair Text-to-Image Generation"**. arXiv. [Paper](https://arxiv.org/abs/2406.19668)

2. `2024.06` **"Aligning Diffusion Models with Noise-Conditioned Perception"**. arXiv. [Paper](https://arxiv.org/abs/2406.17636)

3. `2024.06` **"Margin-aware Preference Optimization for Aligning Diffusion Models without Reference"**. arXiv. [Paper](https://arxiv.org/abs/2406.06424)

4. `2024.06` **"Diffusion-RPO: Aligning Diffusion Models through Relative Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2406.XXXXXX)

5. `2024.06` **"Step-aware Preference Optimization: Aligning Preference with Denoising Performance at Each Step"**. arXiv. [Paper](https://arxiv.org/abs/2406.04314)

### Audio (Audio-LLM etc.)
6. `2024.07` **"Qwen2-Audio Technical Report"**. arXiv. [Paper](https://arxiv.org/abs/2407.10759)


### Video (Video Generation, Video-LLM etc.)
7. `2023.12` **"Silkie: Preference Distillation for Large Visual Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2312.10665)

8. `2024.02` **"Multi-modal Preference Alignment Efficiently Remedies Regression of Visual Instruction Tuning on Language Model"**. arXiv. [Paper](https://arxiv.org/abs/2402.10884)

9. `2023.11` **"Hallucination-Aware Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2311.16839)

10. `2024.08` **"CLIP-DPO: Vision-Language Models as a Source of Preference for Fixing Hallucinations in LVLMs"**. arXiv. [Paper](https://arxiv.org/abs/2408.10433)

11. `2024.08` **"xGen-MM (BLIP-3): A Family of Open Large Multimodal Models"**. arXiv. [Paper](https://arxiv.org/abs/2408.08872)

12. `2024.06` **"i-SRT: Aligning Large Multimodal Models for Videos by Iterative Self-Retrospective Judgment"**. arXiv. [Paper](https://arxiv.org/abs/2406.11280)


### Language
13. `2024.07` **"Efficient and Accurate Memorable Conversation Model using DPO based on sLLM"**. arXiv. [Paper](https://arxiv.org/abs/2407.06537)

14. `2024.06` **"Learning to Ask Informative Questions: Enhancing LLMs with Preference Optimization and Expected Information Gain"**. arXiv. [Paper](https://arxiv.org/abs/2406.17453)

15. `2024.06` **"Direct Multi-Turn Preference Optimization for Language Agents"**. arXiv. [Paper](https://arxiv.org/abs/2406.14868)

16. `2024.06` **"Adaptive Query Rewriting: Aligning Rewriters through Marginal Probability of Conversational Answers"**. arXiv. [Paper](https://arxiv.org/abs/2406.10991)

17. `2024.06` **"Learning to Clarify: Multi-turn Conversations with Action-Based Contrastive Self-Training"**. arXiv. [Paper](https://arxiv.org/abs/2406.00222)


### Multi Objective Optimization
18. `2023.10` **"Beyond One-Preference-Fits-All Alignment: Multi-Objective Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2310.03708)

19. `2024.06` **"Decoding-Time Language Model Alignment with Multiple Objectives"**. arXiv. [Paper](https://arxiv.org/abs/2406.18853)

### Multilingual-LLM
20. `2024.08` **"FuxiTranyu: A Multilingual Large Language Model Trained with Balanced Data"**. arXiv. [Paper](https://arxiv.org/abs/2408.06273)

21. `2024.06` **"LLMs Beyond English: Scaling the Multilingual Capability of LLMs with Cross-Lingual Feedback"**. arXiv. [Paper](https://arxiv.org/abs/2406.01771)

### Math
22. `2024.06` **"Step-level Value Preference Optimization for Mathematical Reasoning"**. arXiv. [Paper](https://arxiv.org/abs/2406.10858)


### Code
### Science
23. `2024.07` **"Clinical Reading Comprehension with Encoder-Decoder Models Enhanced by Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2407.14000)

24. `2024.06` **"STLLaVA-Med: Self-Training Large Language and Vision Assistant for Medical"**. arXiv. [Paper](https://arxiv.org/abs/2406.19973)

25. `2024.06` **"Aqulia-Med LLM: Pioneering Full-Process Open-Source Medical Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2406.12182)

26. `2024.06` **"Direct Preference Optimization for Suppressing Hallucinated Prior Exams in Radiology Report Generation"**. arXiv. [Paper](https://arxiv.org/abs/2406.06496)

27. `2024.08` **"RuleAlign: Making Large Language Models Better Physicians with Diagnostic Rule Alignment"**. arXiv. [Paper](https://arxiv.org/abs/2408.12579)


### Chemistry
28. `2024.07` **"DecompDPO: Decomposed Direct Preference Optimization for Structure-Based Drug Design"**. arXiv. [Paper](https://arxiv.org/abs/2407.13981)

29. `2024.02` **"ChemLLM: A Chemical Large Language Model"**. arXiv. [Paper](https://arxiv.org/abs/2402.06852)


### Biology
none
### Physics
none
### Recommendation && Search (Including Retrieval)
30. `2024.06` **"On Softmax Direct Preference Optimization for Recommendation"**. arXiv. [Paper](https://arxiv.org/abs/2406.09215)


### Finance
31. `2024.08` **"SNFinLLM: Systematic and Nuanced Financial Domain Adaptation of Chinese Large Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2408.02302)


### Embodied-AI
none
### Social Impact (Safety, Privacy, Bias)
32. `2024.07` **"BiasDPO: Mitigating Bias in Language Models through Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2407.13928)

33. `2024.07` **"Robust Utility-Preserving Text Anonymization Based on Large Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2407.11770)

34. `2024.07` **"Exposing Privacy Gaps: Membership Inference Attack on Preference Data for LLM Alignment"**. arXiv. [Paper](https://arxiv.org/abs/2407.06443)

35. `2024.06` **"Preference Tuning For Toxicity Mitigation Generalizes Across Languages"**. arXiv. [Paper](https://arxiv.org/abs/2406.16235)
## Analysis
### General Analysis

1. `2024.07` **"Evaluating the Effectiveness of Direct Preference Optimization in Aligning Large Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2407.08999)

2. `2024.06` **"Analyzing the Impact of Alignment Techniques on Model Robustness and Accuracy"**. arXiv. [Paper](https://arxiv.org/abs/2406.13588)

3. `2024.06` **"Comparative Analysis of Preference Optimization Methods Across Different Domains"**. arXiv. [Paper](https://arxiv.org/abs/2406.08876)

4. `2024.07` **"A Survey of Direct Preference Optimization Techniques in Modern AI Systems"**. arXiv. [Paper](https://arxiv.org/abs/2407.09273)

### Performance Evaluation

5. `2024.06` **"Metrics for Evaluating Alignment Quality in Multi-Modal Models"**. arXiv. [Paper](https://arxiv.org/abs/2406.17483)

6. `2024.06` **"Benchmarking Direct Preference Optimization for Large Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2406.08430)

7. `2024.06` **"Analyzing the Trade-Offs Between Preference Accuracy and Model Complexity"**. arXiv. [Paper](https://arxiv.org/abs/2406.05132)

8. `2024.07` **"Evaluation Framework for Multimodal Preference Alignment Models"**. arXiv. [Paper](https://arxiv.org/abs/2407.07921)

### Robustness and Fairness

9. `2024.07` **"Assessing Fairness in Direct Preference Optimization Techniques"**. arXiv. [Paper](https://arxiv.org/abs/2407.10456)

10. `2024.06` **"Robustness Analysis of Preference-Based Alignment Methods"**. arXiv. [Paper](https://arxiv.org/abs/2406.12234)

11. `2024.06` **"Impact of Alignment Techniques on Model Fairness in Various Applications"**. arXiv. [Paper](https://arxiv.org/abs/2406.09954)

12. `2024.06` **"Evaluating the Effectiveness of Bias Mitigation Strategies in Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2406.09412)

### Scalability

13. `2024.07` **"Scalability Challenges in Preference Optimization for Large-Scale AI Models"**. arXiv. [Paper](https://arxiv.org/abs/2407.11123)

14. `2024.07` **"Analyzing the Scalability of Direct Preference Optimization Techniques in High-Dimensional Spaces"**. arXiv. [Paper](https://arxiv.org/abs/2407.09214)

15. `2024.06` **"Performance and Efficiency Trade-Offs in Scalable Preference Optimization Algorithms"**. arXiv. [Paper](https://arxiv.org/abs/2406.14329)

### Interpretability

16. `2024.06` **"Interpreting the Effects of Direct Preference Optimization on Model Outputs"**. arXiv. [Paper](https://arxiv.org/abs/2406.15374)

17. `2024.06` **"Understanding the Mechanisms of Alignment in Preference-Based Models"**. arXiv. [Paper](https://arxiv.org/abs/2406.12195)

18. `2024.07` **"Tools and Techniques for Interpreting Preference-Based Model Adjustments"**. arXiv. [Paper](https://arxiv.org/abs/2407.06785)

19. `2024.06` **"Analyzing the Impact of Preference Optimization on Model Interpretability"**. arXiv. [Paper](https://arxiv.org/abs/2406.11589)

### Theoretical Analysis

20. `2024.07` **"Theoretical Foundations of Direct Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2407.10342)

21. `2024.06` **"Analyzing the Theoretical Limits of Preference Alignment Techniques"**. arXiv. [Paper](https://arxiv.org/abs/2406.14629)

22. `2024.07` **"Formal Analysis of Optimization Techniques for Aligning Language Models"**. arXiv. [Paper](https://arxiv.org/abs/2407.12022)

23. `2024.06` **"Theoretical Perspectives on the Efficiency and Effectiveness of Preference Optimization"**. arXiv. [Paper](https://arxiv.org/abs/2406.07553)
