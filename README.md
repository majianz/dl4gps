# Deep Learning for Geometry Problem Solving (DL4GPS)

[![Awesome](https://awesome.re/badge.svg)](https://github.com/majianz/gps-survey) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Survey](https://img.shields.io/badge/Survey-DL4GPS-blue)](https://github.com/majianz/gps-survey) 

This repository is the reading list on ***Deep Learning for Geometry Problem Solving (DL4GPS)***. You can also search for corresponding papers by year in folders named after the corresponding time. We will update the papers after a certain period of time. The current deadline for included papers is **April 2025**.

- :large_blue_circle: indicates that the work is not specifically designed for geometry problems.

- :small_red_triangle: represents geometry tasks other than geometry problem solving.

- :x: indicates no deep learning method is used.

:bell: If you have any suggestions or notice something we missed, please don't hesitate to let us know. You can directly email Jianzhe Ma (majianzhe@ruc.edu.cn), or post an issue on this repo.

## Table of Contents

- [Surveys](#surveys)
- [Tasks and Datasets - Fundamental Tasks](#tasks-and-datasets---fundamental-tasks)
    - [Geometry Problem Parsing](#geometry-problem-parsing)
        - [Semantic Parsing for Geometry Problem](#semantic-parsing-for-geometry-problem)
        - [Geometric Diagram Parsing](#geometric-diagram-parsing)
    - [Geometry Problem Understanding](#geometry-problem-understanding)
        - [Geometric Diagram Understanding](#geometric-diagram-understanding)
        - [Geometric Relation Extraction](#geometric-relation-extraction)
        - [Geometric Knowledge Prediction](#geometric-knowledge-prediction)
- [Tasks and Datasets - Core Tasks](#tasks-and-datasets---core-tasks)
    - [Geometry Theorem Proving](#geometry-theorem-proving)
    - [Geometric Numerical Calculation](#geometric-numerical-calculation)
- [Tasks and Datasets - Composite Tasks](#tasks-and-datasets---composite-tasks)
    - [Mathematical Reasoning](#mathematical-reasoning)
    - [Multimodal Perception](#multimodal-perception)
- [Related Surveys](#related-surveys)

## Surveys

1. **Plane Geometry Problem Solving with Multi-modal Reasoning: A Survey**, arXiv:2505.14340 [[paper](https://arxiv.org/abs/2505.14340)]

2. **Towards Geometry Problem Solving in the Large Model Era: A Survey**, arXiv:2506.02690 [[paper](https://arxiv.org/abs/2506.02690)]

## Tasks and Datasets - Fundamental Tasks

### Geometry Problem Parsing

1. **Extracting structured information from the textual description of geometry word problems**, NLPIR 2023 [[paper](https://dl.acm.org/doi/abs/10.1145/3639233.3639255)] :x:

1. [ElementaryGeometryQA] **Automatic Extraction of Structured Information from Elementary Level Geometry Questions into Logic Forms**, Multimed Tools Appl 2024 [[paper](https://link.springer.com/article/10.1007/s11042-024-20463-w)]

1. **Evaluating Automated Geometric Problem Solving With Formal Language Generation on Large Multimodal Models**, IEIR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10959992)]

1. **FGeo-Parser: Autoformalization and Solution of Plane Geometric Problems**, Symmetry 2025 [[paper](https://www.mdpi.com/2073-8994/17/1/8)]

### Semantic Parsing for Geometry Problem

1. **Semantic Parsing of Pre-University Math Problems**, ACL 2017 [[paper](https://aclanthology.org/P17-1195/)] :x:

1. **Beyond Sentential Semantic Parsing: Tackling the Math SAT with a Cascade of Tree Transducers**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1083/)] :large_blue_circle: :x:

1. **From Textbooks to Knowledge: A Case Study in Harvesting Axiomatic Knowledge from Textbooks to Solve Geometry Problems**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1081/)] :x:

1. **Discourse in Multimedia: A Case Study in Extracting Geometry Knowledge from Textbooks**, CL 2019 [[paper](https://aclanthology.org/J19-4002/)] :x:

1. **Extending a Parser to Distant Domains Using a Few Dozen Partially Annotated Examples**, ACL 2018 [[paper](https://aclanthology.org/P18-1110/)]

1. **A Neural Semantic Parser for Math Problems Incorporating Multi-Sentence Information**, TALLIP 2019 [[paper](https://dl.acm.org/doi/abs/10.1145/3314939)] :large_blue_circle:

1. **Two-step memory networks for deep semantic parsing of geometry word problems**, SOFSEM 2020 [[paper](https://dl.acm.org/doi/abs/10.1007/978-3-030-38919-2_57)]

1. **Semantic parsing of geometry statements using supervised machine learning on Synthetic Data**, NatFoM 2021 CICM Workshop [[paper](https://hal.science/hal-03327994/document)]

1. **Cognitive Patterns for Semantic Presentation of Natural-Language Descriptions of Well-Formalizable Problems**, RCAI 2021 [[paper](https://link.springer.com/chapter/10.1007/978-3-030-86855-0_22)] :x:

1. **Exploration of Formalization Techniques for Geometric Entities in Planar Geometry Proposition Texts**, JAIP 2025 [[paper](https://www.clausiuspress.com/assets/default/article/2025/02/27/article_1740641608.pdf)]

### Geometric Diagram Parsing

1. **Retrieving Geometric Information from Images: The Case of Hand-Drawn Diagrams**, KDD 2017 [[paper](https://link.springer.com/article/10.1007/s10618-017-0494-1)] :x:

1. **A Novel Geometric Information Retrieval Tool for Images of Geometric Diagrams**, ICISE-IE 2020 [[paper](https://ieeexplore.ieee.org/abstract/document/9418805)]

1. [2Dgeometricshapes] **2D Geometric Shapes Dataset – For Machine Learning and Pattern Recognition**, Data in Brief 2020 [[paper](https://www.sciencedirect.com/science/article/pii/S2352340920309847)] [[data](https://data.mendeley.com/datasets/wzr2yv7r53/1)]

1. **A Paradigm of Diagram Understanding in Problem Solving**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678637)] :x:

1. [PGDP5K] **Plane Geometry Diagram Parsing**, IJCAI 2022 [[paper](https://www.ijcai.org/proceedings/2022/228)] [[data](https://github.com/mingliangzhang2018/PGDP)]

1. **Learning to Understand Plane Geometry Diagram**, NeurIPS 2022 MATH-AI Workshop [[paper](https://mathai2022.github.io/papers/6.pdf)]

1. **PGDP5K: A Diagram Parsing Dataset for Plane Geometry Problems**, ICPR 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/9956397)]

1. **Usage of Stacked Long Short-Term Memory for Recognition of 3D Analytic Geometry Elements**, ICAART 2022 [[paper](https://www.scitepress.org/Papers/2022/108989/108989.pdf)]

1. **Solving Algebraic Problems with Geometry Diagrams Using Syntax-Semantics Diagram Understanding**, Computers, Materials & Continua 2023 [[paper](https://www.researchgate.net/profile/Litian-Huang/publication/375217917_Solving_Algebraic_Problems_with_Geometry_Diagrams_Using_Syntax-Semantics_Diagram_Understanding/links/654715da3fa26f66f4d60625/Solving-Algebraic-Problems-with-Geometry-Diagrams-Using-Syntax-Semantics-Diagram-Understanding.pdf)] :x:

1. [BBH-geometricshapes] **Challenging BIG-Bench Tasks and Whether Chain-of-Thought Can Solve Them**, Findings of ACL 2023 [[paper](https://aclanthology.org/2023.findings-acl.824/)] [[data](https://huggingface.co/datasets/Joschka/big_bench_hard)]

1. **2D Shape Detection for Solving Geometry Word Problems**, IETE J. Res. 2024 [[paper](https://www.tandfonline.com/doi/abs/10.1080/03772063.2023.2274914)] :x:

1. [SP-1] **Slow Perception: Let's Perceive Geometric Figures Step-by-Step**, arXiv:2412.20631 [[paper](https://arxiv.org/abs/2412.20631)] [[data](https://github.com/Ucas-HaoranWei/Slow-Perception?tab=readme-ov-file)]

1. [GeoCQT] **Leveraging Two-Level Deep Learning Classifers for 2D Shape Recognition to Automatically Solve Geometry Math Word Problems**, PAA 2024 [[paper](https://link.springer.com/article/10.1007/s10044-024-01321-9)]

1. [Tangram] **Tangram: A Challenging Benchmark for Geometric Element Recognizing**, arXiv:2408.13854 [[paper](https://arxiv.org/abs/2408.13854)] [[data](https://github.com/hyper-z/tangram)]

1. [CurveML] **CurveML: A Benchmark for Evaluating and Training Learning-Based Methods of Classification, Recognition, and Fitting of Plane Curves**, Visual Comput 2024 [[paper](https://link.springer.com/article/10.1007/s00371-024-03292-8)] [[data](https://gitlab.com/4ndr3aR/CurveML)]

1. [ElementaryCQT] **ElementaryCQT: A New Dataset and Its Deep Learning Analysis for 2D Geometric Shape Recognition**, SN Comput. Sci. 2025 [[paper](https://link.springer.com/article/10.1007/s42979-024-03521-w)] [[data](https://data.mendeley.com/datasets/d35tjjgjnx/1)]

1. [SynthGeo228K/formalgeo-structure774k] **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)] [[data](https://huggingface.co/datasets/JO-KU/SynthGeo228K)]

### Geometry Problem Understanding

### Geometric Diagram Understanding

1. [Geoclidean] **Geoclidean: Few-Shot Generalization in Euclidean Geometry**, NeurIPS 2022 [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/feb34ce77fc8b94c85d12e608b23ce67-Abstract-Datasets_and_Benchmarks.html)] [[data](https://downloads.cs.stanford.edu/viscam/Geoclidean/geoclidean.zip)]

1. [Geoperception] **Euclid: Supercharging Multimodal LLMs With Synthetic High-Fidelity Visual Descriptions**, arXiv:2412.08737 [[paper](https://arxiv.org/abs/2412.08737)] [[data](https://euclid-multimodal.github.io/)]

1. [GePBench] **GePBench: Evaluating Fundamental Geometric Perception for Multimodal Large Language Models**, arXiv:2412.21036 [[paper](https://arxiv.org/abs/2412.21036)]

1. [GeomRel] **Do Large Language Models Truly Understand Geometric Structures?**, ICLR 2025 [[paper](https://openreview.net/forum?id=FjQOXenaXK)] [[data](https://github.com/banyedy/GeomRel)]

1. **Improving Multimodal LLMs Ability In Geometry Problem Solving, Reasoning, And Multistep Scoring**, arXiv:2412.00846 [[paper](https://arxiv.org/abs/2412.00846)]

1. **Advancing Multimodal LLMs: A Focus on Geometry Problem Solving Reasoning and Sequential Scoring**, MMASIA 2024 [[paper](https://dl.acm.org/doi/full/10.1145/3696409.3700262)]

1. [Geo170K-alignment] **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**, ICLR 2025 [[paper](https://openreview.net/forum?id=px1674Wp3C&noteId=H99kD23um8)] [[data](https://huggingface.co/datasets/Luckyjhg/Geo170K/tree/main)]

1. **GOLD: Geometry Problem Solver With Natural Language Description**, Findings of NAACL 2024 [[paper](https://aclanthology.org/2024.findings-naacl.19/)]

1. [AutoGeo-100k] **AutoGeo: Automating Geometric Image Dataset Creation for Enhanced Geometry Understanding**, IEEE Trans. Multimedia 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10960701/)] [[data](https://autogeo-official.github.io/)]

1. [VGPR] **GeoDANO: Geometric VLM with Domain Agnostic Vision Encoder**, arXiv:2502.11360 [[paper](https://arxiv.org/abs/2502.11360)]

1. [SynthGeo228K/formalgeo-structure774k] **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)] [[data](https://huggingface.co/datasets/JO-KU/SynthGeo228K)]

1. [GeoX-alignment] **GeoX: Geometric Problem Solving Through Unified Formalized Vision-Language Pre-Training**, ICLR 2025 [[paper](https://openreview.net/forum?id=6RiBl5sCDF)] [[data](https://huggingface.co/datasets/U4R/GeoX-data)]

### Geometric Relation Extraction

1. **Diagram Understanding in Geometry Questions**, AAAI 2014 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/9146)] :x:

1. [GeoE100/GeoC50] **Understanding Plane Geometry Problems by Integrating Relations Extracted from Text and Diagram**, PSIVT 2017 [[paper](https://link.springer.com/chapter/10.1007/978-3-319-75786-5_30)] :x:

1. **Understanding Explicit Arithmetic Word Problems and Explicit Plane Geometry Problems Using Syntax-Semantics Models**, IALP 2017 [[paper](https://ieeexplore.ieee.org/abstract/document/8300590)] :x:

1. **Automatic Understanding and Formalization of Natural Language Geometry Problems Using Syntax-Semantics Models**, IJICIC 2018 [[paper](https://www.researchgate.net/publication/322939354_Automatic_understanding_and_formalization_of_natural_language_geometry_problems_using_syntax-semantics_models)] :x:

1. **Automatic Understanding and Formalization of Plane Geometry Proving Problems in Natural Language: A Supervised Approach**, IJAIT 2019 [[paper](https://www.worldscientific.com/doi/abs/10.1142/S0218213019400037)] :x:

1. [GeoRE] **GeoRE: A relation extraction dataset for chinese geometry problems**, NeurIPS 2021 MATHAI4ED Workshop [[paper](https://mathai4ed.github.io/papers/papers/paper_6.pdf)] [[data](https://mathai4ed.github.io/papers/papers/paper_6_GeoRE_sample.json)]

1. **A Novel Geometry Problem Understanding Method based on Uniform Vectorized Syntax-Semantics Model**, IEIR 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/10050038)]

1. **Research on Geometry Problem Text Understanding Based on Bidirectional LSTM-CRF**, ICDH 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/9978458)]

1. **A Knowledge and Semantic Fusion Method for Automatic Geometry Problem Understanding**, Appl. Sci. 2025 [[paper](https://www.mdpi.com/2076-3417/15/7/3857)]

### Geometric Knowledge Prediction

1. **Inter-GPS: Interpretable Geometry Problem Solving with Formal Language and Symbolic Reasoning**, ACL 2021 [[paper](https://aclanthology.org/2021.acl-long.528/)]

1. **E-GPS: Explainable Geometry Problem Solving via Top-Down Solver and Bottom-Up Generator**, CVPR 2024 [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wu_E-GPS_Explainable_Geometry_Problem_Solving_via_Top-Down_Solver_and_Bottom-Up_CVPR_2024_paper.html)]

1. [GNS-260K] **GNS: Solving Plane Geometry Problems by Neural-Symbolic Reasoning with Multi-Modal LLMs**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34679)]

1. [GeoSense] **GeoSense: Evaluating Identification and Application of Geometric Principles in Multimodal Reasoning**, arXiv:2504.12597 [[paper](https://arxiv.org/abs/2504.12597)]

## Tasks and Datasets - Core Tasks

1. [UniGeo] **UniGeo: Unifying Geometry Logical Reasoning via Reformulating Mathematical Expression**, EMNLP 2022 [[paper](https://aclanthology.org/2022.emnlp-main.218/)] [[data](https://github.com/chen-judge/UniGeo)]

1. [formalgeo7k/formalgeo-imo] **FormalGeo: An Extensible Formalized Framework for Olympiad Geometric Problem Solving**, arXiv:2310.18021 [[paper](https://arxiv.org/abs/2310.18021)] [[data](https://github.com/BitSecret/formalgeo7k)] :x:

1. [GeoGPT4V-GPS] **GeoGPT4V: Towards Geometric Multi-modal Large Language Models with Geometric Image Generation**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.44/)] [[data](https://github.com/alibaba/GeoGPT4V)]

1. [GeoVQA] **GeoVQA: A Comprehensive Multimodal Geometry Dataset for Secondary Education**, MIPR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10707789)]

1. [GeoMath] **Geo-LLaVA: A Large Multi-Modal Model for Solving Geometry Math Problems With Meta In-Context Learning**, LGM3A 2024 [[paper](https://dl.acm.org/doi/10.1145/3688866.3689124)]

1. [GPSM4K] **Advancing Multimodal LLMs: A Focus on Geometry Problem Solving Reasoning and Sequential Scoring**, MMASIA 2024 [[paper](https://dl.acm.org/doi/full/10.1145/3696409.3700262)]

1. **Improving Multimodal LLMs Ability In Geometry Problem Solving, Reasoning, And Multistep Scoring**, arXiv:2412.00846 [[paper](https://arxiv.org/abs/2412.00846)]

1. **Geo-LLaVA: A Large Multi-Modal Model for Solving Geometry Math Problems with Meta In-Context Learning**, LGM3A 2024 [[paper](https://dl.acm.org/doi/10.1145/3688866.3689124)]

1. [GeoExpand/GeoSynth] **Enhancing the Geometric Problem-Solving Ability of Multimodal LLMs via Symbolic-Neural Integration**, arXiv:2504.12773 [[paper](https://arxiv.org/abs/2504.12773)] [[data](https://huggingface.co/datasets/ycpNotFound/GeoGen)]

### Geometry Theorem Proving

1. [Proving2H] **A Paradigm of Diagram Understanding in Problem Solving**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678637)] :x:

1. [IMO-AG-30] **Solving olympiad geometry without human demonstrations**, Nature 2024 [[paper](https://www.nature.com/articles/s41586-023-06747-5)] [[data](https://github.com/google-deepmind/alphageometry)]

1. **Wu’s Method Boosts Symbolic AI to Rival Silver Medalists and AlphaGeometry to Outperform Gold Medalists at IMO Geometry**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=aKRtC45gle)]

1. [MO-TG-225] **Proposing and Solving Olympiad Geometry with Guided Tree Search**, arXiv:2412.10673 [[paper](https://arxiv.org/abs/2412.10673)]

1. [IMO-AG-50] **Gold-medalist Performance in Solving Olympiad Geometry with AlphaGeometry2**, arXiv:2502.03544 [[paper](https://arxiv.org/abs/2502.03544)]

### Geometric Numerical Calculation

1. [GEOS] **Solving Geometry Problems: Combining Text and Diagram Interpretation**, EMNLP 2015 [[paper](https://aclanthology.org/D15-1171/)] [data](https://geometry.allenai.org/)] :x:

1. [GEOS++] **From Textbooks to Knowledge: A Case Study in Harvesting Axiomatic Knowledge from Textbooks to Solve Geometry Problems**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1081/)] :x:

1. [GEOS++] **Discourse in Multimedia: A Case Study in Extracting Geometry Knowledge from Textbooks**, CL 2019 [[paper](https://aclanthology.org/J19-4002/)] :x:

1. [GEOS-OS] **Learning to Solve Geometry Problems from Natural Language Demonstrations in Textbooks**, *SEM 2017 [[paper](https://aclanthology.org/S17-1029/)] :x:

1. [GeoShader] **Synthesis of Solutions for Shaded Area Geometry Problems**, FLAIRS 2017 [[paper](https://aaai.org/papers/14-flairs-2017-15416/)] :x:

1. [Geometry3K] **Inter-GPS: Interpretable Geometry Problem Solving with Formal Language and Symbolic Reasoning**, ACL 2021 [[paper](https://aclanthology.org/2021.acl-long.528/)] [[data](https://github.com/lupantech/InterGPS)]

1. [GeoQA] **GeoQA: A Geometric Question Answering Benchmark Towards Multimodal Numerical Reasoning**, Findings of ACL 2021 [[paper](https://aclanthology.org/2021.findings-acl.46)] [[data](https://github.com/chen-judge/GeoQA)]

1. [Geometry3Dcalculation] **Solving Solid Geometric Calculation Problems in Text**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678751)] :x:

1. **Solving Shaded Area Problems by Constructing Equations**, AIET 2021 [[paper](https://link.springer.com/chapter/10.1007/978-981-16-7527-0_8)] :x:

1. [GeometryQA] **Sequence to General Tree Knowledge-Guided Geometry Word Problem Solving**, ACL-IJCNLP 2021 [[paper](https://aclanthology.org/2021.acl-short.121/)] [[data](https://github.com/DoubleBite/Sequence-to-General-tree)]

1. [GeoQA+] **An Augmented Benchmark Dataset for Geometric Question Answering through Dual Parallel Text Encoding**, COLING 2022 [[paper](https://aclanthology.org/2022.coling-1.130/)] [[data](https://github.com/SCNU203/GeoQA-Plus)]

1. [BIG-bench-IG] **Beyond the Imitation Game: Quantifying and Extrapolating the Capabilities of Language Models**, TMLR 2022 [[paper](https://iris.uniroma1.it/handle/11573/1724128)] [[data](https://github.com/google/BIG-bench)] :large_blue_circle:

1. [PGPS9K] **A Multi-Modal Neural Geometric Solver with Textual Clauses Parsed from Diagram**, IJCAI 2023 [[paper](https://www.ijcai.org/proceedings/2023/0376)] [[data](https://github.com/mingliangzhang2018/PGPS-Pretraining)]

1. [Conic10K] **Conic10K: A Challenging Math Problem Understanding and Reasoning Dataset**, Findings of EMNLP 2023 [[paper](https://aclanthology.org/2023.findings-emnlp.427/)] [[data](https://github.com/whyNLP/Conic10K)]

1. [GeomVerse] **GeomVerse: A Systematic Evaluation of Large Models for Geometric Reasoning**, ICML 2024 AI4MATH Workshop [[paper](https://openreview.net/forum?id=1AUbiBrOF1)] [[data](https://storage.googleapis.com/gresearch/GeomVerseV0/GeomVerse.zip)]

1. [aug-Geo3K] **E-GPS: Explainable Geometry Problem Solving via Top-Down Solver and Bottom-Up Generator**, CVPR 2024 [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wu_E-GPS_Explainable_Geometry_Problem_Solving_via_Top-Down_Solver_and_Bottom-Up_CVPR_2024_paper.html)]

1. [GeoEval] **GeoEval: Benchmark for Evaluating LLMs and Multi-Modal Models on Geometry Problem-Solving**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.73/)] [[data](https://github.com/GeoEval/GeoEval)]

1. [GeoMM] **R-CoT: Reverse Chain-of-Thought Problem Generation for Geometric Reasoning in Large Multimodal Models**, arXiv:2410.17885 [[paper](https://arxiv.org/abs/2410.17885)]https://github.com/dle666/r-cot

1. [NBLP] **An Enhanced Relation-Flow Algorithm for Solving Number Line Problems**, IEIR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10960042)] :x:

1. [G-MATH] **BBA: Bi-Modal Behavioral Alignment for Reasoning with Large Vision-Language Models**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.433/)]

1. [Geo170K-qa] **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**, ICLR 2025 [[paper](https://openreview.net/forum?id=px1674Wp3C&noteId=H99kD23um8)] [[data](https://huggingface.co/datasets/Luckyjhg/Geo170K/tree/main)]

1. [GeoTrust] **TrustGeoGen: Scalable and Formal-Verified Data Engine for Trustworthy Multi-modal Geometric Problem Solving**, arXiv:2504.15780 [[paper](https://arxiv.org/abs/2504.15780)]

1. [FormalGeo7K-v2] **FGeo-Parser: Autoformalization and Solution of Plane Geometric Problems**, Symmetry 2025 [[paper](https://www.mdpi.com/2073-8994/17/1/8)] [[data](https://github.com/FormalGeo/FormalGeo)]

1. [VerMulti-Geo] **LMM-R1: Empowering 3B LMMs with Strong Reasoning Abilities Through Two-Stage Rule-Based RL**, arXiv:2503.07536 [[paper](https://arxiv.org/abs/2503.07536)]

1. [GeoMath-8K] **Reason-RFT: Reinforcement Fine-Tuning for Visual Reasoning**, arXiv:2503.20752 [[paper](https://arxiv.org/abs/2503.20752)] :large_blue_circle:

1. [GNS-260K] **GNS: Solving Plane Geometry Problems by Neural-Symbolic Reasoning with Multi-Modal LLMs**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34679)]

1. [GeoSense] **GeoSense: Evaluating Identification and Application of Geometric Principles in Multimodal Reasoning**, arXiv:2504.12597 [[paper](https://arxiv.org/abs/2504.12597)]

1. [formalgeo-reasoning238k] **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)]

## Tasks and Datasets - Composite Tasks

### Mathematical Reasoning

### Multimodal Perception


## Related Surveys

1. **The Gap of Semantic Parsing: A Survey on Automatic Math Word Problem Solvers**, TPAMI 2019 [[paper](https://library.oapen.org/bitstream/handle/20.500.12657/61269/978-3-031-09687-7.pdf?sequence=1#page=246)] :large_blue_circle: :x:

2. **Deep Learning in Automatic Math Word Problem Solvers**, AI in Learning: Designing the Future 2022 [[article](https://library.oapen.org/bitstream/handle/20.500.12657/61269/978-3-031-09687-7.pdf?sequence=1#page=246)] :large_blue_circle:

3. **Evolution of Automated Deduction and Dynamic Constructions in Geometry**, Mathematics Education in the Age of Artificial Intelligence: How Artificial Intelligence can Serve Mathematical Human Learning 2022 [[article](https://link.springer.com/chapter/10.1007/978-3-030-86909-0_1)] :x:

4. **A Survey of Deep Learning for Mathematical Reasoning**, ACL 2023 [[paper](https://aclanthology.org/2023.acl-long.817/)] :large_blue_circle:

5. **Systematic Literature Review: Application of Dynamic Geometry Software to Improve Mathematical Problem-Solving Skills**, Mathline: Jurnal Matematika Dan Pendidikan Matematika 2023 [[paper](https://mathline.unwir.ac.id/index.php/Mathline/article/view/458)] :x:

6. **A Survey of Reasoning with Foundation Models**, arXiv:2312.11562 [[paper](https://arxiv.org/abs/2312.11562)] :large_blue_circle:

7. **A Survey of Reasoning with Foundation Models: Concepts, Methodologies, and Outlook**, ACM Comput. Surv. 2023 [[paper](https://dl.acm.org/doi/full/10.1145/3729218)] :large_blue_circle:

8. **Adapting Large Language Models for Education: Foundational Capabilities, Potentials, and Challenges**, arXiv:2401.08664 [[paper](https://arxiv.org/abs/2401.08664)] :large_blue_circle:

9. **Large Language Models for Mathematical Reasoning: Progresses and Challenges**, EACL 2024 [[paper](https://aclanthology.org/2024.eacl-srw.17/)] :large_blue_circle:

10. **A Survey on Deep Learning for Theorem Proving**, COLM 2024 [[paper](https://openreview.net/forum?id=zlw6AHwukB)] :large_blue_circle:

11. **A Comprehensive Survey of Scientific Large Language Models and Their Applications in Scientific Discovery**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.498/)] :large_blue_circle:

12. **Towards Robust Automated Math Problem Solving: A Survey of Statistical and Deep Learning Approaches**, Evol. Intell. 2024 [[paper](https://link.springer.com/article/10.1007/s12065-024-00957-0)] :large_blue_circle:

13. **A Survey of Mathematical Reasoning in the Era of Multimodal Large Language Model: Benchmark, Method & Challenges**, Findings of ACL 2025 [[paper](https://arxiv.org/abs/2412.11936)] :large_blue_circle:

14. **Decoding Math: A Review of Datasets Shaping AI-Driven Mathematical Reasoning**, JIM 2025 [[paper](https://www.tarupublications.com/doi/10.47974/JIM-2105)] :large_blue_circle:

15. **Visual Large Language Models for Generalized and Specialized Application**, arXiv:2501.02765 [[paper](https://arxiv.org/abs/2501.02765)] :large_blue_circle:

16. **From System 1 to System 2: A Survey of Reasoning Large Language Models**, arXiv:2502.17419 [[paper](https://arxiv.org/abs/2502.17419)] :large_blue_circle:

17. **Towards Scientific Intelligence: A Survey of LLM-based Scientific Agents**, arXiv:2503.24047 [[paper](https://arxiv.org/abs/2503.24047)] :large_blue_circle:



