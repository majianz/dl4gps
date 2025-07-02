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
- [Tasks and Datasets](#tasks-and-datasets)
    - [Fundamental Tasks](#fundamental-tasks)
- [Related Surveys](#related-surveys)

## Surveys

1. **Plane Geometry Problem Solving with Multi-modal Reasoning: A Survey**, arXiv:2505.14340 [[paper](https://arxiv.org/abs/2505.14340)]

2. **Towards Geometry Problem Solving in the Large Model Era: A Survey**, arXiv:2506.02690 [[paper](https://arxiv.org/abs/2506.02690)]

## Tasks and Datasets

### Fundamental Tasks

#### Geometry Problem Parsing

1. **Extracting structured information from the textual description of geometry word problems**, NLPIR 2023 [[paper](https://dl.acm.org/doi/abs/10.1145/3639233.3639255)] :x:

1. **Automatic Extraction of Structured Information from Elementary Level Geometry Questions into Logic Forms**, Multimed Tools Appl 2024 [[paper](https://link.springer.com/article/10.1007/s11042-024-20463-w)]

1. **Evaluating Automated Geometric Problem Solving With Formal Language Generation on Large Multimodal Models**, IEIR 2024 [[paper](https://ieeexplore.ieee.org/abstract/document/10959992)]

1. **FGeo-Parser: Autoformalization and Solution of Plane Geometric Problems**, Symmetry 2025 [[paper](https://www.mdpi.com/2073-8994/17/1/8)]

##### Semantic Parsing for Geometry Problem

1. **Semantic Parsing of Pre-University Math Problems**, ACL 2017 [[paper](https://aclanthology.org/P17-1195/)] :x:

1. **Beyond Sentential Semantic Parsing: Tackling the Math SAT with a Cascade of Tree Transducers**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1083/)] :large_blue_circle: :x:

1. **From Textbooks to Knowledge: A Case Study in Harvesting Axiomatic Knowledge from Textbooks to Solve Geometry Problems**, EMNLP 2017 [[paper](https://aclanthology.org/D17-1081/)] :x:

1. **Discourse in Multimedia: A Case Study in Extracting Geometry Knowledge from Textbooks**, CL 2019 [[paper](https://aclanthology.org/J19-4002/)] :x:

1. **Extending a Parser to Distant Domains Using a Few Dozen Partially Annotated Examples**, ACL 2018 [[paper](https://aclanthology.org/P18-1110/)]

1. **A Neural Semantic Parser for Math Problems Incorporating Multi-Sentence Information**, TALLIP 2019 [[paper](https://dl.acm.org/doi/abs/10.1145/3314939)] :large_blue_circle:

1. **Two-step memory networks for deep semantic parsing of geometry word problems**, SOFSEM 2020 [[paper](https://dl.acm.org/doi/abs/10.1007/978-3-030-38919-2_57)]

1. **Semantic parsing of geometry statements using supervised machine learning on Synthetic Data**, NatFoM 2021 CICM Workshop [[paper](https://hal.science/hal-03327994/document)]

1. **Cognitive Patterns for Semantic Presentation of Natural-Language Descriptions of Well-Formalizable Problems**, RCAI 2021 [[paper](https://link.springer.com/chapter/10.1007/978-3-030-86855-0_22)] :x:

1. **Exploration of Formalization Techniques for Geometric Entities in Planar Geometry Proposition Texts**, JAIP 2025 \[[paper](https://www.clausiuspress.com/assets/default/article/2025/02/27/article_1740641608.pdf)]

##### Geometric Diagram Parsing

1. **Retrieving Geometric Information from Images: The Case of Hand-Drawn Diagrams**, KDD 2017 [[paper](https://link.springer.com/article/10.1007/s10618-017-0494-1)] :x:

1. **A Novel Geometric Information Retrieval Tool for Images of Geometric Diagrams**, ICISE-IE 2020 [[paper](https://ieeexplore.ieee.org/abstract/document/9418805)]

1. **2D geometric shapes dataset – For machine learning and pattern recognition**, Data in Brief 2020 [[paper](https://www.sciencedirect.com/science/article/pii/S2352340920309847)]

1. **A Paradigm of Diagram Understanding in Problem Solving**, TALE 2021 [[paper](https://ieeexplore.ieee.org/abstract/document/9678637)] :x:

1. **Plane Geometry Diagram Parsing**, IJCAI 2022 [[paper](https://www.ijcai.org/proceedings/2022/228)]

1. **Learning to Understand Plane Geometry Diagram**, NeurIPS 2022 MATH-AI Workshop [[paper](https://mathai2022.github.io/papers/6.pdf)]

1. **Usage of Stacked Long Short-Term Memory for Recognition of 3D Analytic Geometry Elements**, ICAART 2022 [[paper](https://www.scitepress.org/Papers/2022/108989/108989.pdf)]

1. **Solving Algebraic Problems with Geometry Diagrams Using Syntax-Semantics Diagram Understanding**, Computers, Materials & Continua 2023 [[paper](https://www.researchgate.net/profile/Litian-Huang/publication/375217917_Solving_Algebraic_Problems_with_Geometry_Diagrams_Using_Syntax-Semantics_Diagram_Understanding/links/654715da3fa26f66f4d60625/Solving-Algebraic-Problems-with-Geometry-Diagrams-Using-Syntax-Semantics-Diagram-Understanding.pdf)] :x:

1. **2D Shape Detection for Solving Geometry Word Problems**, IETE J. Res. 2024 [[paper](https://www.tandfonline.com/doi/abs/10.1080/03772063.2023.2274914)] :x:

1. **Slow Perception: Let's Perceive Geometric Figures Step-by-Step**, arXiv:2412.20631 \[[paper](https://arxiv.org/abs/2412.20631)]

1. **Leveraging Two-Level Deep Learning Classifers for 2D Shape Recognition to Automatically Solve Geometry Math Word Problems**, PAA 2024 [[paper](https://link.springer.com/article/10.1007/s10044-024-01321-9)]

1. **Tangram: A Challenging Benchmark for Geometric Element Recognizing**, arXiv:2408.13854 [[paper](https://arxiv.org/abs/2408.13854)]

1. **CurveML: A Benchmark for Evaluating and Training Learning-Based Methods of Classification, Recognition, and Fitting of Plane Curves**, Visual Comput 2024 [[paper](https://link.springer.com/article/10.1007/s00371-024-03292-8)]

#### Geometry Problem Parsing

##### Geometric Diagram Understanding

###### Geometric Structure Recognition

1. **Geoclidean: Few-Shot Generalization in Euclidean Geometry**, NeurIPS 2022 [[paper](https://proceedings.neurips.cc/paper_files/paper/2022/hash/feb34ce77fc8b94c85d12e608b23ce67-Abstract-Datasets_and_Benchmarks.html)]

1. **Euclid: Supercharging Multimodal LLMs With Synthetic High-Fidelity Visual Descriptions**, arXiv:2412.08737 [[paper](https://arxiv.org/abs/2412.08737)]

1. **GePBench: Evaluating Fundamental Geometric Perception for Multimodal Large Language Models**, arXiv:2412.21036 [[paper](https://arxiv.org/abs/2412.21036)]

1. **Do Large Language Models Truly Understand Geometric Structures?**, ICLR 2025 [[paper](https://openreview.net/forum?id=FjQOXenaXK)]

###### Geometric Diagram Captioning

1. 

### Core Tasks

#### Geometry Theorem Proving

#### Geometric Numerical Calculation

1. [FormalGeo7K-v2] **FGeo-Parser: Autoformalization and Solution of Plane Geometric Problems**, Symmetry 2025 [[paper](https://www.mdpi.com/2073-8994/17/1/8)] [[data](https://github.com/FormalGeo/FormalGeo)]


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



