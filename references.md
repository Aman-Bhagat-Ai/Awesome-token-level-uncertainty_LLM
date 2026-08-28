# Verified Research Papers

This collection contains **24 scholarly works** selected for relevance to token-level uncertainty, semantic uncertainty, hallucination detection, factuality evaluation, calibration, and mitigation. Metadata and links were checked against authoritative scholarly records such as ACL Anthology, ACM, Nature, PMLR, NeurIPS, ICLR, and arXiv.

## Survey and Review Papers

### Survey of Hallucination in Natural Language Generation
**Authors:** Ziwei Ji, Nayeon Lee, Rita Frieske, Tiezheng Yu, Dan Su, Yan Xu, Etsuko Ishii, Yejin Bang, Andrea Madotto, Pascale Fung  
**Year / Venue:** 2023, ACM Computing Surveys 55(12), Article 248  
**[Paper / DOI](https://doi.org/10.1145/3571730)**  
**Relevance:** Broad survey of hallucination measurement and mitigation; useful for positioning token-level uncertainty within the wider hallucination literature.

### A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions
**Authors:** Lei Huang, Weijiang Yu, Weitao Ma, Weihong Zhong, Zhangyin Feng, Haotian Wang, Qianglong Chen, Weihua Peng, Xiaocheng Feng, Bing Qin, Ting Liu  
**Year / Venue:** 2025, ACM Transactions on Information Systems 43(2), Article 42  
**[Paper / DOI](https://doi.org/10.1145/3703155)**  
**Relevance:** Provides a recent taxonomy and review of LLM hallucination detection, benchmarks, mitigation, and open problems.

## Foundational / Calibration

### On Calibration of Modern Neural Networks
**Authors:** Chuan Guo, Geoff Pleiss, Yu Sun, Kilian Q. Weinberger  
**Year / Venue:** 2017, ICML, PMLR 70:1321–1330  
**[Paper / DOI](https://proceedings.mlr.press/v70/guo17a.html)**  
**Relevance:** Establishes practical calibration concepts and temperature scaling, important when interpreting confidence as a reliability signal.

### Simple and Scalable Predictive Uncertainty Estimation using Deep Ensembles
**Authors:** Balaji Lakshminarayanan, Alexander Pritzel, Charles Blundell  
**Year / Venue:** 2017, NeurIPS  
**[Paper](https://proceedings.neurips.cc/paper/2017/hash/9ef2ed4b7fd2c810847ffa5fa85bce38-Abstract.html)**  
**Relevance:** A foundational uncertainty-estimation method that motivates ensemble-based alternatives to single-model confidence estimates.

### Language Models (Mostly) Know What They Know
**Authors:** Saurav Kadavath et al.  
**Year / Venue:** 2022, arXiv:2207.05221  
**[Paper / DOI](https://arxiv.org/abs/2207.05221)**  
**Relevance:** Studies model self-evaluation, P(True), and P(IK), connecting internal confidence to correctness and calibration.

### TruthfulQA: Measuring How Models Mimic Human Falsehoods
**Authors:** Stephanie Lin, Jacob Hilton, Owain Evans  
**Year / Venue:** 2022, ACL  
**[Paper / DOI](https://aclanthology.org/2022.acl-long.229/)**  
**Relevance:** A standard truthfulness benchmark useful for evaluating whether uncertainty signals correspond to factual reliability.

## Token and Semantic Uncertainty

### Fact-Checking the Output of Large Language Models via Token-Level Uncertainty Quantification
**Authors:** Ekaterina Fadeeva, Aleksandr Rubashevskii, Artem Shelmanov, Sergey Petrakov, Haonan Li, Hamdy Mubarak, Evgenii Tsymbalov, Gleb Kuzmin, Alexander Panchenko, Timothy Baldwin, Preslav Nakov, Maxim Panov  
**Year / Venue:** 2024, Findings of ACL, pp. 9367–9385  
**[Paper / DOI](https://aclanthology.org/2024.findings-acl.558/)**  
**Relevance:** Directly studies token-level uncertainty for claim-level fact checking and is the closest paper to the assigned topic.

### Detecting Hallucinations in Large Language Models Using Semantic Entropy
**Authors:** Sebastian Farquhar, Jannik Kossen, Lorenz Kuhn, Yarin Gal  
**Year / Venue:** 2024, Nature 630, 625–630  
**[Paper / DOI](https://doi.org/10.1038/s41586-024-07421-0)**  
**Relevance:** Shows how semantic entropy can detect hallucinations and highlights the difference between lexical uncertainty and semantic uncertainty.

### Semantic Entropy Probes: Robust and Cheap Hallucination Detection in LLMs
**Authors:** Jannik Kossen, J. Han, M. Razzak, L. Schut, S. Malik, Y. Gal  
**Year / Venue:** 2024, arXiv:2406.15927  
**[Paper / DOI](https://arxiv.org/abs/2406.15927)**  
**Relevance:** Uses single-pass hidden-state probes to approximate semantic uncertainty, addressing the cost of multi-sample semantic entropy.

### A Head to Predict and a Head to Question: Pre-trained Uncertainty Quantification Heads for Hallucination Detection in LLM Outputs
**Authors:** Artem Shelmanov, Ekaterina Fadeeva, Akim Tsvigun, Ivan Tsvigun, Zhuohan Xie, Igor Kiselev, Nico Daheim, Caiqi Zhang, Artem Vazhentsev, Mrinmaya Sachan, Preslav Nakov, Timothy Baldwin  
**Year / Venue:** 2025, EMNLP, pp. 35712–35731  
**[Paper / DOI](https://aclanthology.org/2025.emnlp-main.1809/)**  
**Relevance:** Uses pre-trained uncertainty heads over model internals for hallucination detection and improves on standard uncertainty baselines.

### On Subjective Uncertainty Quantification and Calibration in Natural Language Generation
**Authors:** Ziyu Wang, Christopher C. Holmes  
**Year / Venue:** 2025, AISTATS, PMLR 258:3799–3807  
**[Paper](https://proceedings.mlr.press/v258/wang25i.html)**  
**Relevance:** Develops principled task-specific and epistemic uncertainty measures for free-form generation and calibration.

### UNCERTAINTY-LINE: Length-Invariant Estimation of Uncertainty for Large Language Models
**Authors:** Roman Vashurin, Maiya Goloburda, Preslav Nakov, Maxim Panov  
**Year / Venue:** 2025, EMNLP, pp. 7881–7908  
**[Paper / DOI](https://aclanthology.org/2025.emnlp-main.400/)**  
**Relevance:** Corrects length bias in LLM uncertainty estimates, directly relevant to interpreting token-level uncertainty scores.

## Hallucination and Factuality Evaluation

### SelfCheckGPT: Zero-Resource Black-Box Hallucination Detection for Generative Large Language Models
**Authors:** Potsawee Manakul, Adian Liusie, Mark Gales  
**Year / Venue:** 2023, EMNLP, pp. 9004–9017  
**[Paper / DOI](https://aclanthology.org/2023.emnlp-main.557/)**  
**Relevance:** A black-box sampling-based detector that provides a useful comparison point to white-box token-probability methods.

### HaluEval: A Large-Scale Hallucination Evaluation Benchmark for Large Language Models
**Authors:** Junyi Li, Xiaoxue Cheng, Xin Zhao, Jian-Yun Nie, Ji-Rong Wen  
**Year / Venue:** 2023, EMNLP, pp. 6449–6464  
**[Paper / DOI](https://aclanthology.org/2023.emnlp-main.397/)**  
**Relevance:** Provides a benchmark for hallucination recognition across knowledge dialogue, summarization, and QA settings.

### FActScore: Fine-grained Atomic Evaluation of Factual Precision in Long Form Text Generation
**Authors:** Sewon Min, Kalpesh Krishna, Xinxi Lyu, Mike Lewis, Wen-tau Yih, Pang Wei Koh, Mohit Iyyer, Luke Zettlemoyer, Hannaneh Hajishirzi  
**Year / Venue:** 2023, EMNLP, pp. 12076–12100  
**[Paper / DOI](https://aclanthology.org/2023.emnlp-main.741/)**  
**Relevance:** Introduces atomic-fact factual precision, useful for relating uncertainty scores to fine-grained factual correctness.

### TRUE: Re-evaluating Factual Consistency Evaluation
**Authors:** Or Honovich, Roee Aharoni, Jonathan Herzig, Hagai Taitelbaum, Doron Kukliansy, Vered Cohen, Thomas Scialom, Idan Szpektor, Avinatan Hassidim, Yossi Matias  
**Year / Venue:** 2022, NAACL-HLT, pp. 3905–3920  
**[Paper / DOI](https://aclanthology.org/2022.naacl-main.287/)**  
**Relevance:** Compares factual-consistency metrics across 11 datasets and provides context for evaluating hallucination detectors.

### RAGTruth: A Hallucination Corpus for Developing Trustworthy Retrieval-Augmented Language Models
**Authors:** Cheng Niu, Yuanhao Wu, Juno Zhu, Siliang Xu, KaShun Shum, Randy Zhong, Juntong Song, Tong Zhang  
**Year / Venue:** 2024, ACL, pp. 10862–10878  
**[Paper / DOI](https://aclanthology.org/2024.acl-long.585/)**  
**Relevance:** A word-level hallucination corpus for RAG systems, useful for fine-grained evaluation of unsupported generated spans.

### FELM: Benchmarking Factuality Evaluation of Large Language Models
**Authors:** Shiqi Chen, Yiran Zhao, Jinghan Zhang, I-Chun Chern, Siyang Gao, Pengfei Liu, Junxian He  
**Year / Venue:** 2023, NeurIPS Datasets and Benchmarks  
**[Paper](https://proceedings.neurips.cc/paper_files/paper/2023/file/8b8a7960d343e023a6a0afe37eee6022-Paper-Datasets_and_Benchmarks.pdf)**  
**Relevance:** Fine-grained factuality benchmark spanning world knowledge, science, math, writing/recommendation, and reasoning.

### Evaluating Verifiability in Generative Search Engines
**Authors:** Nelson F. Liu, Tianyi Zhang, Percy Liang  
**Year / Venue:** 2023, Findings of EMNLP, pp. 7001–7025  
**[Paper / DOI](https://aclanthology.org/2023.findings-emnlp.467/)**  
**Relevance:** Measures citation support and verifiability in generative search, providing context for external validation of LLM outputs.

### Enabling Large Language Models to Generate Text with Citations
**Authors:** Tianyu Gao, Howard Yen, Jiatong Yu, Danqi Chen  
**Year / Venue:** 2023, EMNLP  
**[Paper / DOI](https://aclanthology.org/2023.emnlp-main.398/)**  
**Relevance:** Introduces ALCE and evaluates citation correctness, completeness, and fluency for LLM-generated answers.

## Mitigation and Verifiability

### RARR: Researching and Revising What Language Models Say, Using Language Models
**Authors:** Luyu Gao, Zhuyun Dai, Panupong Pasupat, Anthony Chen, Arun Tejasvi Chaganty, Yicheng Fan, Vincent Zhao, Ni Lao, Hongrae Lee, Da-Cheng Juan, Kelvin Guu  
**Year / Venue:** 2023, ACL, pp. 16477–16508  
**[Paper / DOI](https://aclanthology.org/2023.acl-long.910/)**  
**Relevance:** Automatically researches evidence and revises unsupported model outputs, offering a complementary mitigation approach.

### Chain-of-Verification Reduces Hallucination in Large Language Models
**Authors:** Shehzaad Dhuliawala, Mojtaba Komeili, Jing Xu, Roberta Raileanu, Xian Li, Asli Celikyilmaz, Jason Weston  
**Year / Venue:** 2023, arXiv:2309.11495  
**[Paper](https://arxiv.org/abs/2309.11495)**  
**Relevance:** Introduces a verification procedure that asks a model to independently check its draft before producing a final answer.

### DoLa: Decoding by Contrasting Layers Improves Factuality in Large Language Models
**Authors:** Yung-Sung Chuang, Yujia Xie, Hongyin Luo, Yoon Kim, James R. Glass, Pengcheng He  
**Year / Venue:** 2024, ICLR  
**[Paper](https://proceedings.iclr.cc/paper_files/paper/2024/hash/edc36117f795ca52a0cbf6a7b3882859-Abstract-Conference.html)**  
**Relevance:** Uses differences between later and earlier layer logits to improve factuality without retrieval or fine-tuning.

### TruthX: Alleviating Hallucinations by Editing Large Language Models in Truthful Space
**Authors:** Shaolei Zhang, Tian Yu, Yang Feng  
**Year / Venue:** 2024, ACL, pp. 8908–8949  
**[Paper / DOI](https://aclanthology.org/2024.acl-long.483/)**  
**Relevance:** Edits internal representations at inference time to increase truthfulness, illustrating how internal states can encode useful reliability information.
