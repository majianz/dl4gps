# Deep Learning for Geometry Problem Solving (DL4GPS)

[![Awesome](https://awesome.re/badge.svg)](https://github.com/majianz/gps-survey) 
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![Survey](https://img.shields.io/badge/Survey-DL4GPS-blue)](https://github.com/majianz/gps-survey) 

This repository is the reading list on ***A Survey of Deep Learning for Geometry Problem Solving (DL4GPS)***. We will update the papers after a certain period of time. The current deadline for included papers is **April 2025**.

- :large_blue_circle: indicates that the work is not specifically designed for geometry problems.

- :small_red_triangle: represents geometry tasks other than geometry problem solving.

- :x: indicates no deep learning method is used.

:bell: If you have any suggestions or notice something we missed, please don't hesitate to let us know. You can directly email Jianzhe Ma (majianzhe@ruc.edu.cn), or post an issue on this repo.

## Table of Contents

- [Surveys](#surveys)
- [Tasks and Datasets - Fundamental Tasks](#tasks-and-datasets---fundamental-tasks)
    - [Geometry Diagram Understanding](#geometry-diagram-understanding)
    - [Semantic Parsing for Geometry Problem](#semantic-parsing-for-geometry-problem)
    - [Geometric Relation Extraction](#geometric-relation-extraction)
    - [Geometric Knowledge Prediction](#geometric-knowledge-prediction)
- [Tasks and Datasets - Core Tasks](#tasks-and-datasets---core-tasks)
    - [Geometry Theorem Proving](#geometry-theorem-proving)
    - [Geometric Numerical Calculation](#geometric-numerical-calculation)
- [Tasks and Datasets - Composite Tasks](#tasks-and-datasets---composite-tasks)
    - [Mathematical Reasoning](#mathematical-reasoning)
- [Tasks and Datasets - Other Geometry Tasks](#tasks-and-datasets---other-geometry-tasks)
    - [Geometric Diagram Generation](#geometric-diagram-generation)
    - [Geometric Construction Problem](#geometric-construction-problem)
    - [Geometric Figure Retrieval](#geometric-figure-retrieval)
    - [Geometric Autoformalization](#geometric-autoformalization)
- [Methods - Architectures](#methods---architectures)
    - [Encoder-Decoder](#encoder-decoder)
    - [Other Architectures](#other-architectures)
- [Methods - Training Stage](#methods---training-stage)
    - [Pre-Training](#pre-training)
    - [Supervised Fine-Tuning](#supervised-fine-tuning)
    - [Reinforcement Learning](#reinforcement-learning)
- [Methods - Inference Stage](#methods---inference-stage)
    - [Test-Time Scaling](#test-time-scaling)
    - [Knowledge-Augmented Inference](#knowledge-augmented-inference)
- [Related Surveys](#related-surveys)
- [Years](#years)
    - [2014](#2014)
    - [2015](#2015)
    - [2016](#2016)
    - [2017](#2017)
    - [2018](#2018)
    - [2019](#2019)
    - [2020](#2020)
    - [2021](#2021)
    - [2022](#2022)
    - [2023](#2023)
    - [2024](#2024)
    - [2025](#2025)
- [Citation](#citation)

## Surveys

- **Plane Geometry Problem Solving with Multi-modal Reasoning: A Survey**, arXiv:2505.14340 [[paper](https://arxiv.org/abs/2505.14340)]
- **Towards Geometry Problem Solving in the Large Model Era: A Survey**, arXiv:2506.02690 [[paper](https://arxiv.org/abs/2506.02690)]

## Tasks and Datasets - Fundamental Tasks

### Geometry Diagram Understanding

- **2D Geometric Shapes Dataset – For Machine Learning and Pattern Recognition**, Data in Brief 2020 [[paper](https://www.sciencedirect.com/science/article/pii/S2352340920309847)] [[2Dgeometricshapes data](https://data.mendeley.com/datasets/wzr2yv7r53/1)]
- **Geoclidean: Few-Shot Generalization in Euclidean Geometry**, NeurIPS 2022 [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/feb34ce77fc8b94c85d12e608b23ce67-Abstract-Datasets_and_Benchmarks.html)] [[Geoclidean data](https://downloads.cs.stanford.edu/viscam/Geoclidean/geoclidean.zip)]
- **Euclid: Supercharging Multimodal LLMs With Synthetic High-Fidelity Visual Descriptions**, arXiv:2412.08737 [[paper](https://arxiv.org/abs/2412.08737)] [[Geoperception data](https://euclid-multimodal.github.io/)]
- **GePBench: Evaluating Fundamental Geometric Perception for Multimodal Large Language Models**, arXiv:2412.21036 [[paper](https://arxiv.org/abs/2412.21036)] [GePBench data]
- **Do Large Language Models Truly Understand Geometric Structures?**, ICLR 2025 [[paper](https://openreview.net/forum?id=FjQOXenaXK)] [[GeomRel data](https://github.com/banyedy/GeomRel)]
- **Improving Multimodal LLMs Ability In Geometry Problem Solving, Reasoning, And Multistep Scoring**, arXiv:2412.00846 [[paper](https://arxiv.org/abs/2412.00846)]
- **Advancing Multimodal LLMs: A Focus on Geometry Problem Solving Reasoning and Sequential Scoring**, MMASIA 2024 [[paper](https://dl.acm.org/doi/full/10.1145/3696409.3700262)]
- **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**, ICLR 2025 [[paper](https://openreview.net/forum?id=px1674Wp3C&noteId=H99kD23um8)] [[Geo170K-alignment data](https://huggingface.co/datasets/Luckyjhg/Geo170K/tree/main)]
- **GOLD: Geometry Problem Solver With Natural Language Description**, Findings of NAACL 2024 [[paper](https://aclanthology.org/2024.findings-naacl.19/)]
- **AutoGeo: Automating Geometric Image Dataset Creation for Enhanced Geometry Understanding**, IEEE Trans. Multimedia 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10960701/)] [[AutoGeo-100k data](https://autogeo-official.github.io/)]
- **GeoDANO: Geometric VLM with Domain Agnostic Vision Encoder**, arXiv:2502.11360 [[paper](https://arxiv.org/abs/2502.11360)] [VGPR data]
- **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)] [[SynthGeo228K/formalgeo-structure774k data](https://huggingface.co/datasets/JO-KU/SynthGeo228K)]
- **GeoX: Geometric Problem Solving Through Unified Formalized Vision-Language Pre-Training**, ICLR 2025 [[paper](https://openreview.net/forum?id=6RiBl5sCDF)] [[GeoX-alignment data](https://huggingface.co/datasets/U4R/GeoX-data)]
- **Decomposing Complex Visual Comprehension Into Atomic Visual Skills for Vision Language Models**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=nFU4xCyoe0)] [[AVSBench data](https://github.com/Atomic-Visual-Skills/AVS)] :large_blue_circle:
- **VisOnlyQA: Large Vision Language Models Still Struggle With Visual Perception of Geometric Information**, arXiv:2412.00947 [[paper](https://arxiv.org/abs/2412.00947)] [[VisOnlyQA data](https://github.com/psunlpgroup/VisOnlyQA)] :large_blue_circle:
- **VisNumBench: Evaluating Number Sense of Multimodal Large Language Models**, arXiv:2503.14939 [[paper](https://arxiv.org/abs/2503.14939)] [[VisNumBench data](https://huggingface.co/datasets/GML-FMGroup/VisNumBench)] :large_blue_circle:
- **MATHGLANCE: Multimodal Large Language Models Do Not Know Where to Look in Mathematical Diagrams**, arXiv:2503.20745 [[paper](https://arxiv.org/abs/2503.20745)] [[MATHGLANCE/GeoPeP data](https://mathglance.github.io/)]
- **Why Vision Language Models Struggle with Visual Arithmetic? Towards Enhanced Chart and Geometry Understanding**, Findings of ACL 2025 [[paper](https://arxiv.org/abs/2502.11492)] [[CogAlign-Probing/CogAlign-train data](https://huggingface.co/datasets/Salesforce/CogAlign)]
- **Retrieving Geometric Information from Images: The Case of Hand-Drawn Diagrams**, KDD 2017 [[paper](https://link.springer.com/article/10.1007/s10618-017-0494-1)] :x:
- **A Novel Geometric Information Retrieval Tool for Images of Geometric Diagrams**, ICISE-IE 2020 [[paper](https://ieeexplore.ieee.org/abstract/document/9418805)]
- **A Paradigm of Diagram Understanding in Problem Solving**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678637)] :x:
- **Plane Geometry Diagram Parsing**, IJCAI 2022 [[paper](https://www.ijcai.org/proceedings/2022/228)] [[PGDP5K data](https://github.com/mingliangzhang2018/PGDP)]
- **Learning to Understand Plane Geometry Diagram**, NeurIPS 2022 MATH-AI Workshop [[paper](https://mathai2022.github.io/papers/6.pdf)] [[PGDP5K data](https://github.com/mingliangzhang2018/PGDP)]
- **PGDP5K: A Diagram Parsing Dataset for Plane Geometry Problems**, ICPR 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/9956397)] [[PGDP5K data](https://github.com/mingliangzhang2018/PGDP)]
- **Usage of Stacked Long Short-Term Memory for Recognition of 3D Analytic Geometry Elements**, ICAART 2022 [[paper](https://www.scitepress.org/Papers/2022/108989/108989.pdf)]
- **Solving Algebraic Problems with Geometry Diagrams Using Syntax-Semantics Diagram Understanding**, Computers, Materials & Continua 2023 [[paper](https://www.researchgate.net/profile/Litian-Huang/publication/375217917_Solving_Algebraic_Problems_with_Geometry_Diagrams_Using_Syntax-Semantics_Diagram_Understanding/links/654715da3fa26f66f4d60625/Solving-Algebraic-Problems-with-Geometry-Diagrams-Using-Syntax-Semantics-Diagram-Understanding.pdf)] :x:
- **Challenging BIG-Bench Tasks and Whether Chain-of-Thought Can Solve Them**, Findings of ACL 2023 [[paper](https://aclanthology.org/2023.findings-acl.824/)] [[BBH-geometricshapes data](https://huggingface.co/datasets/Joschka/big_bench_hard)]
- **2D Shape Detection for Solving Geometry Word Problems**, IETE J. Res. 2024 [[paper](https://www.tandfonline.com/doi/abs/10.1080/03772063.2023.2274914)] :x:
- **Slow Perception: Let's Perceive Geometric Figures Step-by-Step**, arXiv:2412.20631 [[paper](https://arxiv.org/abs/2412.20631)] [[SP-1 data](https://github.com/Ucas-HaoranWei/Slow-Perception?tab=readme-ov-file)]
- **Leveraging Two-Level Deep Learning Classifers for 2D Shape Recognition to Automatically Solve Geometry Math Word Problems**, PAA 2024 [[paper](https://link.springer.com/article/10.1007/s10044-024-01321-9)] [GeoCQT data]
- **Tangram: A Challenging Benchmark for Geometric Element Recognizing**, arXiv:2408.13854 [[paper](https://arxiv.org/abs/2408.13854)] [[Tangram data](https://github.com/hyper-z/tangram)]
- **CurveML: A Benchmark for Evaluating and Training Learning-Based Methods of Classification, Recognition, and Fitting of Plane Curves**, Visual Comput 2024 [[paper](https://link.springer.com/article/10.1007/s00371-024-03292-8)] [[CurveML data](https://gitlab.com/4ndr3aR/CurveML)]
- **ElementaryCQT: A New Dataset and Its Deep Learning Analysis for 2D Geometric Shape Recognition**, SN Comput. Sci. 2025 [[paper](https://link.springer.com/article/10.1007/s42979-024-03521-w)] [[ElementaryCQT data](https://data.mendeley.com/datasets/d35tjjgjnx/1)]
- **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)] [[SynthGeo228K/formalgeo-structure774k data](https://huggingface.co/datasets/JO-KU/SynthGeo228K)]

### Semantic Parsing for Geometry Problem

- **Semantic Parsing of Pre-University Math Problems**, ACL 2017 [[paper](https://aclanthology.org/P17-1195/)] :x:
- **Beyond Sentential Semantic Parsing: Tackling the Math SAT with a Cascade of Tree Transducers**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1083/)] :large_blue_circle: :x:
- **From Textbooks to Knowledge: A Case Study in Harvesting Axiomatic Knowledge from Textbooks to Solve Geometry Problems**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1081/)] :x:
- **Discourse in Multimedia: A Case Study in Extracting Geometry Knowledge from Textbooks**, CL 2019 [[paper](https://aclanthology.org/J19-4002/)] :x:
- **Extending a Parser to Distant Domains Using a Few Dozen Partially Annotated Examples**, ACL 2018 [[paper](https://aclanthology.org/P18-1110/)]
- **A Neural Semantic Parser for Math Problems Incorporating Multi-Sentence Information**, TALLIP 2019 [[paper](https://dl.acm.org/doi/abs/10.1145/3314939)] :large_blue_circle:
- **Two-step memory networks for deep semantic parsing of geometry word problems**, SOFSEM 2020 [[paper](https://dl.acm.org/doi/abs/10.1007/978-3-030-38919-2_57)]
- **Semantic parsing of geometry statements using supervised machine learning on Synthetic Data**, NatFoM 2021 CICM Workshop [[paper](https://hal.science/hal-03327994/document)]
- **Cognitive Patterns for Semantic Presentation of Natural-Language Descriptions of Well-Formalizable Problems**, RCAI 2021 [[paper](https://link.springer.com/chapter/10.1007/978-3-030-86855-0_22)] :x:
- **Exploration of Formalization Techniques for Geometric Entities in Planar Geometry Proposition Texts**, JAIP 2025 [[paper](https://www.clausiuspress.com/assets/default/article/2025/02/27/article_1740641608.pdf)]
- **Extracting structured information from the textual description of geometry word problems**, NLPIR 2023 [[paper](https://dl.acm.org/doi/abs/10.1145/3639233.3639255)] :x:
- **Automatic Extraction of Structured Information from Elementary Level Geometry Questions into Logic Forms**, Multimed Tools Appl 2024 [[paper](https://link.springer.com/article/10.1007/s11042-024-20463-w)] [ElementaryGeometryQA data]
- **Evaluating Automated Geometric Problem Solving With Formal Language Generation on Large Multimodal Models**, IEIR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10959992)]
- **FGeo-Parser: Autoformalization and Solution of Plane Geometric Problems**, Symmetry 2025 [[paper](https://www.mdpi.com/2073-8994/17/1/8)]

### Geometric Relation Extraction

- **Diagram Understanding in Geometry Questions**, AAAI 2014 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/9146)] :x:
- **Understanding Plane Geometry Problems by Integrating Relations Extracted from Text and Diagram**, PSIVT 2017 [[paper](https://link.springer.com/chapter/10.1007/978-3-319-75786-5_30)] [GeoC50 data] :x:
- **Understanding Explicit Arithmetic Word Problems and Explicit Plane Geometry Problems Using Syntax-Semantics Models**, IALP 2017 [[paper](https://ieeexplore.ieee.org/abstract/document/8300590)] :x:
- **Automatic Understanding and Formalization of Natural Language Geometry Problems Using Syntax-Semantics Models**, IJICIC 2018 [[paper](https://www.researchgate.net/publication/322939354_Automatic_understanding_and_formalization_of_natural_language_geometry_problems_using_syntax-semantics_models)] :x:
- **Automatic Understanding and Formalization of Plane Geometry Proving Problems in Natural Language: A Supervised Approach**, IJAIT 2019 [[paper](https://www.worldscientific.com/doi/abs/10.1142/S0218213019400037)] :x:
- **GeoRE: A relation extraction dataset for chinese geometry problems**, NeurIPS 2021 MATHAI4ED Workshop [[paper](https://mathai4ed.github.io/papers/papers/paper_6.pdf)] [[GeoRE data](https://mathai4ed.github.io/papers/papers/paper_6_GeoRE_sample.json)]
- **A Novel Geometry Problem Understanding Method based on Uniform Vectorized Syntax-Semantics Model**, IEIR 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/10050038)]
- **Research on Geometry Problem Text Understanding Based on Bidirectional LSTM-CRF**, ICDH 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/9978458)]
- **A Knowledge and Semantic Fusion Method for Automatic Geometry Problem Understanding**, Appl. Sci. 2025 [[paper](https://www.mdpi.com/2076-3417/15/7/3857)]

### Geometric Knowledge Prediction

- **Inter-GPS: Interpretable Geometry Problem Solving with Formal Language and Symbolic Reasoning**, ACL 2021 [[paper](https://aclanthology.org/2021.acl-long.528/)]
- **E-GPS: Explainable Geometry Problem Solving via Top-Down Solver and Bottom-Up Generator**, CVPR 2024 [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wu_E-GPS_Explainable_Geometry_Problem_Solving_via_Top-Down_Solver_and_Bottom-Up_CVPR_2024_paper.html)]
- **GNS: Solving Plane Geometry Problems by Neural-Symbolic Reasoning with Multi-Modal LLMs**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34679)] [GNS-260K data]
- **GeoSense: Evaluating Identification and Application of Geometric Principles in Multimodal Reasoning**, arXiv:2504.12597 [[paper](https://arxiv.org/abs/2504.12597)] [GeoSense data]

## Tasks and Datasets - Core Tasks

- **UniGeo: Unifying Geometry Logical Reasoning via Reformulating Mathematical Expression**, EMNLP 2022 [[paper](https://aclanthology.org/2022.emnlp-main.218/)] [[UniGeo data](https://github.com/chen-judge/UniGeo)]
- **FormalGeo: An Extensible Formalized Framework for Olympiad Geometric Problem Solving**, arXiv:2310.18021 [[paper](https://arxiv.org/abs/2310.18021)] [[formalgeo7k/formalgeo-imo data](https://github.com/BitSecret/formalgeo7k)] :x:
- **GeoGPT4V: Towards Geometric Multi-modal Large Language Models with Geometric Image Generation**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.44/)] [[GeoGPT4V-GPS data](https://github.com/alibaba/GeoGPT4V)]
- **GeoVQA: A Comprehensive Multimodal Geometry Dataset for Secondary Education**, MIPR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10707789)] [GeoVQA data]
- **Geo-LLaVA: A Large Multi-Modal Model for Solving Geometry Math Problems With Meta In-Context Learning**, LGM3A 2024 [[paper](https://dl.acm.org/doi/10.1145/3688866.3689124)] [GeoMath data]
- **Advancing Multimodal LLMs: A Focus on Geometry Problem Solving Reasoning and Sequential Scoring**, MMASIA 2024 [[paper](https://dl.acm.org/doi/full/10.1145/3696409.3700262)] [GPSM4K data]
- **Improving Multimodal LLMs Ability In Geometry Problem Solving, Reasoning, And Multistep Scoring**, arXiv:2412.00846 [[paper](https://arxiv.org/abs/2412.00846)] [GPSM4K data]
- **Geo-LLaVA: A Large Multi-Modal Model for Solving Geometry Math Problems with Meta In-Context Learning**, LGM3A 2024 [[paper](https://dl.acm.org/doi/10.1145/3688866.3689124)] [GeoMath data]
- **Enhancing the Geometric Problem-Solving Ability of Multimodal LLMs via Symbolic-Neural Integration**, arXiv:2504.12773 [[paper](https://arxiv.org/abs/2504.12773)] [[GeoExpand/GeoSynth data](https://huggingface.co/datasets/ycpNotFound/GeoGen)]

### Geometry Theorem Proving

- **A Paradigm of Diagram Understanding in Problem Solving**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678637)] [Proving2H data] :x:
- **Solving Olympiad Geometry Without Human Demonstrations**, Nature 2024 [[paper](https://www.nature.com/articles/s41586-023-06747-5)] [[IMO-AG-30 data](https://github.com/google-deepmind/alphageometry)]
- **Wu’s Method Boosts Symbolic AI to Rival Silver Medalists and AlphaGeometry to Outperform Gold Medalists at IMO Geometry**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=aKRtC45gle)]
- **Proposing and Solving Olympiad Geometry with Guided Tree Search**, arXiv:2412.10673 [[paper](https://arxiv.org/abs/2412.10673)] [MO-TG-225 data]
- **Gold-medalist Performance in Solving Olympiad Geometry with AlphaGeometry2**, arXiv:2502.03544 [[paper](https://arxiv.org/abs/2502.03544)] [IMO-AG-50 data]

### Geometric Numerical Calculation

- **Solving Geometry Problems: Combining Text and Diagram Interpretation**, EMNLP 2015 [[paper](https://aclanthology.org/D15-1171/)] [GEOS data](https://geometry.allenai.org/)] :x:
- **From Textbooks to Knowledge: A Case Study in Harvesting Axiomatic Knowledge from Textbooks to Solve Geometry Problems**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1081/)] [GEOS++ data] :x:
- **Discourse in Multimedia: A Case Study in Extracting Geometry Knowledge from Textbooks**, CL 2019 [[paper](https://aclanthology.org/J19-4002/)] [GEOS++ data] :x:
- **Learning to Solve Geometry Problems from Natural Language Demonstrations in Textbooks**, *SEM 2017 [[paper](https://aclanthology.org/S17-1029/)] [GEOS-OS] :x:
- **Synthesis of Solutions for Shaded Area Geometry Problems**, FLAIRS 2017 [[paper](https://aaai.org/papers/14-flairs-2017-15416/)] [GeoShader data] :x:
- **Inter-GPS: Interpretable Geometry Problem Solving with Formal Language and Symbolic Reasoning**, ACL 2021 [[paper](https://aclanthology.org/2021.acl-long.528/)] [[Geometry3K data](https://github.com/lupantech/InterGPS)]
- **GeoQA: A Geometric Question Answering Benchmark Towards Multimodal Numerical Reasoning**, Findings of ACL 2021 [[paper](https://aclanthology.org/2021.findings-acl.46)] [[GeoQA data](https://github.com/chen-judge/GeoQA)]
- **Solving Solid Geometric Calculation Problems in Text**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678751)] [Geometry3Dcalculation data] :x:
- **Solving Shaded Area Problems by Constructing Equations**, AIET 2021 [[paper](https://link.springer.com/chapter/10.1007/978-981-16-7527-0_8)] :x:
- **Sequence to General Tree Knowledge-Guided Geometry Word Problem Solving**, ACL-IJCNLP 2021 [[paper](https://aclanthology.org/2021.acl-short.121/)] [[GeometryQA data](https://github.com/DoubleBite/Sequence-to-General-tree)]
- **An Augmented Benchmark Dataset for Geometric Question Answering through Dual Parallel Text Encoding**, COLING 2022 [[paper](https://aclanthology.org/2022.coling-1.130/)] [[GeoQA+ data](https://github.com/SCNU203/GeoQA-Plus)]
- **Beyond the Imitation Game: Quantifying and Extrapolating the Capabilities of Language Models**, TMLR 2022 [[paper](https://iris.uniroma1.it/handle/11573/1724128)] [[BIG-bench-IG data](https://github.com/google/BIG-bench)] :large_blue_circle:
- **A Multi-Modal Neural Geometric Solver with Textual Clauses Parsed from Diagram**, IJCAI 2023 [[paper](https://www.ijcai.org/proceedings/2023/0376)] [[PGPS9K data](https://github.com/mingliangzhang2018/PGPS-Pretraining)]
- **Conic10K: A Challenging Math Problem Understanding and Reasoning Dataset**, Findings of EMNLP 2023 [[paper](https://aclanthology.org/2023.findings-emnlp.427/)] [[Conic10K data](https://github.com/whyNLP/Conic10K)]
- **GeomVerse: A Systematic Evaluation of Large Models for Geometric Reasoning**, ICML 2024 AI4MATH Workshop [[paper](https://openreview.net/forum?id=1AUbiBrOF1)] [[GeomVerse data](https://storage.googleapis.com/gresearch/GeomVerseV0/GeomVerse.zip)]
- **E-GPS: Explainable Geometry Problem Solving via Top-Down Solver and Bottom-Up Generator**, CVPR 2024 [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wu_E-GPS_Explainable_Geometry_Problem_Solving_via_Top-Down_Solver_and_Bottom-Up_CVPR_2024_paper.html)] [aug-Geo3K data]
- **GeoEval: Benchmark for Evaluating LLMs and Multi-Modal Models on Geometry Problem-Solving**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.73/)] [[GeoEval data](https://github.com/GeoEval/GeoEval)]
- **R-CoT: Reverse Chain-of-Thought Problem Generation for Geometric Reasoning in Large Multimodal Models**, arXiv:2410.17885 [[paper](https://arxiv.org/abs/2410.17885)] [[GeoMM data](https://github.com/dle666/r-cot)]
- **An Enhanced Relation-Flow Algorithm for Solving Number Line Problems**, IEIR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10960042)] [NBLP data] :x:
- **BBA: Bi-Modal Behavioral Alignment for Reasoning with Large Vision-Language Models**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.433/)] [G-MATH data]
- **Is Your Model Really a Good Math Reasoner? Evaluating Mathematical Reasoning With Checklist**, arXiv:2407.08733 [[paper](https://arxiv.org/abs/2407.08733)] [[MATHCHECK-GEO data](https://huggingface.co/datasets/PremiLab-Math/MathCheck)]
- **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**, ICLR 2025 [[paper](https://openreview.net/forum?id=px1674Wp3C&noteId=H99kD23um8)] [[ Geo170K-qadata](https://huggingface.co/datasets/Luckyjhg/Geo170K/tree/main)]
- **TrustGeoGen: Scalable and Formal-Verified Data Engine for Trustworthy Multi-modal Geometric Problem Solving**, arXiv:2504.15780 [[paper](https://arxiv.org/abs/2504.15780)] [GeoTrust data]
- **FGeo-Parser: Autoformalization and Solution of Plane Geometric Problems**, Symmetry 2025 [[paper](https://www.mdpi.com/2073-8994/17/1/8)] [[FormalGeo7K-v2 data](https://github.com/FormalGeo/FormalGeo)]
- **LMM-R1: Empowering 3B LMMs with Strong Reasoning Abilities Through Two-Stage Rule-Based RL**, arXiv:2503.07536 [[paper](https://arxiv.org/abs/2503.07536)] [VerMulti-Geo data]
- **Reason-RFT: Reinforcement Fine-Tuning for Visual Reasoning**, arXiv:2503.20752 [[paper](https://arxiv.org/abs/2503.20752)] [GeoMath-8K data] :large_blue_circle:
- **GNS: Solving Plane Geometry Problems by Neural-Symbolic Reasoning with Multi-Modal LLMs**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34679)] [GNS-260K data]
- **GeoSense: Evaluating Identification and Application of Geometric Principles in Multimodal Reasoning**, arXiv:2504.12597 [[paper](https://arxiv.org/abs/2504.12597)] [GeoSense data]
- **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)] [formalgeo-reasoning238k data]

## Tasks and Datasets - Composite Tasks

### Mathematical Reasoning

- **Measuring Mathematical Problem Solving With the MATH Dataset**, NeurIPS 2021 [[paper](https://datasets-benchmarks-proceedings.neurips.cc/paper_files/paper/2021/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper-round2.pdf)] [[MATH/AMPS data](https://github.com/hendrycks/math)] :large_blue_circle:
- **NUMGLUE: A Suite of Fundamental yet Challenging Mathematical Reasoning Tasks**, ACL 2022 [[paper](https://aclanthology.org/2022.acl-long.246/)] [[NUMGLUE data](https://github.com/allenai/numglue)] :large_blue_circle:
- **Lila: A Unified Benchmark for Mathematical Reasoning**, EMNLP 2022 [[paper](https://aclanthology.org/2022.emnlp-main.392/)] [[Lila data](https://huggingface.co/datasets/allenai/lila)] :large_blue_circle:
- **It Ain’t Over: A Multi-Aspect Diverse Math Word Problem Dataset**, EMNLP 2023 [[paper](https://aclanthology.org/2023.emnlp-main.927/)] [[DMath data](https://github.com/JiwooKimAR/dmath)] :large_blue_circle:
- **TheoremQA: A Theorem-driven Question Answering Dataset**, EMNLP 2023 [[paper](https://aclanthology.org/2023.emnlp-main.489/)] [[TheoremQA data](https://huggingface.co/datasets/TIGER-Lab/TheoremQA)] :large_blue_circle:
- **M3exam: A multilingual, multimodal, multilevel benchmark for examining large language models**, NeurIPS 2023 [[paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/117c5c8622b0d539f74f6d1fb082a2e9-Abstract-Datasets_and_Benchmarks.html)] [[M3Exam data](https://github.com/DAMO-NLP-SG/M3Exam)] :large_blue_circle:
- **OlympiadBench: A Challenging Benchmark for Promoting AGI With Olympiad-Level Bilingual Multimodal Scientific Problems**, ACL 2024 [[paper](https://aclanthology.org/2024.acl-long.211/)] [[OlympiadBench data](https://github.com/OpenBMB/OlympiadBench)] :large_blue_circle:
- **MathVista: Evaluating Mathematical Reasoning of Foundation Models in Visual Contexts**, ICLR 2024 [[paper](https://iclr.cc/virtual/2024/oral/19768)] [[MathVista data](https://huggingface.co/datasets/AI4Math/MathVista)] :large_blue_circle:
- **MathVerse: Does Your Multi-Modal LLM Truly See the Diagrams in Visual Math Problems?**, ECCV 2024 [[paper](https://dl.acm.org/doi/10.1007/978-3-031-73242-3_10)] [[MathVerse data](https://huggingface.co/datasets/AI4Math/MathVerse)] :large_blue_circle:
- **Measuring Multimodal Mathematical Reasoning With MATH-Vision Dataset**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/ad0edc7d5fa1a783f063646968b7315b-Abstract-Datasets_and_Benchmarks_Track.html)] [[MATH-Vision data](https://github.com/mathllm/MATH-V)] :large_blue_circle:
- **MM-MATH: Advancing Multimodal Math Evaluation With Process Evaluation and Fine-Grained Classification**, Findings of EMNLP 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.73/)] [[MM-MATH data](https://huggingface.co/datasets/THU-KEG/MM_Math)] :large_blue_circle:
- **We-Math: Does Your Large Multimodal Model Achieve Human-Like Mathematical Reasoning?**, arXiv:2407.01284 [[paper](https://arxiv.org/abs/2407.01284)] [[We-Math data](https://huggingface.co/datasets/We-Math/We-Math)] :large_blue_circle:
- **VisAidMath: Benchmarking Visual-Aided Mathematical Reasoning**, arXiv:2410.22995 [[paper](https://arxiv.org/abs/2410.22995)] [VisAidMath data] :large_blue_circle:
- **CMM-Math: A Chinese Multimodal Math Dataset to Evaluate and Enhance the Mathematics Reasoning of Large Multimodal Models**, arXiv:2409.02834 [[paper](https://arxiv.org/abs/2409.02834)] [[CMM-Math data](https://huggingface.co/datasets/ecnu-icalk/cmm-math)] :large_blue_circle:
- **MathScape: Evaluating MLLMs in Multimodal Math Scenarios Through a Hierarchical Benchmark**, arXiv:2408.07543 [[paper](https://arxiv.org/abs/2408.07543)] [[MathScape data](https://github.com/PKU-Baichuan-MLSystemLab/MathScape)] :large_blue_circle:
- **VisScience: An Extensive Benchmark for Evaluating K12 Educational Multi-Modal Scientific Reasoning**, arXiv:2409.13730 [[paper](https://arxiv.org/abs/2409.13730)] [VisScience data] :large_blue_circle:
- **Multimodal ArXiv: A Dataset for Improving Scientific Comprehension of Large Vision-Language Models**, ACL 2024 [[paper](https://aclanthology.org/2024.acl-long.775/)] [[ArXivQA data](https://huggingface.co/datasets/openbmb/VisRAG-Ret-Test-ArxivQA)] :large_blue_circle:
- **ReMI: A Dataset for Reasoning With Multiple Images**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/6ea56c0baacac9f7764257a43a93c90a-Abstract-Datasets_and_Benchmarks_Track.html)] [[ReMI data](https://huggingface.co/datasets/mehrankazemi/ReMI)] :large_blue_circle:
- **Math-LLaVA: Bootstrapping Mathematical Reasoning for Multimodal Large Language Models**, EMNLP Findings 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.268/)] [[MathV360K data](https://huggingface.co/datasets/Zhiqiang007/MathV360K/tree/main)] :large_blue_circle:
- **MultiMath: Bridging Visual and Mathematical Reasoning for Large Language Models**, arXiv:2409.00147 [[paper](https://arxiv.org/abs/2409.00147)] [[MultiMath-300K data](https://huggingface.co/datasets/pengshuai-rin/multimath-300k)] :large_blue_circle:
- **InfiMM-WebMath-40B: Advancing Multimodal Pre-Training for Enhanced Mathematical Reasoning**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=Twzrpa6V2o)] [[InfiMM-WebMath-40B data](https://huggingface.co/datasets/Infi-MM/InfiMM-WebMath-40B)] :large_blue_circle:
- **MathGLM-Vision: Solving Mathematical Problems With Multi-Modal Large Language Model**, arXiv:2409.13729 [[paper](https://arxiv.org/abs/2409.13729)] [MathVL data] :large_blue_circle:
- **Mathematical Problem Solving in Arabic: Assessing Large Language Models**, Procedia Comput. Sci. 2024 [[paper](https://www.sciencedirect.com/science/article/pii/S187705092402982X)] [ArMATH data] :large_blue_circle:
- **M3CoT: A Novel Benchmark for Multi-Domain Multi-Step Multi-Modal Chain-of-Thought**, ACL 2024 [[paper](https://aclanthology.org/2024.acl-long.446/)] [[M3CoT data](https://huggingface.co/datasets/LightChen2333/M3CoT)] :large_blue_circle:
- **MathOdyssey: Benchmarking Mathematical Problem-Solving Skills in Large Language Models Using Odyssey Math Data**, arXiv:2406.18321 [[paper](https://arxiv.org/abs/2406.18321)] [[MathOdyssey data](https://huggingface.co/datasets/MathOdyssey/MathOdyssey)] :large_blue_circle:
- **PutnamBench: Evaluating Neural Theorem-Provers on the Putnam Mathematical Competition**, NeurIPS 2024 [[paper](https://openreview.net/forum?id=ChKCF75Ocd)] [[PutnamBench data](https://github.com/trishullab/PutnamBench)] :large_blue_circle:
- **ConceptMath: A Bilingual Concept-wise Benchmark for Measuring Mathematical Reasoning of Large Language Models**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.407/)] [[ConceptMath data](https://github.com/conceptmath/conceptmath)] :large_blue_circle:
- **Functional Benchmarks for Robust Evaluation of Reasoning Performance, and the Reasoning Gap**, arXiv:2402.19450 [[paper](https://arxiv.org/abs/2402.19450)] [MATH() data] :large_blue_circle:
- **MathBench: Evaluating the Theory and Application Proficiency of LLMs with a Hierarchical Mathematics Benchmark**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.411/)] [[MathBench data](https://github.com/open-compass/MathBench)] :large_blue_circle:
- **HARP: A Challenging Human-Annotated Math Reasoning Benchmark**, arXiv:2412.08819 [[paper](https://arxiv.org/abs/2412.08819)] [[HARP data](https://github.com/aadityasingh/HARP)] :large_blue_circle:
- **M3GIA: A Cognition-Inspired Multilingual and Multimodal General Intelligence Ability Benchmark**, arXiv:2406.05343 [[paper](https://arxiv.org/abs/2406.05343)] [[M3GIA data](https://huggingface.co/datasets/Songweii/M3GIA)] :large_blue_circle:
- **DART-Math: Difficulty-Aware Rejection Tuning for Mathematical Problem-Solving**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/0ef1afa0daa888d695dcd5e9513bafa3-Abstract-Conference.html)] [[DART-Math data](https://github.com/hkust-nlp/dart-math)] :large_blue_circle:
- **MathScale: Scaling Instruction Tuning for Mathematical Reasoning**, ICML 2024 [[paper](https://proceedings.mlr.press/v235/tang24k.html)] [[MathScaleQA data](https://huggingface.co/papers/2403.02884)] :large_blue_circle:
- **UTMath: Math Evaluation with Unit Test via Reasoning-to-Coding Thoughts**, arXiv:2411.07240 [[paper](https://arxiv.org/abs/2411.07240)] [[UTMath data](https://github.com/utmathgroup/utmath)] :large_blue_circle:
- **MultiLingPoT: Enhancing Mathematical Reasoning with Multilingual Program Fine-tuning**, arXiv:2412.12609 [[paper](https://arxiv.org/abs/2412.12609)] [[MultiLingPoT data](https://github.com/Nianqi-Li/MultiLingPoT)] :large_blue_circle:
- **System-2 Mathematical Reasoning via Enriched Instruction Tuning**, arXiv:2412.16964 [[paper](https://arxiv.org/abs/2412.16964)] [EITMath data] :large_blue_circle:
- **AtomThink: A Slow Thinking Framework for Multimodal Mathematical Reasoning**, arXiv:2411.11930 [[paper](https://arxiv.org/abs/2411.11930)] [[AMATH-SFT data](https://huggingface.co/datasets/Quinn777/AMATH-SFT)] :large_blue_circle:
- **Can Atomic Step Decomposition Enhance the Self-structured Reasoning of Multimodal Large Models?**, arXiv:2503.06252 [[paper](https://arxiv.org/abs/2503.06252)] [[AMATH-SFT data](https://huggingface.co/datasets/Quinn777/AMATH-SFT)] :large_blue_circle:
- **URSA: Understanding and Verifying Chain-of-Thought Reasoning in Multimodal Mathematics**, arXiv:2501.04686 [[paper](https://arxiv.org/abs/2501.04686)] [[MMathCoT-1M data](https://huggingface.co/datasets/URSA-MATH/MMathCoT-1M)] :large_blue_circle:
- **DynaMath: A Dynamic Visual Benchmark for Evaluating Mathematical Reasoning Robustness of Vision Language Models**, ICLR 2025 [[paper](https://openreview.net/forum?id=VOAMTA8jKu)] [[DynaMath data](https://huggingface.co/datasets/DynaMath/DynaMath_Sample)] :large_blue_circle:
- **CoMT: A Novel Benchmark for Chain of Multi-modal Thought on Large Vision-Language Models**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34538)] [[CoMT data](https://huggingface.co/datasets/czh-up/CoMT)] :large_blue_circle:
- **Feynman: Knowledge-Infused Diagramming Agent for Scaling Visual Reasoning Data**, openreview 2025 [[paper](https://openreview.net/forum?id=jNmsuEE4Gf)] [Diagramma data] :large_blue_circle:
- **MV-MATH: Evaluating Multimodal Math Reasoning in Multi-Visual Contexts**, arXiv:2502.20808 [[paper](https://arxiv.org/abs/2502.20808)] [[MV-MATH data](https://huggingface.co/datasets/PeijieWang/MV-MATH)] :large_blue_circle:
- **CMMaTH: A Chinese Multi-modal Math Skill Evaluation Benchmark for Foundation Models**, COLING 2025 [[paper](https://aclanthology.org/2025.coling-main.184/)] [CMMaTH data] :large_blue_circle:
- **Math-PUMA: Progressive Upward Multimodal Alignment to Enhance Mathematical Reasoning**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34815)] [[Math-PUMA-1M data](https://huggingface.co/Math-PUMA)] :large_blue_circle:
- **VisualWebInstruct: Scaling up Multimodal Instruction Data through Web Search**, arXiv:2503.10582 [[paper](https://arxiv.org/abs/2503.10582)] [[VisualWebInstruct data](https://huggingface.co/datasets/TIGER-Lab/VisualWebInstruct)] :large_blue_circle:
- **MAVIS: Mathematical Visual Instruction Tuning with an Automatic Data Engine**, ICLR 2025 [[data](https://github.com/ZrrSkywalker/MAVIS)] [[MAVIS-Instruct data](https://openreview.net/forum?id=MnJzJ2gvuf)]
- **Omni-MATH: A Universal Olympiad Level Mathematic Benchmark for Large Language Models**, ICLR 2025 [[paper](https://openreview.net/forum?id=yaqPf0KAlN)] [[Omni-MATH data](https://omni-math.github.io/)] :large_blue_circle:
- **MathConstruct: Challenging LLM Reasoning with Constructive Proofs**, ICLR 2025 VerifAI Workshop [[paper](https://openreview.net/forum?id=nHW2tiGMrb)] [[MathConstruct data](https://github.com/eth-sri/mathconstruct)] :large_blue_circle:
- **Benchmarking Multimodal Mathematical Reasoning with Explicit Visual Dependency**, arXiv:2504.18589 [[paper](https://arxiv.org/abs/2504.18589)] [[VCBench data](https://huggingface.co/datasets/cloudcatcher2/VCBench)] :large_blue_circle:
- **Challenging the Boundaries of Reasoning: An Olympiad-Level Math Benchmark for Large Language Models**, arXiv:2503.21380 [[paper](https://arxiv.org/abs/2503.21380)] [[OlymMATH data](https://huggingface.co/datasets/RUC-AIBOX/OlymMATH)] :large_blue_circle:
- **Recitation over Reasoning: How Cutting-Edge Language Models Can Fail on Elementary School-Level Reasoning Problems?**, arXiv:2504.00509 [[paper](https://arxiv.org/abs/2504.00509)] [[RoR-Bench data](https://huggingface.co/datasets/kaiyan289/RoR-Bench/tree/main)] :large_blue_circle:
- **PolyMath: Evaluating Mathematical Reasoning in Multilingual Contexts**, arXiv:2504.18428 [[paper](https://arxiv.org/abs/2504.18428)] [[PolyMath data](https://huggingface.co/datasets/Qwen/PolyMath)] :large_blue_circle:
- **LLMs Are Not Intelligent Thinkers: Introducing Mathematical Topic Tree Benchmark for Comprehensive Evaluation of LLMs**, NAACL 2025 [[paper](https://aclanthology.org/2025.naacl-long.161/)] [[MaTT data](https://github.com/arashgholami/MaTT)] :large_blue_circle:
- **Who's the MVP? A Game-Theoretic Evaluation Benchmark for Modular Attribution in LLM Agents**, arXiv:2502.00510 [[paper](https://arxiv.org/abs/2502.00510)] [[CapaBench data](https://github.com/zoe-yyx/CapaBench)] :large_blue_circle:
- **MATH-Perturb: Benchmarking LLMs' Math Reasoning Abilities against Hard Perturbations**, ICLR 2025 LLM Reason&Plan Workshop [[paper](https://openreview.net/forum?id=M8OLGgYK7e&referrer=%5Bthe%20profile%20of%20Xinyun%20Chen%5D%28%2Fprofile%3Fid%3D~Xinyun_Chen1%29)] [[MATH-Perturb data](https://math-perturb.github.io/)] :large_blue_circle:
- **Two Heads are Better Than One: Test-time Scaling of Multi-agent Collaborative Reasoning**, arXiv:2504.09772 [[paper](https://arxiv.org/abs/2504.09772)] [[M500 data](https://huggingface.co/datasets/Can111/m500)] :large_blue_circle:
- **Key-Point-Driven Data Synthesis with Its Enhancement on Mathematical Reasoning**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34593)] [KPMATH-M data] :large_blue_circle:
- **MathFlow: Enhancing the Perceptual Flow of MLLMs for Visual Mathematical Problems**, arXiv:2503.16549 [[paper](https://arxiv.org/abs/2503.16549)] [[FlowVerse data](https://github.com/MathFlow-zju/MathFlow)] :large_blue_circle:

## Tasks and Datasets - Other Geometry Tasks

### Geometric Diagram Generation

- **GeoX: Geometric Problem Solving Through Unified Formalized Vision-Language Pre-Training**, ICLR 2025 [[paper](https://openreview.net/forum?id=6RiBl5sCDF)] [[GeoX-pretrain data](https://huggingface.co/datasets/U4R/GeoX-data)]
- **Automatic Reconstruction of Plane Geometry Figures in Documents**, EITT 2015 [[paper](https://ieeexplore.ieee.org/abstract/document/7446145/)] :small_red_triangle: :x:
- **Solid Geometric Object Reconstruction from Single Line Drawing Image**, GRAPP 2015 [[paper](https://www.scitepress.org/PublishedPapers/2015/52612/)] :small_red_triangle: :x:
- **Recovering Solid Geometric Object from Single Line Drawing Image**, Multimed Tools Appl 2016 [[paper](https://link.springer.com/article/10.1007/s11042-015-2966-x)] :small_red_triangle: :x:
- **An Example-based Approach to 3D Man-made Object Reconstruction from Line Drawings**, Pattern Recogn 2016 [[paper](https://www.sciencedirect.com/science/article/pii/S0031320316301170)] :small_red_triangle: :x:
- **Context-aware Geometric Object Reconstruction for Mobile Education**, MM 2016 [[paper](https://dl.acm.org/doi/abs/10.1145/2964284.2967244)] :small_red_triangle: :x:
- **Automated Generation of Illustrations for Synthetic Geometry Proofs**, ADG 2021 [[paper](https://arxiv.org/abs/2201.00540)] :small_red_triangle: :x:
- **Automatically Building Diagrams for Olympiad Geometry Problems**, CADE 2021 [[paper](https://dl.acm.org/doi/abs/10.1007/978-3-030-79876-5_33)] [[GMBL data](https://github.com/rkruegs123/geo-model-builder?tab=readme-ov-file)] :small_red_triangle: :x:
- **A Precise Text-to-Diagram Generation Method for Elementary Geometry**, ICCWAMTIP 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10387090)] :small_red_triangle:
- **MagicGeo: Training-Free Text-Guided Geometric Diagram Generation**, arXiv:2502.13855 [[paper](https://arxiv.org/abs/2502.13855)] [MagicGeoBench data] :small_red_triangle:
- **GeoUni: A Unified Model for Generating Geometry Diagrams, Problems and Problem Solutions**, arXiv:2504.10146 [[paper](https://arxiv.org/pdf/2504.10146)]

### Geometric Construction Problem

- **Learning to Solve Geometric Construction Problems from Images**, CICM 2021 [[paper](https://link.springer.com/chapter/10.1007/978-3-030-81097-9_14)] :small_red_triangle:
- **EuclidNet: Deep Visual Reasoning for Constructible Problems in Geometry**, AIML 2023 [[paper](https://arxiv.org/abs/2301.13007)] :small_red_triangle:
- **Beyond Lines and Circles Unveiling the Geometric Reasoning Gap in Large Language Models**, Findings of EMNLP 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.360/)] [[Euclidea/PyEuclidea data](https://github.com/mirefek/py_euclidea)] :small_red_triangle:

### Geometric Figure Retrieval

- **Plane Geometry Figure Retrieval Based on Bilayer Geometric Attributed Graph Matching**, ICPR 2014 [[paper](https://ieeexplore.ieee.org/abstract/document/6976773/)] :small_red_triangle: :x:
- **Plane Geometry Figure Retrieval with Bag of Shapes**, IAPR 2014 DAS Workshop [[paper](https://ieeexplore.ieee.org/abstract/document/6976773/)] :small_red_triangle: :x:
- **Plane Geometry Diagram Retrieval by Using Hierarchical Searching Strategy**, ICIMCS 2016 [[paper](https://dl.acm.org/doi/abs/10.1145/3007669.3007671)] :small_red_triangle: :x:
- **Analysis of Stroke Intersection for Overlapping PGF Elements**, IAPR 2016 DAS Workshop [[paper](https://ieeexplore.ieee.org/abstract/document/7490125/)] :small_red_triangle: :x:
- **Improving PGF retrieval effectiveness with active learning**, ICPR 2016 [[paper](https://ieeexplore.ieee.org/abstract/document/7899787/)] :small_red_triangle: :x:
- **Improving Retrieval of Plane Geometry Figure with Learning to Rank**, PTRL 2016 [[paper](https://www.sciencedirect.com/science/article/abs/pii/S0167865516301040)] :small_red_triangle: :x:

### Geometric Autoformalization

- **Autoformalizing Euclidean Geometry**, ICML 2024 [[paper](https://dl.acm.org/doi/abs/10.5555/3692070.3693567)] [[LeanEuclid data](https://github.com/loganrjmurphy/LeanEuclid?tab=readme-ov-file)] :small_red_triangle:

## Methods - Architectures

### Encoder-Decoder

- **Inter-GPS: Interpretable Geometry Problem Solving with Formal Language and Symbolic Reasoning**, ACL 2021 [[paper](https://aclanthology.org/2021.acl-long.528/)]
- **GeoQA: A Geometric Question Answering Benchmark Towards Multimodal Numerical Reasoning**, Findings of ACL 2021 [[paper](https://aclanthology.org/2021.findings-acl.46)]
- **Sequence to General Tree Knowledge-Guided Geometry Word Problem Solving**, ACL-IJCNLP 2021 [[paper](https://aclanthology.org/2021.acl-short.121/)]
- **A Graph Convolutional Network Feature Learning Framework for Interpretable Geometry Problem Solving**, IEIR 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/10050084)]
- **An Augmented Benchmark Dataset for Geometric Question Answering through Dual Parallel Text Encoding**, COLING 2022 [[paper](https://aclanthology.org/2022.coling-1.130/)]
- **UniGeo: Unifying Geometry Logical Reasoning via Reformulating Mathematical Expression**, EMNLP 2022 [[paper](https://aclanthology.org/2022.emnlp-main.218/)]
- **Solving Geometry Problems via Feature Learning and Contrastive Learning of Multimodal Data**, CMES 2023 [[paper](https://openurl.ebsco.com/EPDB%3Agcd%3A9%3A20307273/detailv2?sid=ebsco%3Aplink%3Ascholar&id=ebsco%3Agcd%3A161884174&crl=c&link_origin=scholar.google.com)]
- **A Multi-Modal Neural Geometric Solver with Textual Clauses Parsed from Diagram**, IJCAI 2023 [[paper](https://www.ijcai.org/proceedings/2023/0376)]
- **UniMath: A Foundational and Multimodal Mathematical Reasoner**, EMNLP 2023 [[paper](https://aclanthology.org/2023.emnlp-main.440/)] :large_blue_circle:
- **Interpretable Geometry Problem Solving Using Improved RetinaNet and Graph Convolutional Network**, Electronics 2023 [[paper](https://www.mdpi.com/2079-9292/12/22/4578)]
- **A Symbolic Characters Aware Model for Solving Geometry Problems**, MM 2023 [[paper](https://dl.acm.org/doi/abs/10.1145/3581783.3612570/)]
- **The Geometric Neural Solution Combined with Text Diagram Parsing**, IEIR 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10391229)]
- **SUFFI-GPSC: Sufficient Geometry Problem Solution Checking with Symbolic Computation and Logical Reasoning**, ICCWAMTIP 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10387025/)]
- **LANS: A Layout-Aware Neural Solver for Plane Geometry Problem**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.153/)]
- **GAPS: Geometry-Aware Problem Solver**, arXiv:2401.16287 [[paper](https://arxiv.org/abs/2401.16287)]
- **E-GPS: Explainable Geometry Problem Solving via Top-Down Solver and Bottom-Up Generator**, CVPR 2024 [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wu_E-GPS_Explainable_Geometry_Problem_Solving_via_Top-Down_Solver_and_Bottom-Up_CVPR_2024_paper.html)]
- **FGeo-TP: A Language Model-Enhanced Solver for Geometry Problems**, Symmetry 2024 [[paper](https://www.mdpi.com/2073-8994/16/4/421)]
- **FGeo-DRL: Deductive Reasoning for Geometric Problems Through Deep Reinforcement Learning**, Symmetry 2024 [[paper](https://www.mdpi.com/2073-8994/16/4/437)]
- **FGeo-HyperGNet: Geometric Problem Solving Integrating Formal Symbolic System and Hypergraph Neural Network**, arXiv:2402.11461 [[paper](https://arxiv.org/abs/2402.11461)]
- **GOLD: Geometry Problem Solver With Natural Language Description**, Findings of NAACL 2024 [[paper](https://aclanthology.org/2024.findings-naacl.19/)]
- **Learning to Solve Geometry Problems via Simulating Human Dual-Reasoning Process**, IJCAI 2024 [[paper](https://www.ijcai.org/proceedings/2024/0725.pdf)]
- **Math-LLaVA: Bootstrapping Mathematical Reasoning for Multimodal Large Language Models**, EMNLP Findings 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.268/)] :large_blue_circle:
- **Fuse, Reason and Verify: Geometry Problem Solving With Parsed Clauses From Diagram**, arXiv:2407.07327 [[paper](https://arxiv.org/abs/2407.07327)]
- **EAGLE: Elevating Geometric Reasoning Through LLM-Empowered Visual Instruction Tuning**, arXiv:2408.11397 [[paper](https://arxiv.org/abs/2408.11397)]
- **MultiMath: Bridging Visual and Mathematical Reasoning for Large Language Models**, arXiv:2409.00147 [[paper](https://arxiv.org/abs/2409.00147)] :large_blue_circle:
- **MathGLM-Vision: Solving Mathematical Problems With Multi-Modal Large Language Model**, arXiv:2409.13729 [[paper](https://arxiv.org/abs/2409.13729)] :large_blue_circle:
- **Enhancing Geometry Problem Solving With Attention Mechanism and Super-Resolution**, ICBASE 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10762589)]
- **Geo-Qwen: A Geometry Problem-Solving Method Based on Generative Large Language Models and Heuristic Reasoning**, ICCWAMTIP 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10873683)]
- **Geo-LLaVA: A Large Multi-Modal Model for Solving Geometry Math Problems With Meta In-Context Learning**, LGM3A 2024 [[paper](https://dl.acm.org/doi/10.1145/3688866.3689124)]
- **A Geometric Neural Solving Method Based on a Diagram Text Information Fusion Analysis**, Sci. Rep. 2024 [[paper](https://www.nature.com/articles/s41598-024-83287-6)]
- **Maths: Multimodal Transformer-Based Human-Readable Solver**, ICME 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10687434)]
- **R-CoT: Reverse Chain-of-Thought Problem Generation for Geometric Reasoning in Large Multimodal Models**, arXiv:2410.17885 [[paper](https://arxiv.org/abs/2410.17885)]
- **SANS: Spatial-Aware Neural Solver for Plane Geometry Problem**, ICPR 2025 [[paper](https://link.springer.com/chapter/10.1007/978-3-031-78119-3_13)]
- **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**, ICLR 2025 [[paper](https://openreview.net/forum?id=px1674Wp3C&noteId=H99kD23um8)]
- **MAVIS: Mathematical Visual Instruction Tuning with an Automatic Data Engine**, ICLR 2025 [[paper](https://openreview.net/forum?id=MnJzJ2gvuf)]
- **GeoX: Geometric Problem Solving Through Unified Formalized Vision-Language Pre-Training**, ICLR 2025 [[paper](https://openreview.net/forum?id=6RiBl5sCDF)]
- **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)]
- **GeoDANO: Geometric VLM with Domain Agnostic Vision Encoder**, arXiv:2502.11360 [[paper](https://arxiv.org/abs/2502.11360)]
- **Math-PUMA: Progressive Upward Multimodal Alignment to Enhance Mathematical Reasoning**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34815)] :large_blue_circle:
- **GeoCoder: Solving Geometry Problems by Generating Modular Code through Vision-Language Models**, Findings of NAACL 2025 [[paper](https://aclanthology.org/2025.findings-naacl.410.pdf)]
- **VisualWebInstruct: Scaling up Multimodal Instruction Data through Web Search**, arXiv:2503.10582 [[paper](https://arxiv.org/abs/2503.10582)] [[VisualWebInstruct data](https://huggingface.co/datasets/TIGER-Lab/VisualWebInstruct)] :large_blue_circle:
- **GNS: Solving Plane Geometry Problems by Neural-Symbolic Reasoning with Multi-Modal LLMs**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34679)]
- **Enhancing the Geometric Problem-Solving Ability of Multimodal LLMs via Symbolic-Neural Integration**, arXiv:2504.12773 [[paper](https://arxiv.org/abs/2504.12773)]
- **RedStar: Does Scaling Long-CoT Data Unlock Better Slow-Reasoning Systems?**, arXiv:2501.11284 [[paper](https://arxiv.org/abs/2501.11284)]
- **Open Eyes, Then Reason: Fine-grained Visual Mathematical Understanding in MLLMs**, arXiv:2501.06430 [[paper](https://arxiv.org/abs/2501.06430)]
- **LMM-R1: Empowering 3B LMMs with Strong Reasoning Abilities Through Two-Stage Rule-Based RL**, arXiv:2503.07536 [[paper](https://arxiv.org/abs/2503.07536)]

### Other Architectures

- **Geometry Problem Solving Based on Counter-factual Evolutionary Reasoning**, CASE 2023 [[paper](https://scholar.googleusercontent.com/scholar.bib?q=info:886PxuxR1JUJ:scholar.google.com/&output=citation&scisdr=ClEqZRNsEMPsmsftMLY:AFWwaeYAAAAAZ3_rKLazJo3qQt7lUpGqpZbgTnM&scisig=AFWwaeYAAAAAZ3_rKO4RO1QaJNkkTXC9mGtJJJQ&scisf=4&ct=citation&cd=-1&hl=zh-CN)]
- **GeoDRL: A Self-Learning Framework for Geometry Problem Solving using Reinforcement Learning in Deductive Reasoning**, ACL 2023 [[paper](https://aclanthology.org/2023.findings-acl.850/)]
- **Hologram Reasoning for Solving Algebra Problems With Geometry Diagrams**, arXiv:2408.10592 [[paper](https://arxiv.org/abs/2408.10592)]
- **Solving Olympiad Geometry Without Human Demonstrations**, Nature 2024 [[paper](https://www.nature.com/articles/s41586-023-06747-5)]
- **Wu’s Method Boosts Symbolic AI to Rival Silver Medalists and AlphaGeometry to Outperform Gold Medalists at IMO Geometry**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=aKRtC45gle)]
- **Proposing and Solving Olympiad Geometry with Guided Tree Search**, arXiv:2412.10673 [[paper](https://arxiv.org/abs/2412.10673)]
- **Gold-medalist Performance in Solving Olympiad Geometry with AlphaGeometry2**, arXiv:2502.03544 [[paper](https://arxiv.org/abs/2502.03544)]
- **DART-Math: Difficulty-Aware Rejection Tuning for Mathematical Problem-Solving**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/0ef1afa0daa888d695dcd5e9513bafa3-Abstract-Conference.html)] :large_blue_circle:
- **MultiLingPoT: Enhancing Mathematical Reasoning with Multilingual Program Fine-tuning**, arXiv:2412.12609 [[paper](https://arxiv.org/abs/2412.12609)] :large_blue_circle:
- **MathScale: Scaling Instruction Tuning for Mathematical Reasoning**, ICML 2024 [[paper](https://proceedings.mlr.press/v235/tang24k.html)] :large_blue_circle:
- **System-2 Mathematical Reasoning via Enriched Instruction Tuning**, arXiv:2412.16964 [[paper](https://arxiv.org/abs/2412.16964)] :large_blue_circle:
- **Pi-GPS: Enhancing Geometry Problem Solving by Unleashing the Power of Diagrammatic Information**, arXiv:2503.05543 [[paper](https://arxiv.org/abs/2503.05543)]
- **GeoUni: A Unified Model for Generating Geometry Diagrams, Problems and Problem Solutions**, arXiv:2504.10146 [[paper](https://arxiv.org/pdf/2504.10146)]
- **Offline Training of Language Model Agents with Functions as Learnable Weights**, ICML 2024 [[paper](https://proceedings.mlr.press/v235/zhang24cd.html)] :large_blue_circle:
- **Strategyllm: Large Language Models as Strategy Generators, Executors, Optimizers, and Evaluators for Problem Solving**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/af7cc9e2366b8f8837a6ef339810277a-Abstract-Conference.html)] :large_blue_circle:
- **MACM: Utilizing a Multi-Agent System for Condition Mining in Solving Complex Mathematical Problems**, NeurIPS 2024 [[paper](https://openreview.net/forum?id=VR2RdSxtzs)] :large_blue_circle:
- **Breaking Mental Set to Improve Reasoning through Diverse Multi-Agent Debate**, ICLR 2025 [[paper](https://openreview.net/forum?id=t6QHYUOQL7)] :large_blue_circle:

## Methods - Training Stage

### Pre-Training

- **GeoQA: A Geometric Question Answering Benchmark Towards Multimodal Numerical Reasoning**, Findings of ACL 2021 [[paper](https://aclanthology.org/2021.findings-acl.46)]
- **UniGeo: Unifying Geometry Logical Reasoning via Reformulating Mathematical Expression**, EMNLP 2022 [[paper](https://aclanthology.org/2022.emnlp-main.218/)]
- **A Multi-Modal Neural Geometric Solver with Textual Clauses Parsed from Diagram**, IJCAI 2023 [[paper](https://www.ijcai.org/proceedings/2023/0376)]
- **Fuse, Reason and Verify: Geometry Problem Solving With Parsed Clauses From Diagram**, arXiv:2407.07327 [[paper](https://arxiv.org/abs/2407.07327)]
- **A Symbolic Characters Aware Model for Solving Geometry Problems**, MM 2023 [[paper](https://dl.acm.org/doi/abs/10.1145/3581783.3612570/)]
- **LANS: A Layout-Aware Neural Solver for Plane Geometry Problem**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.153/)]
- **A Geometric Neural Solving Method Based on a Diagram Text Information Fusion Analysis**, Sci. Rep. 2024 [[paper](https://www.nature.com/articles/s41598-024-83287-6)]
- **SANS: Spatial-Aware Neural Solver for Plane Geometry Problem**, ICPR 2025 [[paper](https://link.springer.com/chapter/10.1007/978-3-031-78119-3_13)]
- **Measuring Mathematical Problem Solving With the MATH Dataset**, NeurIPS 2021 [[paper](https://datasets-benchmarks-proceedings.neurips.cc/paper_files/paper/2021/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper-round2.pdf)] :large_blue_circle:
- **InfiMM-WebMath-40B: Advancing Multimodal Pre-Training for Enhanced Mathematical Reasoning**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=Twzrpa6V2o)] :large_blue_circle:
- **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)]
- **GeoX: Geometric Problem Solving Through Unified Formalized Vision-Language Pre-Training**, ICLR 2025 [[paper](https://openreview.net/forum?id=6RiBl5sCDF)]
- **MAVIS: Mathematical Visual Instruction Tuning with an Automatic Data Engine**, ICLR 2025 [[data](https://github.com/ZrrSkywalker/MAVIS)]
- **GeoDANO: Geometric VLM with Domain Agnostic Vision Encoder**, arXiv:2502.11360 [[paper](https://arxiv.org/abs/2502.11360)]
- **Open Eyes, Then Reason: Fine-grained Visual Mathematical Understanding in MLLMs**, arXiv:2501.06430 [[paper](https://arxiv.org/abs/2501.06430)]

### Supervised Fine-Tuning

- **Synthetic Data Generator for Solving Korean Arithmetic Word Problem**, Mathematics 2022 [[paper](https://www.mdpi.com/2227-7390/10/19/3525)] :large_blue_circle:
- **GeomVerse: A Systematic Evaluation of Large Models for Geometric Reasoning**, ICML 2024 AI4MATH Workshop [[paper](https://openreview.net/forum?id=1AUbiBrOF1)]
- **MAVIS: Mathematical Visual Instruction Tuning with an Automatic Data Engine**, ICLR 2025 [[paper](https://openreview.net/forum?id=MnJzJ2gvuf)]
- **Enhancing the Geometric Problem-Solving Ability of Multimodal LLMs via Symbolic-Neural Integration**, arXiv:2504.12773 [[paper](https://arxiv.org/abs/2504.12773)]
- **TrustGeoGen: Scalable and Formal-Verified Data Engine for Trustworthy Multi-modal Geometric Problem Solving**, arXiv:2504.15780 [[paper](https://arxiv.org/abs/2504.15780)]
- **MATHGLANCE: Multimodal Large Language Models Do Not Know Where to Look in Mathematical Diagrams**, arXiv:2503.20745 [[paper](https://arxiv.org/abs/2503.20745)] [[MATHGLANCE/GeoPeP data](https://mathglance.github.io/)]
- **Why Vision Language Models Struggle with Visual Arithmetic? Towards Enhanced Chart and Geometry Understanding**, Findings of ACL 2025 [[paper](https://arxiv.org/abs/2502.11492)] [[CogAlign-Probing/CogAlign-train data](https://huggingface.co/datasets/Salesforce/CogAlign)]
- **VisOnlyQA: Large Vision Language Models Still Struggle With Visual Perception of Geometric Information**, arXiv:2412.00947 [[paper](https://arxiv.org/abs/2412.00947)] :large_blue_circle:
- **MathScale: Scaling Instruction Tuning for Mathematical Reasoning**, ICML 2024 [[paper](https://proceedings.mlr.press/v235/tang24k.html)] :large_blue_circle:
- **Key-Point-Driven Data Synthesis with Its Enhancement on Mathematical Reasoning**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34593)] :large_blue_circle:
- **R-CoT: Reverse Chain-of-Thought Problem Generation for Geometric Reasoning in Large Multimodal Models**, arXiv:2410.17885 [[paper](https://arxiv.org/abs/2410.17885)]
- **VISTA: Visual Integrated System for Tailored Automation in Math Problem Generation Using LLM**, PMLR 2025 [[paper](https://proceedings.mlr.press/v264/lee25b)]
- **Feynman: Knowledge-Infused Diagramming Agent for Scaling Visual Reasoning Data**, openreview 2025 [[paper](https://openreview.net/forum?id=jNmsuEE4Gf)] :large_blue_circle:
- **Proposing and Solving Olympiad Geometry with Guided Tree Search**, arXiv:2412.10673 [[paper](https://arxiv.org/abs/2412.10673)]
- **An Augmented Benchmark Dataset for Geometric Question Answering through Dual Parallel Text Encoding**, COLING 2022 [[paper](https://aclanthology.org/2022.coling-1.130/)]
- **A Multi-Modal Neural Geometric Solver with Textual Clauses Parsed from Diagram**, IJCAI 2023 [[paper](https://www.ijcai.org/proceedings/2023/0376)]
- **GAPS: Geometry-Aware Problem Solver**, arXiv:2401.16287 [[paper](https://arxiv.org/abs/2401.16287)]
- **E-GPS: Explainable Geometry Problem Solving via Top-Down Solver and Bottom-Up Generator**, CVPR 2024 [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wu_E-GPS_Explainable_Geometry_Problem_Solving_via_Top-Down_Solver_and_Bottom-Up_CVPR_2024_paper.html)]
- **FormalGeo: An Extensible Formalized Framework for Olympiad Geometric Problem Solving**, arXiv:2310.18021 [[paper](https://arxiv.org/abs/2310.18021)] :x:
- **A Deep Reinforcement Learning Agent for Geometry Online Tutoring**, KAIS 2023 [[paper](https://link.springer.com/article/10.1007/s10115-022-01804-3)]
- **SANS: Spatial-Aware Neural Solver for Plane Geometry Problem**, ICPR 2025 [[paper](https://link.springer.com/chapter/10.1007/978-3-031-78119-3_13)]
- **DART-Math: Difficulty-Aware Rejection Tuning for Mathematical Problem-Solving**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/0ef1afa0daa888d695dcd5e9513bafa3-Abstract-Conference.html)] :large_blue_circle:
- **Math-LLaVA: Bootstrapping Mathematical Reasoning for Multimodal Large Language Models**, EMNLP Findings 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.268/)] [[MathV360K data](https://huggingface.co/datasets/Zhiqiang007/MathV360K/tree/main)] :large_blue_circle:
- **GeoVQA: A Comprehensive Multimodal Geometry Dataset for Secondary Education**, MIPR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10707789)]
- **Advancing Multimodal LLMs: A Focus on Geometry Problem Solving Reasoning and Sequential Scoring**, MMASIA 2024 [[paper](https://dl.acm.org/doi/full/10.1145/3696409.3700262)]
- **Vision-Language Models Can Self-Improve Reasoning via Reflection**, arXiv:2411.00855 [[paper](https://arxiv.org/abs/2411.00855)] :large_blue_circle:
- **MultiLingPoT: Enhancing Mathematical Reasoning with Multilingual Program Fine-tuning**, arXiv:2412.12609 [[paper](https://arxiv.org/abs/2412.12609)] :large_blue_circle:
- **System-2 Mathematical Reasoning via Enriched Instruction Tuning**, arXiv:2412.16964 [[paper](https://arxiv.org/abs/2412.16964)] :large_blue_circle:
- **MM-Verify: Enhancing Multimodal Reasoning with Chain-of-Thought Verification**, arXiv:2502.13383 [[paper](https://arxiv.org/abs/2502.13383)] :large_blue_circle:
- **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**, ICLR 2025 [[paper](https://openreview.net/forum?id=px1674Wp3C&noteId=H99kD23um8)]
- **GeoCoder: Solving Geometry Problems by Generating Modular Code through Vision-Language Models**, Findings of NAACL 2025 [[paper](https://aclanthology.org/2025.findings-naacl.410.pdf)]
- **M3CoT: A Novel Benchmark for Multi-Domain Multi-Step Multi-Modal Chain-of-Thought**, ACL 2024 [[paper](https://aclanthology.org/2024.acl-long.446/)] :large_blue_circle:
- **URSA: Understanding and Verifying Chain-of-Thought Reasoning in Multimodal Mathematics**, arXiv:2501.04686 [[paper](https://arxiv.org/abs/2501.04686)] :large_blue_circle:
- **GNS: Solving Plane Geometry Problems by Neural-Symbolic Reasoning with Multi-Modal LLMs**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34679)]
- **LLaVA-o1: Let Vision Language Models Reason Step-by-Step**, arXiv:2411.10440 [[paper](https://arxiv.org/abs/2411.10440)] :large_blue_circle:
- **AtomThink: A Slow Thinking Framework for Multimodal Mathematical Reasoning**, arXiv:2411.11930 [[paper](https://arxiv.org/abs/2411.11930)] :large_blue_circle:
- **RedStar: Does Scaling Long-CoT Data Unlock Better Slow-Reasoning Systems?**, arXiv:2501.11284 [[paper](https://arxiv.org/abs/2501.11284)]
- **Virgo: A Preliminary Exploration on Reproducing o1-like MLLM**, arXiv:2501.01904 [[paper](https://arxiv.org/abs/2501.01904)] :large_blue_circle:
- **BBA: Bi-Modal Behavioral Alignment for Reasoning with Large Vision-Language Models**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.433/)]
- **GeoGPT4V: Towards Geometric Multi-Modal Large Language Models With Geometric Image Generation**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.44/)]
- **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)]
- **GeoX: Geometric Problem Solving Through Unified Formalized Vision-Language Pre-Training**, ICLR 2025 [[paper](https://openreview.net/forum?id=6RiBl5sCDF)]
- **SoTA with Less: MCTS-Guided Sample Selection for Data-Efficient Visual Reasoning Self-Improvement**, arXiv:2504.07934 [[paper](https://arxiv.org/abs/2504.07934)] :large_blue_circle:
- **VisualWebInstruct: Scaling up Multimodal Instruction Data through Web Search**, arXiv:2503.10582 [[paper](https://arxiv.org/abs/2503.10582)] :large_blue_circle:

### Reinforcement Learning

- **A Deep Reinforcement Learning Agent for Geometry Online Tutoring**, KAIS 2023 [[paper](https://link.springer.com/article/10.1007/s10115-022-01804-3)]
- **GeoDRL: A Self-Learning Framework for Geometry Problem Solving using Reinforcement Learning in Deductive Reasoning**, ACL 2023 [[paper](https://aclanthology.org/2023.findings-acl.850/)]
- **FGeo-DRL: Deductive Reasoning for Geometric Problems Through Deep Reinforcement Learning**, Symmetry 2024 [[paper](https://www.mdpi.com/2073-8994/16/4/437)]
- **Hologram Reasoning for Solving Algebra Problems With Geometry Diagrams**, arXiv:2408.10592 [[paper](https://arxiv.org/abs/2408.10592)]
- **LMM-R1: Empowering 3B LMMs with Strong Reasoning Abilities Through Two-Stage Rule-Based RL**, arXiv:2503.07536 [[paper](https://arxiv.org/abs/2503.07536)]
- **MultiMath: Bridging Visual and Mathematical Reasoning for Large Language Models**, arXiv:2409.00147 [[paper](https://arxiv.org/abs/2409.00147)] :large_blue_circle:
- **MAVIS: Mathematical Visual Instruction Tuning with an Automatic Data Engine**, ICLR 2025 [[paper](https://openreview.net/forum?id=MnJzJ2gvuf)]
- **RedStar: Does Scaling Long-CoT Data Unlock Better Slow-Reasoning Systems?**, arXiv:2501.11284 [[paper](https://arxiv.org/abs/2501.11284)]
- **Why Vision Language Models Struggle with Visual Arithmetic? Towards Enhanced Chart and Geometry Understanding**, Findings of ACL 2025 [[paper](https://arxiv.org/abs/2502.11492)]
- **Vision-R1: Incentivizing Reasoning Capability in Multimodal Large Language Models**, arXiv:2503.06749 [[paper](https://arxiv.org/abs/2503.06749)] :large_blue_circle:
- **OpenVLThinker: An Early Exploration to Complex Vision-Language Reasoning via Iterative Self-Improvement**, arXiv:2503.17352 [[paper](https://arxiv.org/abs/2503.17352)] :large_blue_circle:
- **Reason-RFT: Reinforcement Fine-Tuning for Visual Reasoning**, arXiv:2503.20752 [[paper](https://arxiv.org/abs/2503.20752)] :large_blue_circle:
- **Boosting the Generalization and Reasoning of Vision Language Models with Curriculum Reinforcement Learning**, arXiv:2503.07065 [[paper](https://arxiv.org/abs/2502.15969)] :large_blue_circle:
- **GeoUni: A Unified Model for Generating Geometry Diagrams, Problems and Problem Solutions**, arXiv:2504.10146 [[paper](https://arxiv.org/pdf/2504.10146)]
- **Boosting MLLM Reasoning with Text-Debiased Hint-GRPO**, arXiv:2503.23905 [[paper](https://arxiv.org/abs/2503.23905)]
- **SFT or RL? An Early Investigation into Training R1-Like Reasoning Large Vision-Language Models**, arXiv:2504.11468 [[paper](https://arxiv.org/abs/2504.11468)] :large_blue_circle:
- **NoisyRollout: Reinforcing Visual Reasoning with Data Augmentation**, arXiv:2504.13055 [[paper](https://arxiv.org/abs/2504.13055)] :large_blue_circle:
- **Reinforcement Learning for Reasoning in Large Language Models with One Training Example**, arXiv:2504.20571 [[paper](https://arxiv.org/abs/2504.20571)] :large_blue_circle:
- **GPG: A Simple and Strong Reinforcement Learning Baseline for Model Reasoning**, arXiv:2504.02546 [[paper](https://arxiv.org/abs/2504.02546)]

## Methods - Inference Stage

### Test-Time Scaling

- **Reprompting: Automated Chain-of-Thought Prompt Inference Through Gibbs Sampling**, ICML 2024 [[paper](https://proceedings.mlr.press/v235/xu24b.html)] :large_blue_circle:
- **Hint-before-Solving Prompting: Guiding LLMs to Effectively Utilize Encoded Knowledge**, arXiv:2402.14310 [[paper](https://arxiv.org/abs/2402.14310)] :large_blue_circle:
- **Null-Shot Prompting: Rethinking Prompting Large Language Models With Hallucination**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.740/)] :large_blue_circle:
- **Cumulative Reasoning with Large Language Models**, arXiv:2308.04371 [[paper](https://arxiv.org/abs/2308.04371)] :large_blue_circle:
- **Progressive-Hint Prompting Improves Reasoning in Large Language Models**, ICML 2024 AI4MATH Workshop [[paper](https://openreview.net/forum?id=UkFEs3ciz8)] :large_blue_circle:
- **MathSensei: Mathematical Reasoning with a Tool-Augmented Large Language Model**, ICLR 2024 ME-FoMo Workshop [[paper](https://openreview.net/forum?id=YDQ6eBB4py)] :large_blue_circle:
- **Divide-and-Conquer Meets Consensus: Unleashing the Power of Functions in Code Generation**, NeurIPS 2024 [[paper](https://openreview.net/forum?id=cFqAANINgW)] :large_blue_circle:
- **SBSC: Step-By-Step Coding for Improving Mathematical Olympiad Performance**, ICLR 2025 [[paper](https://openreview.net/forum?id=wSkvf2WyYz)] :large_blue_circle:
- **Reason-and-Execute Prompting: Enhancing Multi-Modal Large Language Models for Solving Geometry Questions**, MM 2024 [[paper](https://dl.acm.org/doi/abs/10.1145/3664647.3681484)]
- **Plan, Verify and Switch: Integrated Reasoning with Diverse X-of-Thoughts**, EMNLP 2023 [[paper](https://aclanthology.org/2023.emnlp-main.169/)] :large_blue_circle:
- **CREATOR: Tool Creation for Disentangling Abstract and Concrete Reasoning of Large Language Models**, Findings of EMNLP 2023 [[paper](https://aclanthology.org/2023.findings-emnlp.462/)] :large_blue_circle:
- **ToRA: A Tool-Integrated Reasoning Agent for Mathematical Problem Solving**, ICLR 2024 [[paper](https://openreview.net/forum?id=Ep0TtjVoap)] :large_blue_circle:
- **Evaluating Automated Geometric Problem Solving With Formal Language Generation on Large Multimodal Models**, IEIR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10959992)]
- **Describe-then-Reason: Improving Multimodal Mathematical Reasoning Through Visual Comprehension Training**, arXiv:2404.14604 [[paper](https://arxiv.org/abs/2404.14604)] :large_blue_circle:
- **Beyond Captioning: Task-Specific Prompting for Improved VLM Performance in Mathematical Reasoning**, arXiv:2410.05928 [[paper](https://arxiv.org/abs/2410.05928)]
- **Multi-Step Chain-of-Thought in Geometry Problem Solving**, EIECS 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10800087)]
- **Proposing and Solving Olympiad Geometry with Guided Tree Search**, arXiv:2412.10673 [[paper](https://arxiv.org/abs/2412.10673)]
- **Enhancing the Geometric Problem-Solving Ability of Multimodal LLMs via Symbolic-Neural Integration**, arXiv:2504.12773 [[paper](https://arxiv.org/abs/2504.12773)]
- **Solving Olympiad Geometry Without Human Demonstrations**, Nature 2024 [[paper](https://www.nature.com/articles/s41586-023-06747-5)]
- **Gold-medalist Performance in Solving Olympiad Geometry with AlphaGeometry2**, arXiv:2502.03544 [[paper](https://arxiv.org/abs/2502.03544)]
- **GeoDRL: A Self-Learning Framework for Geometry Problem Solving using Reinforcement Learning in Deductive Reasoning**, ACL 2023 [[paper](https://aclanthology.org/2023.findings-acl.850/)]
- **GAPS: Geometry-Aware Problem Solver**, arXiv:2401.16287 [[paper](https://arxiv.org/abs/2401.16287)]
- **LLaVA-o1: Let Vision Language Models Reason Step-by-Step**, arXiv:2411.10440 [[paper](https://arxiv.org/abs/2411.10440)] :large_blue_circle:
- **FGeo-DRL: Deductive Reasoning for Geometric Problems Through Deep Reinforcement Learning**, Symmetry 2024 [[paper](https://www.mdpi.com/2073-8994/16/4/437)]
- **MC-NEST--Enhancing Mathematical Reasoning in Large Language Models with a Monte Carlo Nash Equilibrium Self-Refine Tree**, arXiv:2411.15645 [[paper](https://arxiv.org/abs/2411.15645)] :large_blue_circle:
- **Mulberry: Empowering MLLM With o1-like Reasoning and Reflection via Collective Monte Carlo Tree Search**, arXiv:2412.18319 [[paper](https://arxiv.org/abs/2412.18319)] :large_blue_circle:
- **Progressive Multimodal Reasoning via Active Retrieval**, arXiv:2412.14835 [[paper](https://arxiv.org/abs/2412.14835)] :large_blue_circle:
- **Boosting Multimodal Reasoning with MCTS-Automated Structured Thinking**, arXiv:2502.02339 [[paper](https://arxiv.org/abs/2502.02339)] :large_blue_circle:
- **VisuoThink: Empowering LVLM Reasoning with Multimodal Tree Search**, arXiv:2504.09130 [[paper](https://arxiv.org/abs/2504.09130)]
- **Deliberate Reasoning for LLMs as Structure-Aware Planning with Accurate World Model**, arXiv:2410.03136 [[paper](https://arxiv.org/abs/2410.03136)] :large_blue_circle:
- **AtomThink: A Slow Thinking Framework for Multimodal Mathematical Reasoning**, arXiv:2411.11930 [[paper](https://arxiv.org/abs/2411.11930)] :large_blue_circle:
- **Can Atomic Step Decomposition Enhance the Self-structured Reasoning of Multimodal Large Models?**, arXiv:2503.06252 [[paper](https://arxiv.org/abs/2503.06252)] :large_blue_circle:
- **URSA: Understanding and Verifying Chain-of-Thought Reasoning in Multimodal Mathematics**, arXiv:2501.04686 [[paper](https://arxiv.org/abs/2501.04686)] :large_blue_circle:
- **VisualPRM: An Effective Process Reward Model for Multimodal Reasoning**, arXiv:2503.10291 [[paper](https://arxiv.org/abs/2503.10291)] :large_blue_circle:
- **VILBENCH: A Suite for Vision-Language Process Reward Modeling**, arXiv:2503.20271 [[paper](https://arxiv.org/abs/2503.20271)] :large_blue_circle:
- **PRM-BAS: Enhancing Multimodal Reasoning through PRM-guided Beam Annealing Search**, arXiv:2504.10222 [[paper](https://arxiv.org/abs/2504.10222)] :large_blue_circle:
- **Learning From Correctness Without Prompting Makes LLM Efficient Reasoner**, COLM 2024 [[paper](https://openreview.net/forum?id=dcbNzhVVQj)] :large_blue_circle:
- **Generative Verifiers: Reward Modeling as Next-Token Prediction**, ICLR 2025 [[paper](https://openreview.net/forum?id=Ccwp4tFEtE)] :large_blue_circle:
- **Vision-Language Models Can Self-Improve Reasoning via Reflection**, arXiv:2411.00855 [[paper](https://arxiv.org/abs/2411.00855)] :large_blue_circle:
- **Two Heads are Better Than One: Test-time Scaling of Multi-agent Collaborative Reasoning**, arXiv:2504.09772 [[paper](https://arxiv.org/abs/2504.09772)] :large_blue_circle:

### Knowledge-Augmented Inference
- **Give me a Hint: Can LLMs Take a Hint to Solve Math Problems?**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=eeZG97VjYa)] :large_blue_circle:
- **Skills-in-Context: Unlocking Compositionality in Large Language Models**, Findings of EMNLP 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.812/)] :large_blue_circle:
- **Curriculum Demonstration Selection for In-Context Learning**, SAC 2025 [[paper](https://dl.acm.org/doi/abs/10.1145/3672608.3707810)] :large_blue_circle:
- **CoMT: A Novel Benchmark for Chain of Multi-modal Thought on Large Vision-Language Models**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34538)] :large_blue_circle:
- **All in an Aggregated Image for In-Image Learning**, arXiv:2402.17971 [[paper](https://arxiv.org/abs/2402.17971)] :large_blue_circle:
- **Geo-LLaVA: A Large Multi-Modal Model for Solving Geometry Math Problems With Meta In-Context Learning**, LGM3A 2024 [[paper](https://dl.acm.org/doi/10.1145/3688866.3689124)]
- **Advancing Multimodal LLMs: A Focus on Geometry Problem Solving Reasoning and Sequential Scoring**, MMASIA 2024 [[paper](https://dl.acm.org/doi/full/10.1145/3696409.3700262)]
- **GeoCoder: Solving Geometry Problems by Generating Modular Code through Vision-Language Models**, Findings of NAACL 2025 [[paper](https://aclanthology.org/2025.findings-naacl.410.pdf)]
- **Enhancing LLM Reasoning via Vision-Augmented Prompting**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/328c922d068dd4ccb23cec5c64e6c7fc-Abstract-Conference.html)]
- **Visual Sketchpad: Sketching as a Visual Chain of Thought for Multimodal Language Models**, NeurIPS 2024 [[paper](https://openreview.net/forum?id=GNSMl1P5VR)] :large_blue_circle:
- **Interactive Sketchpad: A Multimodal Tutoring System for Collaborative, Visual Problem-Solving**, arXiv:2503.16434 [[paper](https://arxiv.org/abs/2503.16434)] :large_blue_circle:
- **CogCom: A Visual Language Model with Chain-of-Manipulations Reasoning**, ICLR 2025 [[paper](https://openreview.net/forum?id=Fg0eo2AkST)] :large_blue_circle:
- **VisuoThink: Empowering LVLM Reasoning with Multimodal Tree Search**, arXiv:2504.09130 [[paper](https://arxiv.org/abs/2504.09130)]
- **Learning to Plan by Updating Natural Language**, Findings of EMNLP 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.589/)] :large_blue_circle:
- **Explicit Memory Learning with Expectation Maximization**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.927.pdf)] :large_blue_circle:

## Related Surveys

- **The Gap of Semantic Parsing: A Survey on Automatic Math Word Problem Solvers**, TPAMI 2019 [[paper](https://library.oapen.org/bitstream/handle/20.500.12657/61269/978-3-031-09687-7.pdf?sequence=1#page=246)] :large_blue_circle: :x:
- **Deep Learning in Automatic Math Word Problem Solvers**, AI in Learning: Designing the Future 2022 [[article](https://library.oapen.org/bitstream/handle/20.500.12657/61269/978-3-031-09687-7.pdf?sequence=1#page=246)] :large_blue_circle:
- **Evolution of Automated Deduction and Dynamic Constructions in Geometry**, Mathematics Education in the Age of Artificial Intelligence: How Artificial Intelligence can Serve Mathematical Human Learning 2022 [[article](https://link.springer.com/chapter/10.1007/978-3-030-86909-0_1)] :x:
- **A Survey of Deep Learning for Mathematical Reasoning**, ACL 2023 [[paper](https://aclanthology.org/2023.acl-long.817/)] :large_blue_circle:
- **Systematic Literature Review: Application of Dynamic Geometry Software to Improve Mathematical Problem-Solving Skills**, Mathline: Jurnal Matematika Dan Pendidikan Matematika 2023 [[paper](https://mathline.unwir.ac.id/index.php/Mathline/article/view/458)] :x:
- **A Survey of Reasoning with Foundation Models**, arXiv:2312.11562 [[paper](https://arxiv.org/abs/2312.11562)] :large_blue_circle:
- **A Survey of Reasoning with Foundation Models: Concepts, Methodologies, and Outlook**, ACM Comput. Surv. 2023 [[paper](https://dl.acm.org/doi/full/10.1145/3729218)] :large_blue_circle:
- **Adapting Large Language Models for Education: Foundational Capabilities, Potentials, and Challenges**, arXiv:2401.08664 [[paper](https://arxiv.org/abs/2401.08664)] :large_blue_circle:
- **Large Language Models for Mathematical Reasoning: Progresses and Challenges**, EACL 2024 [[paper](https://aclanthology.org/2024.eacl-srw.17/)] :large_blue_circle:
- **A Survey on Deep Learning for Theorem Proving**, COLM 2024 [[paper](https://openreview.net/forum?id=zlw6AHwukB)] :large_blue_circle:
- **A Comprehensive Survey of Scientific Large Language Models and Their Applications in Scientific Discovery**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.498/)] :large_blue_circle:
- **Towards Robust Automated Math Problem Solving: A Survey of Statistical and Deep Learning Approaches**, Evol. Intell. 2024 [[paper](https://link.springer.com/article/10.1007/s12065-024-00957-0)] :large_blue_circle:
- **A Survey of Mathematical Reasoning in the Era of Multimodal Large Language Model: Benchmark, Method & Challenges**, Findings of ACL 2025 [[paper](https://arxiv.org/abs/2412.11936)] :large_blue_circle:
- **Decoding Math: A Review of Datasets Shaping AI-Driven Mathematical Reasoning**, JIM 2025 [[paper](https://www.tarupublications.com/doi/10.47974/JIM-2105)] :large_blue_circle:
- **Visual Large Language Models for Generalized and Specialized Application**, arXiv:2501.02765 [[paper](https://arxiv.org/abs/2501.02765)] :large_blue_circle:
- **From System 1 to System 2: A Survey of Reasoning Large Language Models**, arXiv:2502.17419 [[paper](https://arxiv.org/abs/2502.17419)] :large_blue_circle:
- **Towards Scientific Intelligence: A Survey of LLM-based Scientific Agents**, arXiv:2503.24047 [[paper](https://arxiv.org/abs/2503.24047)] :large_blue_circle:

## Years

### 2014

1. **Diagram Understanding in Geometry Questions**, AAAI 2014 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/9146)] :x:
2. **Synthesis of Geometry Proof Problems**, AAAI 2014 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/8745)] :x:
3. **Plane Geometry Figure Retrieval Based on Bilayer Geometric Attributed Graph Matching**, ICPR 2014 [[paper](https://ieeexplore.ieee.org/abstract/document/6976773/)] :small_red_triangle: :x:
4. **Plane Geometry Figure Retrieval with Bag of Shapes**, IAPR 2014 DAS Workshop [[paper](https://ieeexplore.ieee.org/abstract/document/6976773/)] :small_red_triangle: :x:

### 2015

1. **Solving Geometry Problems: Combining Text and Diagram Interpretation**, EMNLP 2015 [[paper](https://aclanthology.org/D15-1171/)] :x:
2. **Automatic Reconstruction of Plane Geometry Figures in Documents**, EITT 2015 [[paper](https://ieeexplore.ieee.org/abstract/document/7446145/)] :small_red_triangle: :x:
3. **Overlapped-Triangle Analysis with Hierarchical Ranking of Dominance**, ICDAR 2015 [[paper](https://ieeexplore.ieee.org/abstract/document/7333870/)] :x:
4. **Solid Geometric Object Reconstruction from Single Line Drawing Image**, GRAPP 2015 [[paper](https://www.scitepress.org/PublishedPapers/2015/52612/)] :small_red_triangle: :x:

### 2016

1. **Plane Geometry Diagram Retrieval by Using Hierarchical Searching Strategy**, ICIMCS 2016 [[paper](https://dl.acm.org/doi/abs/10.1145/3007669.3007671)] :small_red_triangle: :x:
2. **Analysis of Stroke Intersection for Overlapping PGF Elements**, IAPR 2016 DAS Workshop [[paper](https://ieeexplore.ieee.org/abstract/document/7490125/)] :small_red_triangle: :x:
3. **AnalyticalInk: An Interactive Learning Environment for Math Word Problem Solving**, IUI 2016 [[paper](https://dl.acm.org/doi/abs/10.1145/2856767.2856789)] :x:
4. **My Computer Is an Honor Student — but How Intelligent Is It? Standardized Tests as a Measure of AI**, AIMA 2016 [[paper](https://ojs.aaai.org/aimagazine/index.php/aimagazine/article/view/2636)] :large_blue_circle: :x:
5. **Improving PGF retrieval effectiveness with active learning**, ICPR 2016 [[paper](https://ieeexplore.ieee.org/abstract/document/7899787/)] :small_red_triangle: :x:
6. **Improving Retrieval of Plane Geometry Figure with Learning to Rank**, PTRL 2016 [[paper](https://www.sciencedirect.com/science/article/abs/pii/S0167865516301040)] :small_red_triangle: :x:
7. **Recovering Solid Geometric Object from Single Line Drawing Image**, Multimed Tools Appl 2016 [[paper](https://link.springer.com/article/10.1007/s11042-015-2966-x)] :small_red_triangle: :x:
8. **An Example-based Approach to 3D Man-made Object Reconstruction from Line Drawings**, Pattern Recogn 2016 [[paper](https://www.sciencedirect.com/science/article/pii/S0031320316301170)] :small_red_triangle: :x:
9. **Context-aware Geometric Object Reconstruction for Mobile Education**, MM 2016 [[paper](https://dl.acm.org/doi/abs/10.1145/2964284.2967244)] :small_red_triangle: :x:

### 2017

1. **Semantic Parsing of Pre-University Math Problems**, ACL 2017 [[paper](https://aclanthology.org/P17-1195/)] :x:
2. **Synthesis of Solutions for Shaded Area Geometry Problems**, FLAIRS 2017 [[paper](https://aaai.org/papers/14-flairs-2017-15416/)] :x:
3. **From Textbooks to Knowledge: A Case Study in Harvesting Axiomatic Knowledge from Textbooks to Solve Geometry Problems**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1081/)] :x:
4. **Learning to Solve Geometry Problems from Natural Language Demonstrations in Textbooks**, *SEM 2017 [[paper](https://aclanthology.org/S17-1029/)] :x:
5. **Understanding Explicit Arithmetic Word Problems and Explicit Plane Geometry Problems Using Syntax-Semantics Models**, IALP 2017 [[paper](https://ieeexplore.ieee.org/abstract/document/8300590)] :x:
6. **Beyond Sentential Semantic Parsing: Tackling the Math SAT with a Cascade of Tree Transducers**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1083/)] :large_blue_circle: :x:
7. **Retrieving Geometric Information from Images: The Case of Hand-Drawn Diagrams**, KDD 2017 [[paper](https://link.springer.com/article/10.1007/s10618-017-0494-1)] :x:
8. **Understanding Plane Geometry Problems by Integrating Relations Extracted from Text and Diagram**, PSIVT 2017 [[paper](https://link.springer.com/chapter/10.1007/978-3-319-75786-5_30)] :x:
9. **Automatic Assessment of Student Answers for Geometric Theorem Proving Questions**, MERCon 2017 [[paper](https://ieeexplore.ieee.org/abstract/document/7980520/)] :x:

### 2018

1. **Automatic Understanding and Formalization of Natural Language Geometry Problems Using Syntax-Semantics Models**, IJICIC 2018 [[paper](https://www.researchgate.net/publication/322939354_Automatic_understanding_and_formalization_of_natural_language_geometry_problems_using_syntax-semantics_models)] :x:
2. **Extending a Parser to Distant Domains Using a Few Dozen Partially Annotated Examples**, ACL 2018 [[paper](https://aclanthology.org/P18-1110/)]

### 2019

1. **A Sharing Framework for Solving Explicit Arithmetic Word Problems and Proving Plane Geometry Theorems**, IJPRAI 2019 [[paper](https://www.worldscientific.com/doi/abs/10.1142/S0218001419400056)] :x:
2. **Discourse in Multimedia: A Case Study in Extracting Geometry Knowledge from Textbooks**, CL 2019 [[paper](https://aclanthology.org/J19-4002/)] :x:
3. **Automatically Proving Plane Geometry Theorems Stated by Text and Diagram**, IJPRAI 2019 [[paper](https://www.worldscientific.com/doi/abs/10.1142/S0218001419400032)] :x:
4. **Automatic Understanding and Formalization of Plane Geometry Proving Problems in Natural Language: A Supervised Approach**, IJAIT 2019 [[paper](https://www.worldscientific.com/doi/abs/10.1142/S0218213019400037)] :x:
5. **A Neural Semantic Parser for Math Problems Incorporating Multi-Sentence Information**, TALLIP 2019 [[paper](https://dl.acm.org/doi/abs/10.1145/3314939)] :large_blue_circle:
6. **AiFu at SemEval-2019 Task 10: A Symbolic and Sub-symbolic Integrated System for SAT Math Question Answering**, SemEval 2019 [[paper](https://aclanthology.org/S19-2154/)] :large_blue_circle:
7. **Robot for Mathematics College Entrance Examination**, ATCM 2019 [[paper](https://atcm.mathandtech.org/EP2019/invited/4382019_21719.pdf)] :large_blue_circle:
8. **SemEval-2019 Task 10: Math Question Answering**, SemEval 2019 [[paper](https://aclanthology.org/S19-2153/)] :large_blue_circle:
9. **The Gap of Semantic Parsing: A Survey on Automatic Math Word Problem Solvers**, TPAMI 2019 [[paper](https://library.oapen.org/bitstream/handle/20.500.12657/61269/978-3-031-09687-7.pdf?sequence=1#page=246)] :large_blue_circle: :x:
10. **ProblemSolver at SemEval-2019 Task 10: Sequence-to-Sequence Learning and Expression Trees**, SemEval 2019 [[paper](https://aclanthology.org/S19-2227/)] :large_blue_circle:

### 2020

1. **Two-step Memory Networks for Deep Semantic Parsing of Geometry Word Problems**, SOFSEM 2020 [[paper](https://dl.acm.org/doi/abs/10.1007/978-3-030-38919-2_57)]
2. **A Novel Geometric Information Retrieval Tool for Images of Geometric Diagrams**, ICISE-IE 2020 [[paper](https://ieeexplore.ieee.org/abstract/document/9418805)]
3. **Applied Aspects of the Integrated Problem Solving System with Natural Language Interface**, Inforino 2020 [[paper](https://ieeexplore.ieee.org/abstract/document/9111841/)] :x:
4. **Design an Intelligent Problem Solver in Geometry based on Knowledge Model of Relations**, Engineering Letters 2020 [[paper](https://www.engineeringletters.com/issues_v28/issue_4/EL_28_4_17.pdf)] :x:
5. **Ontology-Controlled Geometric Solver**, RCAI 2020 [[paper](https://link.springer.com/chapter/10.1007/978-3-030-59535-7_19)] :x:
6. **2D Geometric Shapes Dataset – For Machine Learning and Pattern Recognition**, Data in Brief 2020 [[paper](https://www.sciencedirect.com/science/article/pii/S2352340920309847)]

### 2021

1. **Inter-GPS: Interpretable Geometry Problem Solving with Formal Language and Symbolic Reasoning**, ACL 2021 [[paper](https://aclanthology.org/2021.acl-long.528/)]
2. **GeoRE: A Relation Extraction Dataset for Chinese Geometry Problems**, NeurIPS 2021 MATHAI4ED Workshop [[paper](https://mathai4ed.github.io/papers/papers/paper_6.pdf)]
3. **GeoQA: A Geometric Question Answering Benchmark Towards Multimodal Numerical Reasoning**, Findings of ACL 2021 [[paper](https://aclanthology.org/2021.findings-acl.46)]
4. **Semantic Parsing of Geometry Statements Using Supervised Machine Learning on Synthetic Data**, NatFoM 2021 CICM Workshop [[paper](https://hal.science/hal-03327994/document)]
5. **Learning to Solve Geometric Construction Problems from Images**, CICM 2021 [[paper](https://link.springer.com/chapter/10.1007/978-3-030-81097-9_14)] :small_red_triangle:
6. **Automated Generation of Illustrations for Synthetic Geometry Proofs**, ADG 2021 [[paper](https://arxiv.org/abs/2201.00540)] :small_red_triangle: :x:
7. **Solving Solid Geometric Calculation Problems in Text**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678751)] :x:
8. **Automated Discovery of Geometrical Theorems in GeoGebra**, ThEdu 2021 [[paper](https://arxiv.org/abs/2202.04627)] :x:
9. **Automatically Building Diagrams for Olympiad Geometry Problems**, CADE 2021 [[paper](https://dl.acm.org/doi/abs/10.1007/978-3-030-79876-5_33)] :small_red_triangle: :x:
10. **Linguistic Processor Integration for Solving Planimetric Problems**, IJCINI 2021 [[paper](https://www.igi-global.com/article/linguistic-processor-integration-for-solving-planimetric-problems/274062)] :x:
11. **A Paradigm of Diagram Understanding in Problem Solving**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678637)] :x:
12. **Sequence to General Tree Knowledge-Guided Geometry Word Problem Solving**, ACL-IJCNLP 2021 [[paper](https://aclanthology.org/2021.acl-short.121/)]
13. **Proving Geometric Problem by Adding Auxiliary Lines-Based on Hypothetical Test**, AIET 2021 [[paper](https://link.springer.com/chapter/10.1007/978-981-16-7527-0_12)] :x:
14. **Solving Shaded Area Problems by Constructing Equations**, AIET 2021 [[paper](https://link.springer.com/chapter/10.1007/978-981-16-7527-0_8)] :x:
15. **Cognitive Patterns for Semantic Presentation of Natural-Language Descriptions of Well-Formalizable Problems**, RCAI 2021 [[paper](https://link.springer.com/chapter/10.1007/978-3-030-86855-0_22)] :x:
16. **Measuring Mathematical Problem Solving With the MATH Dataset**, NeurIPS 2021 [[paper](https://datasets-benchmarks-proceedings.neurips.cc/paper_files/paper/2021/file/be83ab3ecd0db773eb2dc1b0a17836a1-Paper-round2.pdf)] :large_blue_circle:

### 2022

1. **A Graph Convolutional Network Feature Learning Framework for Interpretable Geometry Problem Solving**, IEIR 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/10050084)]
2. **An Augmented Benchmark Dataset for Geometric Question Answering through Dual Parallel Text Encoding**, COLING 2022 [[paper](https://aclanthology.org/2022.coling-1.130/)]
3. **Plane Geometry Diagram Parsing**, IJCAI 2022 [[paper](https://www.ijcai.org/proceedings/2022/228)]
4. **Learning to Understand Plane Geometry Diagram**, NeurIPS 2022 MATH-AI Workshop [[paper](https://mathai2022.github.io/papers/6.pdf)]
5. **PGDP5K: A Diagram Parsing Dataset for Plane Geometry Problems**, ICPR 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/9956397)]
6. **UniGeo: Unifying Geometry Logical Reasoning via Reformulating Mathematical Expression**, EMNLP 2022 [[paper](https://aclanthology.org/2022.emnlp-main.218/)]
7. **A Novel Geometry Problem Understanding Method based on Uniform Vectorized Syntax-Semantics Model**, IEIR 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/10050038)]
8. **Geoclidean: Few-Shot Generalization in Euclidean Geometry**, NeurIPS 2022 [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/feb34ce77fc8b94c85d12e608b23ce67-Abstract-Datasets_and_Benchmarks.html)]
9. **A Method for Expanding Predicates and Rules in Automated Geometry Reasoning System**, Mathematics 2022 [[paper](https://www.mdpi.com/2227-7390/10/7/1177)] :x:
10. **Research on Geometry Problem Text Understanding Based on Bidirectional LSTM-CRF**, ICDH 2022 [[paper](https://ieeexplore.ieee.org/abstract/document/9978458)]
11. **Synthetic Data Generator for Solving Korean Arithmetic Word Problem**, Mathematics 2022 [[paper](https://www.mdpi.com/2227-7390/10/19/3525)] :large_blue_circle:
12. **Usage of Stacked Long Short-Term Memory for Recognition of 3D Analytic Geometry Elements**, ICAART 2022 [[paper](https://www.scitepress.org/Papers/2022/108989/108989.pdf)]
13. **Complex Modeling of Inductive and Deductive Reasoning by the Example of a Planimetric Problem Solver**, IITI 2022 [[paper](https://link.springer.com/chapter/10.1007/978-3-031-19620-1_43)] :x:
14. **Natural Language Processing and Functioning Ontological Solver with Visualization in an Integrated System**, IntelliSys 2022 [[paper](https://link.springer.com/chapter/10.1007/978-3-031-16078-3_46)] :x:
15. **Beyond the Imitation Game: Quantifying and Extrapolating the Capabilities of Language Models**, TMLR 2022 [[paper](https://iris.uniroma1.it/handle/11573/1724128)] :large_blue_circle:
16. **Deep Learning in Automatic Math Word Problem Solvers**, AI in Learning: Designing the Future 2022 [[article](https://library.oapen.org/bitstream/handle/20.500.12657/61269/978-3-031-09687-7.pdf?sequence=1#page=246)] :large_blue_circle:
17. **Evolution of Automated Deduction and Dynamic Constructions in Geometry**, Mathematics Education in the Age of Artificial Intelligence: How Artificial Intelligence can Serve Mathematical Human Learning 2022 [[article](https://link.springer.com/chapter/10.1007/978-3-030-86909-0_1)] :x:
18. **Supervised Learning Use to Acquire Knowledge from 2D Analytic Geometry Problems**, ACIIDS 2022 [[paper](https://link.springer.com/chapter/10.1007/978-981-19-8234-7_15)] :x:
19. **NUMGLUE: A Suite of Fundamental yet Challenging Mathematical Reasoning Tasks**, ACL 2022 [[paper](https://aclanthology.org/2022.acl-long.246/)] :large_blue_circle:
20. **Lila: A Unified Benchmark for Mathematical Reasoning**, EMNLP 2022 [[paper](https://aclanthology.org/2022.emnlp-main.392/)] :large_blue_circle:

### 2023

1. **EuclidNet: Deep Visual Reasoning for Constructible Problems in Geometry**, AIML 2023 [[paper](https://arxiv.org/abs/2301.13007)] :small_red_triangle:
2. **Solving Geometry Problems via Feature Learning and Contrastive Learning of Multimodal Data**, CMES 2023 [[paper](https://openurl.ebsco.com/EPDB%3Agcd%3A9%3A20307273/detailv2?sid=ebsco%3Aplink%3Ascholar&id=ebsco%3Agcd%3A161884174&crl=c&link_origin=scholar.google.com)]
3. **A Deep Reinforcement Learning Agent for Geometry Online Tutoring**, KAIS 2023 [[paper](https://link.springer.com/article/10.1007/s10115-022-01804-3)]
4. **GeoDRL: A Self-Learning Framework for Geometry Problem Solving using Reinforcement Learning in Deductive Reasoning**, ACL 2023 [[paper](https://aclanthology.org/2023.findings-acl.850/)]
5. **Solving Algebraic Problems with Geometry Diagrams Using Syntax-Semantics Diagram Understanding**, Computers, Materials & Continua 2023 [[paper](https://www.researchgate.net/profile/Litian-Huang/publication/375217917_Solving_Algebraic_Problems_with_Geometry_Diagrams_Using_Syntax-Semantics_Diagram_Understanding/links/654715da3fa26f66f4d60625/Solving-Algebraic-Problems-with-Geometry-Diagrams-Using-Syntax-Semantics-Diagram-Understanding.pdf)] :x:
6. **A Multi-Modal Neural Geometric Solver with Textual Clauses Parsed from Diagram**, IJCAI 2023 [[paper](https://www.ijcai.org/proceedings/2023/0376)]
7. **UniMath: A Foundational and Multimodal Mathematical Reasoner**, EMNLP 2023 [[paper](https://aclanthology.org/2023.emnlp-main.440/)] :large_blue_circle:
8. **Geometry Problem Solving Based on Counter-factual Evolutionary Reasoning**, CASE 2023 [[paper](https://scholar.googleusercontent.com/scholar.bib?q=info:886PxuxR1JUJ:scholar.google.com/&output=citation&scisdr=ClEqZRNsEMPsmsftMLY:AFWwaeYAAAAAZ3_rKLazJo3qQt7lUpGqpZbgTnM&scisig=AFWwaeYAAAAAZ3_rKO4RO1QaJNkkTXC9mGtJJJQ&scisf=4&ct=citation&cd=-1&hl=zh-CN)]
9. **Interpretable Geometry Problem Solving Using Improved RetinaNet and Graph Convolutional Network**, Electronics 2023 [[paper](https://www.mdpi.com/2079-9292/12/22/4578)]
10. **A Symbolic Characters Aware Model for Solving Geometry Problems**, MM 2023 [[paper](https://dl.acm.org/doi/abs/10.1145/3581783.3612570/)]
11. **FormalGeo: An Extensible Formalized Framework for Olympiad Geometric Problem Solving**, arXiv:2310.18021 [[paper](https://arxiv.org/abs/2310.18021)] :x:
12. **A Precise Text-to-Diagram Generation Method for Elementary Geometry**, ICCWAMTIP 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10387090)] :small_red_triangle:
13. **The Geometric Neural Solution Combined with Text Diagram Parsing**, IEIR 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10391229)]
14. **SUFFI-GPSC: Sufficient Geometry Problem Solution Checking with Symbolic Computation and Logical Reasoning**, ICCWAMTIP 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10387025/)]
15. **Extracting structured information from the textual description of geometry word problems**, NLPIR 2023 [[paper](https://dl.acm.org/doi/abs/10.1145/3639233.3639255)] :x:
16. **Conic10K: A Challenging Math Problem Understanding and Reasoning Dataset**, Findings of EMNLP 2023 [[paper](https://aclanthology.org/2023.findings-emnlp.427/)]
17. **Automated Evaluation of Student Answers for Geometric Questions Based on the Theorem 'Angles on a Straight Line Add to 180±'**, SLAAI-ICAI 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10365025/)]
18. **Estimating Answer Strategies using Online Handwritten Data: A Study using Geometry Problems**, ICETC 2023 [[paper](https://dl.acm.org/doi/abs/10.1145/3629296.3629347)]
19. **It Ain’t Over: A Multi-Aspect Diverse Math Word Problem Dataset**, EMNLP 2023 [[paper](https://aclanthology.org/2023.emnlp-main.927/)] :large_blue_circle:
20. **Visual Amplification of Geometry Problems: A Method for Synchronized Highlighting in Text and Diagrams**, IEIR 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10391250)]
21. **Systematic Literature Review: Application of Dynamic Geometry Software to Improve Mathematical Problem-solving Skills**, JMPM 2023 [[paper](https://mathline.unwir.ac.id/index.php/Mathline/article/view/458)] :x:
22. **Challenging BIG-Bench Tasks and Whether Chain-of-Thought Can Solve Them**, Findings of ACL 2023 [[paper](https://aclanthology.org/2023.findings-acl.824/)]
23. **M3exam: A Multilingual, Multimodal, Multilevel Benchmark for Examining Large Language Models**, NeurIPS 2023 [[paper](https://proceedings.neurips.cc/paper_files/paper/2023/hash/117c5c8622b0d539f74f6d1fb082a2e9-Abstract-Datasets_and_Benchmarks.html)] :large_blue_circle:
24. **TheoremQA: A Theorem-driven Question Answering Dataset**, EMNLP 2023 [[paper](https://aclanthology.org/2023.emnlp-main.489/)] :large_blue_circle:
25. **CREATOR: Tool Creation for Disentangling Abstract and Concrete Reasoning of Large Language Models**, Findings of EMNLP 2023 [[paper](https://aclanthology.org/2023.findings-emnlp.462/)] :large_blue_circle:
26. **Cumulative Reasoning with Large Language Models**, arXiv:2308.04371 [[paper](https://arxiv.org/abs/2308.04371)] :large_blue_circle:
27. **Plan, Verify and Switch: Integrated Reasoning with Diverse X-of-Thoughts**, EMNLP 2023 [[paper](https://aclanthology.org/2023.emnlp-main.169/)] :large_blue_circle:
28. **Adapting Large Language Models for Education: Foundational Capabilities, Potentials, and Challenges**, arXiv:2401.08664 [[paper](https://arxiv.org/abs/2401.08664)] :large_blue_circle:
29. **A Survey of Deep Learning for Mathematical Reasoning**, ACL 2023 [[paper](https://aclanthology.org/2023.acl-long.817/)] :large_blue_circle:
30. **Systematic Literature Review: Application of Dynamic Geometry Software to Improve Mathematical Problem-Solving Skills**, Mathline: Jurnal Matematika Dan Pendidikan Matematika 2023 [[paper](https://mathline.unwir.ac.id/index.php/Mathline/article/view/458)] :x:
31. **A Survey of Reasoning with Foundation Models**, arXiv:2312.11562 [[paper](https://arxiv.org/abs/2312.11562)] :large_blue_circle:
32. **A Survey of Reasoning with Foundation Models: Concepts, Methodologies, and Outlook**, ACM Comput. Surv. 2023 [[paper](https://dl.acm.org/doi/full/10.1145/3729218)] :large_blue_circle:
33. **Geometry Problem Solving Based on Deep Learning**, CSMIS 2023 [[paper](https://ieeexplore.ieee.org/abstract/document/10548031/)]

### 2024

1. **LANS: A Layout-Aware Neural Solver for Plane Geometry Problem**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.153/)]
2. **GeomVerse: A Systematic Evaluation of Large Models for Geometric Reasoning**, ICML 2024 AI4MATH Workshop [[paper](https://openreview.net/forum?id=1AUbiBrOF1)]
3. **Solving Olympiad Geometry Without Human Demonstrations**, Nature 2024 [[paper](https://www.nature.com/articles/s41586-023-06747-5)]
4. **GAPS: Geometry-Aware Problem Solver**, arXiv:2401.16287 [[paper](https://arxiv.org/abs/2401.16287)]
5. **E-GPS: Explainable Geometry Problem Solving via Top-Down Solver and Bottom-Up Generator**, CVPR 2024 [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wu_E-GPS_Explainable_Geometry_Problem_Solving_via_Top-Down_Solver_and_Bottom-Up_CVPR_2024_paper.html)]
6. **Beyond Lines and Circles Unveiling the Geometric Reasoning Gap in Large Language Models**, Findings of EMNLP 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.360/)] :small_red_triangle:
7. **FGeo-TP: A Language Model-Enhanced Solver for Geometry Problems**, Symmetry 2024 [[paper](https://www.mdpi.com/2073-8994/16/4/421)]
8. **FGeo-DRL: Deductive Reasoning for Geometric Problems Through Deep Reinforcement Learning**, Symmetry 2024 [[paper](https://www.mdpi.com/2073-8994/16/4/437)]
9. **FGeo-SSS: A Search-Based Symbolic Solver for Human-Like Automated Geometric Reasoning**, Symmetry 2024 [[paper](https://www.mdpi.com/2073-8994/16/4/404)] :x:
10. **FGeo-HyperGNet: Geometric Problem Solving Integrating Formal Symbolic System and Hypergraph Neural Network**, arXiv:2402.11461 [[paper](https://arxiv.org/abs/2402.11461)]
11. **OlympiadBench: A Challenging Benchmark for Promoting AGI With Olympiad-Level Bilingual Multimodal Scientific Problems**, ACL 2024 [[paper](https://aclanthology.org/2024.acl-long.211/)] :large_blue_circle:
12. **MathVista: Evaluating Mathematical Reasoning of Foundation Models in Visual Contexts**, ICLR 2024 [[paper](https://iclr.cc/virtual/2024/oral/19768)] :large_blue_circle:
13. **MathVerse: Does Your Multi-Modal LLM Truly See the Diagrams in Visual Math Problems?**, ECCV 2024 [[paper](https://dl.acm.org/doi/10.1007/978-3-031-73242-3_10)] :large_blue_circle:
14. **Measuring Multimodal Mathematical Reasoning With MATH-Vision Dataset**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/ad0edc7d5fa1a783f063646968b7315b-Abstract-Datasets_and_Benchmarks_Track.html)] :large_blue_circle:
15. **MM-MATH: Advancing Multimodal Math Evaluation With Process Evaluation and Fine-Grained Classification**, Findings of EMNLP 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.73/)] :large_blue_circle:
16. **Wu’s Method Boosts Symbolic AI to Rival Silver Medalists and AlphaGeometry to Outperform Gold Medalists at IMO Geometry**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=aKRtC45gle)]
17. **GOLD: Geometry Problem Solver With Natural Language Description**, Findings of NAACL 2024 [[paper](https://aclanthology.org/2024.findings-naacl.19/)]
18. **Learning to Solve Geometry Problems via Simulating Human Dual-Reasoning Process**, IJCAI 2024 [[paper](https://www.ijcai.org/proceedings/2024/0725.pdf)]
19. **Autoformalizing Euclidean Geometry**, ICML 2024 [[paper](https://dl.acm.org/doi/abs/10.5555/3692070.3693567)] :small_red_triangle:
20. **GeoEval: Benchmark for Evaluating LLMs and Multi-Modal Models on Geometry Problem-Solving**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.73/)]
21. **GeoGPT4V: Towards Geometric Multi-Modal Large Language Models With Geometric Image Generation**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.44/)]
22. **Figuring Figures: An Assessment of Large Language Models on Different Modalities of Math Word Problems**, ICMLT 2024 [[paper](https://dl.acm.org/doi/abs/10.1145/3674029.3674041)]
23. **Math-LLaVA: Bootstrapping Mathematical Reasoning for Multimodal Large Language Models**, EMNLP Findings 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.268/)] :large_blue_circle:
24. **We-Math: Does Your Large Multimodal Model Achieve Human-Like Mathematical Reasoning?**, arXiv:2407.01284 [[paper](https://arxiv.org/abs/2407.01284)] :large_blue_circle:
25. **Fuse, Reason and Verify: Geometry Problem Solving With Parsed Clauses From Diagram**, arXiv:2407.07327 [[paper](https://arxiv.org/abs/2407.07327)]
26. **Is Your Model Really a Good Math Reasoner? Evaluating Mathematical Reasoning With Checklist**, arXiv:2407.08733 [[paper](https://arxiv.org/abs/2407.08733)]
27. **Hologram Reasoning for Solving Algebra Problems With Geometry Diagrams**, arXiv:2408.10592 [[paper](https://arxiv.org/abs/2408.10592)]
28. **EAGLE: Elevating Geometric Reasoning Through LLM-Empowered Visual Instruction Tuning**, arXiv:2408.11397 [[paper](https://arxiv.org/abs/2408.11397)]
29. **Tangram: A Challenging Benchmark for Geometric Element Recognizing**, arXiv:2408.13854 [[paper](https://arxiv.org/abs/2408.13854)]
30. **Leveraging Two-Level Deep Learning Classifers for 2D Shape Recognition to Automatically Solve Geometry Math Word Problems**, PAA 2024 [[paper](https://link.springer.com/article/10.1007/s10044-024-01321-9)]
31. **MultiMath: Bridging Visual and Mathematical Reasoning for Large Language Models**, arXiv:2409.00147 [[paper](https://arxiv.org/abs/2409.00147)] :large_blue_circle:
32. **InfiMM-WebMath-40B: Advancing Multimodal Pre-Training for Enhanced Mathematical Reasoning**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=Twzrpa6V2o)] :large_blue_circle:
33. **MathGLM-Vision: Solving Mathematical Problems With Multi-Modal Large Language Model**, arXiv:2409.13729 [[paper](https://arxiv.org/abs/2409.13729)] :large_blue_circle:
34. **Enhancing Geometry Problem Solving With Attention Mechanism and Super-Resolution**, ICBASE 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10762589)]
35. **Automated Generation of Geometry Proof Problems Based on Point Geometry Identity**, Journal of Automated Reasoning 2024 [[paper](https://link.springer.com/article/10.1007/s10817-024-09699-1)] :x:
36. **Geo-Qwen: A Geometry Problem-Solving Method Based on Generative Large Language Models and Heuristic Reasoning**, ICCWAMTIP 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10873683)]
37. **Formal Representation and Solution of Plane Geometric Problems**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=8wDSfs1W3w)]
38. **GeoVQA: A Comprehensive Multimodal Geometry Dataset for Secondary Education**, MIPR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10707789)]
39. **Geo-LLaVA: A Large Multi-Modal Model for Solving Geometry Math Problems With Meta In-Context Learning**, LGM3A 2024 [[paper](https://dl.acm.org/doi/10.1145/3688866.3689124)]
40. **Reason-and-Execute Prompting: Enhancing Multi-Modal Large Language Models for Solving Geometry Questions**, MM 2024 [[paper](https://dl.acm.org/doi/abs/10.1145/3664647.3681484)]
41. **R-CoT: Reverse Chain-of-Thought Problem Generation for Geometric Reasoning in Large Multimodal Models**, arXiv:2410.17885 [[paper](https://arxiv.org/abs/2410.17885)]
42. **LLaVA-o1: Let Vision Language Models Reason Step-by-Step**, arXiv:2411.10440 [[paper](https://arxiv.org/abs/2411.10440)] :large_blue_circle:
43. **Vision-Language Models Can Self-Improve Reasoning via Reflection**, arXiv:2411.00855 [[paper](https://arxiv.org/abs/2411.00855)] :large_blue_circle:
44. **A Geometric Neural Solving Method Based on a Diagram Text Information Fusion Analysis**, Sci. Rep. 2024 [[paper](https://www.nature.com/articles/s41598-024-83287-6)]
45. **Slow Perception: Let's Perceive Geometric Figures Step-by-Step**, arXiv:2412.20631 [[paper](https://arxiv.org/abs/2412.20631)]
46. **Maths: Multimodal Transformer-Based Human-Readable Solver**, ICME 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10687434)]
47. **Automatic Extraction of Structured Information from Elementary Level Geometry Questions into Logic Forms**, Multimed Tools Appl 2024 [[paper](https://link.springer.com/article/10.1007/s11042-024-20463-w)]
48. **Improving Multimodal LLMs Ability in Geometry Problem Solving, Reasoning, and Multistep Scoring**, arXiv:2412.00846 [[paper](https://arxiv.org/abs/2412.00846)]
49. **Advancing Multimodal LLMs: A Focus on Geometry Problem Solving Reasoning and Sequential Scoring**, MMASIA 2024 [[paper](https://dl.acm.org/doi/full/10.1145/3696409.3700262)]
50. **Visual Sketchpad: Sketching as a Visual Chain of Thought for Multimodal Language Models**, NeurIPS 2024 [[paper](https://openreview.net/forum?id=GNSMl1P5VR)] :large_blue_circle:
51. **2D Shape Detection for Solving Geometry Word Problems**, IETE J. Res. 2024 [[paper](https://www.tandfonline.com/doi/abs/10.1080/03772063.2023.2274914)] :x:
52. **VisAidMath: Benchmarking Visual-Aided Mathematical Reasoning**, arXiv:2410.22995 [[paper](https://arxiv.org/abs/2410.22995)] :large_blue_circle:
53. **Euclid: Supercharging Multimodal LLMs With Synthetic High-Fidelity Visual Descriptions**, arXiv:2412.08737 [[paper](https://arxiv.org/abs/2412.08737)]
54. **AtomThink: A Slow Thinking Framework for Multimodal Mathematical Reasoning**, arXiv:2411.11930 [[paper](https://arxiv.org/abs/2411.11930)] :large_blue_circle:
55. **Mulberry: Empowering MLLM With o1-like Reasoning and Reflection via Collective Monte Carlo Tree Search**, arXiv:2412.18319 [[paper](https://arxiv.org/abs/2412.18319)] :large_blue_circle:
56. **What is the True Performance of Large Multimodal Models in Visual Context-Based Mathematical Reasoning? An Analysis of Multiple Datasets and Future Research Directions**, ICTC 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10827294)]
57. **GePBench: Evaluating Fundamental Geometric Perception for Multimodal Large Language Models**, arXiv:2412.21036 [[paper](https://arxiv.org/abs/2412.21036)]
58. **DrawEduMath: Evaluating Vision Language Models with Expert-Annotated Students’ Hand-Drawn Math Images**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=0vQYvcinij)] :large_blue_circle:
59. **An Enhanced Relation-Flow Algorithm for Solving Number Line Problems**, IEIR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10960042)] :x:
60. **Describe-then-Reason: Improving Multimodal Mathematical Reasoning Through Visual Comprehension Training**, arXiv:2404.14604 [[paper](https://arxiv.org/abs/2404.14604)] :large_blue_circle:
61. **Enhancing LLM Reasoning via Vision-Augmented Prompting**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/328c922d068dd4ccb23cec5c64e6c7fc-Abstract-Conference.html)]
62. **Evaluating Automated Geometric Problem Solving With Formal Language Generation on Large Multimodal Models**, IEIR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10959992)]
63. **Multi-Step Chain-of-Thought in Geometry Problem Solving**, EIECS 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10800087)]
64. **VisOnlyQA: Large Vision Language Models Still Struggle With Visual Perception of Geometric Information**, arXiv:2412.00947 [[paper](https://arxiv.org/abs/2412.00947)] :large_blue_circle:
65. **CMM-Math: A Chinese Multimodal Math Dataset to Evaluate and Enhance the Mathematics Reasoning of Large Multimodal Models**, arXiv:2409.02834 [[paper](https://arxiv.org/abs/2409.02834)] :large_blue_circle:
66. **All in an Aggregated Image for In-Image Learning**, arXiv:2402.17971 [[paper](https://arxiv.org/abs/2402.17971)] :large_blue_circle:
67. **CurveML: A Benchmark for Evaluating and Training Learning-Based Methods of Classification, Recognition, and Fitting of Plane Curves**, Visual Comput 2024 [[paper](https://link.springer.com/article/10.1007/s00371-024-03292-8)]
68. **Multimodal ArXiv: A Dataset for Improving Scientific Comprehension of Large Vision-Language Models**, ACL 2024 [[paper](https://aclanthology.org/2024.acl-long.775/)] :large_blue_circle:
69. **MathScape: Evaluating MLLMs in Multimodal Math Scenarios Through a Hierarchical Benchmark**, arXiv:2408.07543 [[paper](https://arxiv.org/abs/2408.07543)] :large_blue_circle:
70. **VisScience: An Extensive Benchmark for Evaluating K12 Educational Multi-Modal Scientific Reasoning**, arXiv:2409.13730 [[paper](https://arxiv.org/abs/2409.13730)] :large_blue_circle:
71. **Progressive Multimodal Reasoning via Active Retrieval**, arXiv:2412.14835 [[paper](https://arxiv.org/abs/2412.14835)] :large_blue_circle:
72. **Decomposing Complex Visual Comprehension Into Atomic Visual Skills for Vision Language Models**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=nFU4xCyoe0)] :large_blue_circle:
73. **ReMI: A Dataset for Reasoning With Multiple Images**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/6ea56c0baacac9f7764257a43a93c90a-Abstract-Datasets_and_Benchmarks_Track.html)] :large_blue_circle:
74. **M3GIA: A Cognition-Inspired Multilingual and Multimodal General Intelligence Ability Benchmark**, arXiv:2406.05343 [[paper](https://arxiv.org/abs/2406.05343)] :large_blue_circle:
75. **Mathematical Problem Solving in Arabic: Assessing Large Language Models**, Procedia Comput. Sci. 2024 [[paper](https://www.sciencedirect.com/science/article/pii/S187705092402982X)] :large_blue_circle:
76. **M3CoT: A Novel Benchmark for Multi-Domain Multi-Step Multi-Modal Chain-of-Thought**, ACL 2024 [[paper](https://aclanthology.org/2024.acl-long.446/)] :large_blue_circle:
77. **MathOdyssey: Benchmarking Mathematical Problem-Solving Skills in Large Language Models Using Odyssey Math Data**, arXiv:2406.18321 [[paper](https://arxiv.org/abs/2406.18321)] :large_blue_circle:
78. **PutnamBench: Evaluating Neural Theorem-Provers on the Putnam Mathematical Competition**, NeurIPS 2024 [[paper](https://openreview.net/forum?id=ChKCF75Ocd)] :large_blue_circle:
79. **From Blind Solvers to Logical Thinkers: Benchmarking LLMs’ Logical Integrity on Faulty Mathematical Problems**, arXiv:2410.18921 [[paper](https://arxiv.org/abs/2410.18921)] :large_blue_circle:
80. **ConceptMath: A Bilingual Concept-wise Benchmark for Measuring Mathematical Reasoning of Large Language Models**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.407/)] :large_blue_circle:
81. **Functional Benchmarks for Robust Evaluation of Reasoning Performance, and the Reasoning Gap**, arXiv:2402.19450 [[paper](https://arxiv.org/abs/2402.19450)] :large_blue_circle:
82. **MathBench: Evaluating the Theory and Application Proficiency of LLMs with a Hierarchical Mathematics Benchmark**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.411/)] :large_blue_circle:
83. **HARP: A Challenging Human-Annotated Math Reasoning Benchmark**, arXiv:2412.08819 [[paper](https://arxiv.org/abs/2412.08819)] :large_blue_circle:
84. **Progressive-Hint Prompting Improves Reasoning in Large Language Models**, ICML 2024 AI4MATH Workshop [[paper](https://openreview.net/forum?id=UkFEs3ciz8)] :large_blue_circle:
85. **Learning to Plan by Updating Natural Language**, Findings of EMNLP 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.589/)] :large_blue_circle:
86. **Reprompting: Automated Chain-of-Thought Prompt Inference Through Gibbs Sampling**, ICML 2024 [[paper](https://proceedings.mlr.press/v235/xu24b.html)] :large_blue_circle:
87. **Skills-in-Context: Unlocking Compositionality in Large Language Models**, Findings of EMNLP 2024 [[paper](https://aclanthology.org/2024.findings-emnlp.812/)] :large_blue_circle:
88. **ToRA: A Tool-Integrated Reasoning Agent for Mathematical Problem Solving**, ICLR 2024 [[paper](https://openreview.net/forum?id=Ep0TtjVoap)] :large_blue_circle:
89. **Can Generative AI Solve Geometry Problems? Strengths and Weaknesses of LLMs for Geometric Reasoning in Spanish**, IJIMAI 2024 [[paper](https://dialnet.unirioja.es/servlet/articulo?codigo=9906100)]
90. **Explicit Memory Learning with Expectation Maximization**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.927.pdf)] :large_blue_circle:
91. **MathSensei: Mathematical Reasoning with a Tool-Augmented Large Language Model**, ICLR 2024 ME-FoMo Workshop [[paper](https://openreview.net/forum?id=YDQ6eBB4py)] :large_blue_circle:
92. **Null-Shot Prompting: Rethinking Prompting Large Language Models With Hallucination**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.740/)] :large_blue_circle:
93. **Strategyllm: Large Language Models as Strategy Generators, Executors, Optimizers, and Evaluators for Problem Solving**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/af7cc9e2366b8f8837a6ef339810277a-Abstract-Conference.html)] :large_blue_circle:
94. **BBA: Bi-Modal Behavioral Alignment for Reasoning with Large Vision-Language Models**, Findings of ACL 2024 [[paper](https://aclanthology.org/2024.findings-acl.433/)]
95. **Hint-before-Solving Prompting: Guiding LLMs to Effectively Utilize Encoded Knowledge**, arXiv:2402.14310 [[paper](https://arxiv.org/abs/2402.14310)] :large_blue_circle:
96. **MathScale: Scaling Instruction Tuning for Mathematical Reasoning**, ICML 2024 [[paper](https://proceedings.mlr.press/v235/tang24k.html)] :large_blue_circle:
97. **Learning From Correctness Without Prompting Makes LLM Efficient Reasoner**, COLM 2024 [[paper](https://openreview.net/forum?id=dcbNzhVVQj)] :large_blue_circle:
98. **MACM: Utilizing a Multi-Agent System for Condition Mining in Solving Complex Mathematical Problems**, NeurIPS 2024 [[paper](https://openreview.net/forum?id=VR2RdSxtzs)] :large_blue_circle:
99. **Divide-and-Conquer Meets Consensus: Unleashing the Power of Functions in Code Generation**, NeurIPS 2024 [[paper](https://openreview.net/forum?id=cFqAANINgW)] :large_blue_circle:
100. **Deliberate Reasoning for LLMs as Structure-Aware Planning with Accurate World Model**, arXiv:2410.03136 [[paper](https://arxiv.org/abs/2410.03136)] :large_blue_circle:
101. **Give me a Hint: Can LLMs Take a Hint to Solve Math Problems?**, NeurIPS 2024 MATH-AI Workshop [[paper](https://openreview.net/forum?id=eeZG97VjYa)] :large_blue_circle:
102. **MC-NEST--Enhancing Mathematical Reasoning in Large Language Models with a Monte Carlo Nash Equilibrium Self-Refine Tree**, arXiv:2411.15645 [[paper](https://arxiv.org/abs/2411.15645)] :large_blue_circle:
103. **DART-Math: Difficulty-Aware Rejection Tuning for Mathematical Problem-Solving**, NeurIPS 2024 [[paper](https://proceedings.neurips.cc/paper_files/paper/2024/hash/0ef1afa0daa888d695dcd5e9513bafa3-Abstract-Conference.html)] :large_blue_circle:
104. **Offline Training of Language Model Agents with Functions as Learnable Weights**, ICML 2024 [[paper](https://proceedings.mlr.press/v235/zhang24cd.html)] :large_blue_circle:
105. **UTMath: Math Evaluation with Unit Test via Reasoning-to-Coding Thoughts**, arXiv:2411.07240 [[paper](https://arxiv.org/abs/2411.07240)] :large_blue_circle:
106. **MultiLingPoT: Enhancing Mathematical Reasoning with Multilingual Program Fine-tuning**, arXiv:2412.12609 [[paper](https://arxiv.org/abs/2412.12609)] :large_blue_circle:
107. **System-2 Mathematical Reasoning via Enriched Instruction Tuning**, arXiv:2412.16964 [[paper](https://arxiv.org/abs/2412.16964)] :large_blue_circle:
108. **Beyond Captioning: Task-Specific Prompting for Improved VLM Performance in Mathematical Reasoning**, arXiv:2410.05928 [[paper](https://arxiv.org/abs/2410.05928)]
109. **Data for Mathematical Copilots: Better Ways of Presenting Proofs for Machine Learning**, arXiv:2412.15184 [[paper](https://arxiv.org/abs/2412.15184)] :large_blue_circle:
110. **Adapting Large Language Models for Education: Foundational Capabilities, Potentials, and Challenges**, arXiv:2401.08664 [[paper](https://arxiv.org/abs/2401.08664)] :large_blue_circle:
111. **Large Language Models for Mathematical Reasoning: Progresses and Challenges**, EACL 2024 [[paper](https://aclanthology.org/2024.eacl-srw.17/)] :large_blue_circle:
112. **A Survey on Deep Learning for Theorem Proving**, COLM 2024 [[paper](https://openreview.net/forum?id=zlw6AHwukB)] :large_blue_circle:
113. **A Comprehensive Survey of Scientific Large Language Models and Their Applications in Scientific Discovery**, EMNLP 2024 [[paper](https://aclanthology.org/2024.emnlp-main.498/)] :large_blue_circle:
114. **Towards Robust Automated Math Problem Solving: A Survey of Statistical and Deep Learning Approaches**, Evol. Intell. 2024 [[paper](https://link.springer.com/article/10.1007/s12065-024-00957-0)] :large_blue_circle:
115. **Proposing and Solving Olympiad Geometry with Guided Tree Search**, arXiv:2412.10673 [[paper](https://arxiv.org/abs/2412.10673)]

### 2025

1. **AutoGeo: Automating Geometric Image Dataset Creation for Enhanced Geometry Understanding**, IEEE Trans. Multimedia 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10960701/)]
2. **SANS: Spatial-Aware Neural Solver for Plane Geometry Problem**, ICPR 2025 [[paper](https://link.springer.com/chapter/10.1007/978-3-031-78119-3_13)]
3. **G-LLaVA: Solving Geometric Problem with Multi-Modal Large Language Model**, ICLR 2025 [[paper](https://openreview.net/forum?id=px1674Wp3C&noteId=H99kD23um8)]
4. **MAVIS: Mathematical Visual Instruction Tuning with an Automatic Data Engine**, ICLR 2025 [[paper](https://openreview.net/forum?id=MnJzJ2gvuf)]
5. **DynaMath: A Dynamic Visual Benchmark for Evaluating Mathematical Reasoning Robustness of Vision Language Models**, ICLR 2025 [[paper](https://openreview.net/forum?id=VOAMTA8jKu)] :large_blue_circle:
6. **Do Large Language Models Truly Understand Geometric Structures?**, ICLR 2025 [[paper](https://openreview.net/forum?id=FjQOXenaXK)]
7. **GeoX: Geometric Problem Solving Through Unified Formalized Vision-Language Pre-Training**, ICLR 2025 [[paper](https://openreview.net/forum?id=6RiBl5sCDF)]
8. **Diagram Formalization Enhanced Multi-Modal Geometry Problem Solver**, ICASSP 2025 [[paper](https://ieeexplore.ieee.org/abstract/document/10889286/)]
9. **A Knowledge and Semantic Fusion Method for Automatic Geometry Problem Understanding**, Appl. Sci. 2025 [[paper](https://www.mdpi.com/2076-3417/15/7/3857)]
10. **ElementaryCQT: A New Dataset and Its Deep Learning Analysis for 2D Geometric Shape Recognition**, SN Comput. Sci. 2025 [[paper](https://link.springer.com/article/10.1007/s42979-024-03521-w)]
11. **Exploration of Formalization Techniques for Geometric Entities in Planar Geometry Proposition Texts**, JAIP 2025 [[paper](https://www.clausiuspress.com/assets/default/article/2025/02/27/article_1740641608.pdf)]
12. **FGeo-Parser: Autoformalization and Solution of Plane Geometric Problems**, Symmetry 2025 [[paper](https://www.mdpi.com/2073-8994/17/1/8)]
13. **GeoDANO: Geometric VLM with Domain Agnostic Vision Encoder**, arXiv:2502.11360 [[paper](https://arxiv.org/abs/2502.11360)]
14. **Math-PUMA: Progressive Upward Multimodal Alignment to Enhance Mathematical Reasoning**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34815)] :large_blue_circle:
15. **Multimodal Large Language Models for High School Mathematical Reasoning: Impact of Input Modality and Artifacts**, Authorea Preprints 2025 [[paper](https://www.techrxiv.org/doi/full/10.36227/techrxiv.174197904.42332272)] :large_blue_circle:
16. **URSA: Understanding and Verifying Chain-of-Thought Reasoning in Multimodal Mathematics**, arXiv:2501.04686 [[paper](https://arxiv.org/abs/2501.04686)] :large_blue_circle:
17. **Vision-R1: Incentivizing Reasoning Capability in Multimodal Large Language Models**, arXiv:2503.06749 [[paper](https://arxiv.org/abs/2503.06749)] :large_blue_circle:
18. **VISTA: Visual Integrated System for Tailored Automation in Math Problem Generation Using LLM**, PMLR 2025 [[paper](https://proceedings.mlr.press/v264/lee25b)]
19. **LMM-R1: Empowering 3B LMMs with Strong Reasoning Abilities Through Two-Stage Rule-Based RL**, arXiv:2503.07536 [[paper](https://arxiv.org/abs/2503.07536)]
20. **VisualPRM: An Effective Process Reward Model for Multimodal Reasoning**, arXiv:2503.10291 [[paper](https://arxiv.org/abs/2503.10291)] :large_blue_circle:
21. **VisualWebInstruct: Scaling up Multimodal Instruction Data through Web Search**, arXiv:2503.10582 [[paper](https://arxiv.org/abs/2503.10582)] :large_blue_circle:
22. **VisNumBench: Evaluating Number Sense of Multimodal Large Language Models**, arXiv:2503.14939 [[paper](https://arxiv.org/abs/2503.14939)] :large_blue_circle:
23. **Interactive Sketchpad: A Multimodal Tutoring System for Collaborative, Visual Problem-Solving**, arXiv:2503.16434 [[paper](https://arxiv.org/abs/2503.16434)] :large_blue_circle:
24. **OpenVLThinker: An Early Exploration to Complex Vision-Language Reasoning via Iterative Self-Improvement**, arXiv:2503.17352 [[paper](https://arxiv.org/abs/2503.17352)] :large_blue_circle:
25. **MathAgent: Leveraging a Mixture-of-Math-Agent Framework for Real-World Multimodal Mathematical Error Detection**, arXiv:2503.18132 [[paper](https://arxiv.org/abs/2503.18132)] :large_blue_circle:
26. **Reason-RFT: Reinforcement Fine-Tuning for Visual Reasoning**, arXiv:2503.20752 [[paper](https://arxiv.org/abs/2503.20752)] :large_blue_circle:
27. **VILBENCH: A Suite for Vision-Language Process Reward Modeling**, arXiv:2503.20271 [[paper](https://arxiv.org/abs/2503.20271)] :large_blue_circle:
28. **SoTA with Less: MCTS-Guided Sample Selection for Data-Efficient Visual Reasoning Self-Improvement**, arXiv:2504.07934 [[paper](https://arxiv.org/abs/2504.07934)] :large_blue_circle:
29. **VisuoThink: Empowering LVLM Reasoning with Multimodal Tree Search**, arXiv:2504.09130 [[paper](https://arxiv.org/abs/2504.09130)]
30. **GNS: Solving Plane Geometry Problems by Neural-Symbolic Reasoning with Multi-Modal LLMs**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34679)]
31. **Enhancing the Geometric Problem-Solving Ability of Multimodal LLMs via Symbolic-Neural Integration**, arXiv:2504.12773 [[paper](https://arxiv.org/abs/2504.12773)]
32. **GeoSense: Evaluating Identification and Application of Geometric Principles in Multimodal Reasoning**, arXiv:2504.12597 [[paper](https://arxiv.org/abs/2504.12597)]
33. **CoMT: A Novel Benchmark for Chain of Multi-modal Thought on Large Vision-Language Models**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34538)] :large_blue_circle:
34. **Gold-medalist Performance in Solving Olympiad Geometry with AlphaGeometry2**, arXiv:2502.03544 [[paper](https://arxiv.org/abs/2502.03544)]
35. **Feynman: Knowledge-Infused Diagramming Agent for Scaling Visual Reasoning Data**, openreview 2025 [[paper](https://openreview.net/forum?id=jNmsuEE4Gf)] :large_blue_circle:
36. **GeoUni: A Unified Model for Generating Geometry Diagrams, Problems and Problem Solutions**, arXiv:2504.10146 [[paper](https://arxiv.org/pdf/2504.10146)]
37. **MagicGeo: Training-Free Text-Guided Geometric Diagram Generation**, arXiv:2502.13855 [[paper](https://arxiv.org/abs/2502.13855)] :small_red_triangle:
38. **MATHGLANCE: Multimodal Large Language Models Do Not Know Where to Look in Mathematical Diagrams**, arXiv:2503.20745 [[paper](https://arxiv.org/abs/2503.20745)]
39. **Virgo: A Preliminary Exploration on Reproducing o1-like MLLM**, arXiv:2501.01904 [[paper](https://arxiv.org/abs/2501.01904)] :large_blue_circle:
40. **Open Eyes, Then Reason: Fine-grained Visual Mathematical Understanding in MLLMs**, arXiv:2501.06430 [[paper](https://arxiv.org/abs/2501.06430)]
41. **MV-MATH: Evaluating Multimodal Math Reasoning in Multi-Visual Contexts**, arXiv:2502.20808 [[paper](https://arxiv.org/abs/2502.20808)] :large_blue_circle:
42. **Pi-GPS: Enhancing Geometry Problem Solving by Unleashing the Power of Diagrammatic Information**, arXiv:2503.05543 [[paper](https://arxiv.org/abs/2503.05543)]
43. **MathFlow: Enhancing the Perceptual Flow of MLLMs for Visual Mathematical Problems**, arXiv:2503.16549 [[paper](https://arxiv.org/abs/2503.16549)] :large_blue_circle:
44. **RedStar: Does Scaling Long-CoT Data Unlock Better Slow-Reasoning Systems?**, arXiv:2501.11284 [[paper](https://arxiv.org/abs/2501.11284)]
45. **Can Atomic Step Decomposition Enhance the Self-structured Reasoning of Multimodal Large Models?**, arXiv:2503.06252 [[paper](https://arxiv.org/abs/2503.06252)] :large_blue_circle:
46. **GeoCoder: Solving Geometry Problems by Generating Modular Code through Vision-Language Models**, Findings of NAACL 2025 [[paper](https://aclanthology.org/2025.findings-naacl.410.pdf)]
47. **DrawEduMath: Evaluating Vision Language Models with Expert-Annotated Students’ Hand-Drawn Math Images**, NAACL 2025 [[paper](https://openreview.net/forum?id=0vQYvcinij)] :large_blue_circle:
48. **Benchmarking Multimodal Mathematical Reasoning with Explicit Visual Dependency**, arXiv:2504.18589 [[paper](https://arxiv.org/abs/2504.18589)] :large_blue_circle:
49. **CogCom: A Visual Language Model with Chain-of-Manipulations Reasoning**, ICLR 2025 [[paper](https://openreview.net/forum?id=Fg0eo2AkST)] :large_blue_circle:
50. **CMMaTH: A Chinese Multi-modal Math Skill Evaluation Benchmark for Foundation Models**, COLING 2025 [[paper](https://aclanthology.org/2025.coling-main.184/)] :large_blue_circle:
51. **Boosting Multimodal Reasoning with MCTS-Automated Structured Thinking**, arXiv:2502.02339 [[paper](https://arxiv.org/abs/2502.02339)] :large_blue_circle:
52. **Forgotten Polygons: Multimodal Large Language Models are Shape-Blind**, arXiv:2502.15969 [[paper](https://arxiv.org/abs/2502.15969)]
53. **Boosting the Generalization and Reasoning of Vision Language Models with Curriculum Reinforcement Learning**, arXiv:2503.07065 [[paper](https://arxiv.org/abs/2502.15969)] :large_blue_circle:
54. **Boosting MLLM Reasoning with Text-Debiased Hint-GRPO**, arXiv:2503.23905 [[paper](https://arxiv.org/abs/2503.23905)]
55. **PRM-BAS: Enhancing Multimodal Reasoning through PRM-guided Beam Annealing Search**, arXiv:2504.10222 [[paper](https://arxiv.org/abs/2504.10222)] :large_blue_circle:
56. **SFT or RL? An Early Investigation into Training R1-Like Reasoning Large Vision-Language Models**, arXiv:2504.11468 [[paper](https://arxiv.org/abs/2504.11468)] :large_blue_circle:
57. **NoisyRollout: Reinforcing Visual Reasoning with Data Augmentation**, arXiv:2504.13055 [[paper](https://arxiv.org/abs/2504.13055)] :large_blue_circle:
58. **TrustGeoGen: Scalable and Formal-Verified Data Engine for Trustworthy Multi-modal Geometric Problem Solving**, arXiv:2504.15780 [[paper](https://arxiv.org/abs/2504.15780)]
59. **On The Potential of Using Generative Artificial Intelligence for Geometry Educational Activities**, hal 2025 [[paper](https://hal.science/hal-05022472/)]
60. **Omni-MATH: A Universal Olympiad Level Mathematic Benchmark for Large Language Models**, ICLR 2025 [[paper](https://openreview.net/forum?id=yaqPf0KAlN)] :large_blue_circle:
61. **MathConstruct: Challenging LLM Reasoning with Constructive Proofs**, ICLR 2025 VerifAI Workshop [[paper](https://openreview.net/forum?id=nHW2tiGMrb)] :large_blue_circle:
62. **TMATH: A Dataset for Evaluating Large Language Models in Generating Educational Hints for Math Word Problems**, COLING 2025 [[paper](https://aclanthology.org/2025.coling-main.340/)] :large_blue_circle:
63. **MathClean: A Benchmark for Synthetic Mathematical Data Cleaning**, arXiv:2502.19508 [[paper](https://arxiv.org/abs/2502.19058)] :large_blue_circle:
64. **Challenging the Boundaries of Reasoning: An Olympiad-Level Math Benchmark for Large Language Models**, arXiv:2503.21380 [[paper](https://arxiv.org/abs/2503.21380)] :large_blue_circle:
65. **Recitation over Reasoning: How Cutting-Edge Language Models Can Fail on Elementary School-Level Reasoning Problems?**, arXiv:2504.00509 [[paper](https://arxiv.org/abs/2504.00509)] :large_blue_circle:
66. **PolyMath: Evaluating Mathematical Reasoning in Multilingual Contexts**, arXiv:2504.18428 [[paper](https://arxiv.org/abs/2504.18428)] :large_blue_circle:
67. **LLMs Are Not Intelligent Thinkers: Introducing Mathematical Topic Tree Benchmark for Comprehensive Evaluation of LLMs**, NAACL 2025 [[paper](https://aclanthology.org/2025.naacl-long.161/)] :large_blue_circle:
68. **Who's the MVP? A Game-Theoretic Evaluation Benchmark for Modular Attribution in LLM Agents**, arXiv:2502.00510 [[paper](https://arxiv.org/abs/2502.00510)] :large_blue_circle:
69. **MATH-Perturb: Benchmarking LLMs' Math Reasoning Abilities against Hard Perturbations**, ICLR 2025 LLM Reason&Plan Workshop [[paper](https://openreview.net/forum?id=M8OLGgYK7e&referrer=%5Bthe%20profile%20of%20Xinyun%20Chen%5D%28%2Fprofile%3Fid%3D~Xinyun_Chen1%29)] :large_blue_circle:
70. **Generative Verifiers: Reward Modeling as Next-Token Prediction**, ICLR 2025 [[paper](https://openreview.net/forum?id=Ccwp4tFEtE)] :large_blue_circle:
71. **Breaking Mental Set to Improve Reasoning through Diverse Multi-Agent Debate**, ICLR 2025 [[paper](https://openreview.net/forum?id=t6QHYUOQL7)] :large_blue_circle:
72. **SBSC: Step-By-Step Coding for Improving Mathematical Olympiad Performance**, ICLR 2025 [[paper](https://openreview.net/forum?id=wSkvf2WyYz)] :large_blue_circle:
73. **Curriculum Demonstration Selection for In-Context Learning**, SAC 2025 [[paper](https://dl.acm.org/doi/abs/10.1145/3672608.3707810)] :large_blue_circle:
74. **GPG: A Simple and Strong Reinforcement Learning Baseline for Model Reasoning**, arXiv:2504.02546 [[paper](https://arxiv.org/abs/2504.02546)]
75. **Reinforcement Learning for Reasoning in Large Language Models with One Training Example**, arXiv:2504.20571 [[paper](https://arxiv.org/abs/2504.20571)] :large_blue_circle:
76. **Why Vision Language Models Struggle with Visual Arithmetic? Towards Enhanced Chart and Geometry Understanding**, Findings of ACL 2025 [[paper](https://arxiv.org/abs/2502.11492)]
77. **MM-Verify: Enhancing Multimodal Reasoning with Chain-of-Thought Verification**, arXiv:2502.13383 [[paper](https://arxiv.org/abs/2502.13383)] :large_blue_circle:
78. **Two Heads are Better Than One: Test-time Scaling of Multi-agent Collaborative Reasoning**, arXiv:2504.09772 [[paper](https://arxiv.org/abs/2504.09772)] :large_blue_circle:
79. **Climbing the Ladder of Reasoning: What LLMs Can-and Still Can't-Solve after SFT?**, arXiv:2504.11741 [[paper](https://arxiv.org/abs/2504.11741)] :large_blue_circle:
80. **Key-Point-Driven Data Synthesis with Its Enhancement on Mathematical Reasoning**, AAAI 2025 [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/34593)] :large_blue_circle:
81. **A Survey of Mathematical Reasoning in the Era of Multimodal Large Language Model: Benchmark, Method & Challenges**, Findings of ACL 2025 [[paper](https://arxiv.org/abs/2412.11936)] :large_blue_circle:
82. **Decoding Math: A Review of Datasets Shaping AI-Driven Mathematical Reasoning**, JIM 2025 [[paper](https://www.tarupublications.com/doi/10.47974/JIM-2105)] :large_blue_circle:
83. **Visual Large Language Models for Generalized and Specialized Application**, arXiv:2501.02765 [[paper](https://arxiv.org/abs/2501.02765)] :large_blue_circle:
84. **From System 1 to System 2: A Survey of Reasoning Large Language Models**, arXiv:2502.17419 [[paper](https://arxiv.org/abs/2502.17419)] :large_blue_circle:
85. **Towards Scientific Intelligence: A Survey of LLM-based Scientific Agents**, arXiv:2503.24047 [[paper](https://arxiv.org/abs/2503.24047)] :large_blue_circle:
86. **Plane Geometry Problem Solving with Multi-modal Reasoning: A Survey**, arXiv:2505.14340 [[paper](https://arxiv.org/abs/2505.14340)]
87. **Towards Geometry Problem Solving in the Large Model Era: A Survey**, arXiv:2506.02690 [[paper](https://arxiv.org/abs/2506.02690)]

## Citation

If you find this repository useful, please consider citing our survey paper:

```
@article{ma2025survey,
  title={A Survey of Deep Learning for Geometry Problem Solving},
  author={Ma, Jianzhe and Wang, Wenxuan and Jin, Qin},
  journal={arXiv preprint arXiv:2507.11936},
  year={2025}
}
```