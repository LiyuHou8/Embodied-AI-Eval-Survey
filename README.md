# Embodied-AI-Eval-Survey
A collection of papers and resources related to evaluations on Embodied AI.

# Papers and resources for Embodied AI evaluation

<!-- The papers are organized according to our survey: [A Survey on Evaluation of Embodied AI](embodied ai arxiv上面的链接). -->

NOTE: As we cannot update the arXiv paper in real time, please refer to this repo for the latest updates and the paper may be updated later. We also welcome any pull request or issues to help us make this survey perfect. Your contributions will be acknowledged in acknowledgements.

Please let us know if you find out a mistake or have any suggestions by e-mail: houly25@mails.jlu.edu.cn.

(We recommend copying lygao25@mails.jlu.edu.cn to ensure your message reaches us.)

![结构图示例](./assets/tree-picture1.png)

## Table of Contents

- [News and Updates](#news-and-updates)
- [What to evaluation](#What-to-evaluation)
  - [Perception and Understanding](#Perception-and-Understanding)
  - [Cognition and Reasoning](#Cognition-and-Reasoning)
  - [Task Planning and Decision-Making](#Task-Planning-and-Decision-Making)
  - [Action Execution and Control](#Action-Execution-and-Control)
  - [Trustworthiness and Generalization](#Trustworthiness-and-Generalization)
- [Where to evaluate](#Where-to-evaluate)
  - [Simulators](#Simulators)
  - [Datasets](#Datasets)
  - [Benchmarks](#Benchmarks)
- [How to evaluate](#How-to-evaluate)
  - [Core Performance Evaluation](#Core-Performance-Evaluation)
  - [Multidimensional and Hybrid Evaluation](#Multidimensional-and-Hybrid-Evaluation)
- [Contributing](#contributing)
- [Citation](#citation)
- [Acknowledgments](#acknowledgements)

---

## 📢 News and updates <a id="news-and-updates"></a>
- **[2026-01-05]** We created this repository.

## 📚 What to evaluation <a id="What-to-evaluation"></a>

### Perception and Understanding <a id="Perception-and-Understanding"></a>

#### Spatial Perception and Understanding
1. An evaluation of the RGB-D SLAM system. Felix Endres et al. ICRA 2012. [[paper](https://ieeexplore.ieee.org/abstract/document/6225199)]
2. A benchmark for the evaluation of RGB-D SLAM systems. Jürgen Sturm IROS 2012. [[paper](https://ieeexplore.ieee.org/abstract/document/6385773)][[data](https://cvg.cit.tum.de/data/datasets/rgbd-dataset)]
3. Comprehensive performance evaluation between visual slam and lidar slam for mobile robots: Theories and experiments. Yu-Lin Zhao et al. Applied Sciences 2024. [[paper](https://www.mdpi.com/2076-3417/14/9/3945)]
4. Performance evaluation of 2D LiDAR SLAM algorithms in simulated orchard environments. Qiujie Li et al. Computers and Electronics in Agriculture 2024. [[paper](https://www.sciencedirect.com/science/article/pii/S0168169924003855)]
5. LiDAR-based 3D SLAM for autonomous navigation in stacked cage farming houses: An evaluation. Jiacheng Jiang et al. Computers and Electronics in Agriculture 2025. [[paper](https://www.sciencedirect.com/science/article/pii/S0168169924012766)]
6. A Review of Simultaneous Localization and Mapping for the Robotic-Based Nondestructive Evaluation of Infrastructures. Ali Ghadimzadeh Alamdari et al. Sensors 2025. [[paper](https://www.mdpi.com/1424-8220/25/3/712)][[data](https://github.com/arvinebr/SLAM_review)]
7. How challenging is a challenge? cems: a challenge evaluation module for slam visual perception. Xuhui Zhao et al. JINT 2024. [[paper](https://link.springer.com/article/10.1007/s10846-024-02077-4)]
8. Embodiedscan: A holistic multi-modal 3d perception suite towards embodied ai. Tai Wang et al. CVPR 2024. [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_EmbodiedScan_A_Holistic_Multi-Modal_3D_Perception_Suite_Towards_Embodied_AI_CVPR_2024_paper.html)]
9. Embspatial-bench: Benchmarking spatial understanding for embodied tasks with large vision-language models. Mengfei Du et al. ACL 2024. [[paper](https://aclanthology.org/2024.acl-short.33/)][[data](https://github.com/mengfeidu/EmbSpatial-Bench)]
10. Spatial reasoning with vision-language models in ego-centric multi-view scenes. Mohsen Gholami et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.06266)]
11. Towards Autonomous UAV Visual Object Search in City Space: Benchmark and Agentic Methodology. Yatai Ji et al. arXiv 2025. [[paper](https://arxiv.org/abs/2505.08765)]
12. Why do mllms struggle with spatial understanding? a systematic analysis from data to architecture. Wanyue Zhang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.02359)][[data](https://huggingface.co/datasets/WanyueZhang/MulSeT)][[code](https://github.com/WanyueZhang-ai/spatial-understanding)]
13. Seeing from another perspective: Evaluating multi-view understanding in mllms. Chun-Hsiao Yeh et al. arXiv 2025. [[paper](https://arxiv.org/abs/2504.15280)][[benchmark](https://danielchyeh.github.io/All-Angles-Bench/)]
14. Beyond the Visible: Benchmarking Occlusion Perception in Multimodal Large Language Models. Zhaochen Liu et al. arXiv 2025. [[paper](https://arxiv.org/abs/2508.04059)]
15. Towards Omnidirectional Reasoning with 360-R1: A Dataset, Benchmark, and GRPO-based Method. Xinshen Zhang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2505.14197)]
16. CaptionQA: Is Your Caption as Useful as the Image Itself?. Shijia Yang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2511.21025)][[code](https://github.com/bronyayang/CaptionQA)]
17. ViewSpatial-Bench: Evaluating Multi-perspective Spatial Localization in Vision-Language Models. Dingming Li et al. arXiv 2025. [[paper](https://arxiv.org/abs/2505.21500)]
18. InternSpatial: A Comprehensive Dataset for Spatial Reasoning in Vision-Language Models. Nianchen Deng et al. arXiv 2025. [[paper](https://arxiv.org/abs/2506.18385)]

#### Scene and Physics Understanding
1. Llm meets scene graph: Can large language models understand and generate scene graphs? a benchmark and empirical study. Dongil Yang et al. ACL 2025. [[paper](https://aclanthology.org/2025.acl-long.1036/)][[benchmark](https://tsg-bench.netlify.app/)][[code](https://github.com/docworlds/tsg-bench)]
2. Embodiedscan: A holistic multi-modal 3d perception suite towards embodied ai. Tai Wang et al. CVPR 2024. [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Wang_EmbodiedScan_A_Holistic_Multi-Modal_3D_Perception_Suite_Towards_Embodied_AI_CVPR_2024_paper.html)]
3. ObjVariantEnsemble: Advancing Point Cloud LLM Evaluation in Challenging Scenes with Subtly Distinguished Objects. Qihang Cao et al. Proceedings of the AAAI Conference on Artificial Intelligence 2025. [[paper](https://ojs.aaai.org/index.php/AAAI/article/view/32190)][[projectpage](https://ove-benchmark.github.io/OVE/)]
4. CORE-3D: Context-aware Open-vocabulary Retrieval by Embeddings in 3D. Mohamad Amin Mirzaei et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.24528)]
5. Physbench: Benchmarking and enhancing vision-language models for physical world understanding. Wei Chow et al. ICLR 2025. [[paper](https://arxiv.org/abs/2501.16411)][[projectpage](https://physbench.github.io/)]
6. Text-Scene: A Scene-to-Language Parsing Framework for 3D Scene Understanding. Haoyuan Li et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.16721)]
7. Wow: Towards a world omniscient world model through embodied interaction. Xiaowei Chi et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.22642)]
8. PhysToolBench: Benchmarking Physical Tool Understanding for MLLMs. Zixin Zhang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2510.09507)][[projectpage](https://github.com/EnVision-Research/PhysToolBench)]


#### Social and Human-like Understanding
1. Activitynet: A large-scale video benchmark for human activity understanding. Fabian Caba Heilbron et al. CVPR 2015. [[paper](https://openaccess.thecvf.com/content_cvpr_2015/html/Heilbron_ActivityNet_A_Large-Scale_2015_CVPR_paper.html)][[projectpage](http://activity-net.org/)]
2. ACT-thor: A controlled benchmark for embodied action understanding in simulated environments. Michael Hanna et al. COLING 2022. [[paper](https://aclanthology.org/2022.coling-1.495/)][[data](https://github.com/hannamw/ACT-Thor)]
3. HIS-GPT: Towards 3D Human-In-Scene Multimodal Understanding. Jiahe Zhao et al. ICCV 2025. [[paper](https://arxiv.org/abs/2503.12955)][[benchmark](https://github.com/ZJHTerry18/HumanInScene)]
4. Can Vision Language Models Understand Mimed Actions?. Hyundong Justin Cho et al. Findings of ACL 2025. [[paper](https://aclanthology.org/2025.findings-acl.1372/)][[projectpage](https://justin-cho.com/mime)]
5. SoMi-ToM: Evaluating Multi-Perspective Theory of Mind in Embodied Social Interactions. Xianzhe Fan et al. arXiv 2025. [[paper](https://arxiv.org/abs/2506.23046)][[benchmark](https://github.com/XianzheFan/SoMi-ToM)][[data](https://huggingface.co/datasets/SoMi-ToM/SoMi-ToM)]
6. MEMO-Bench: A Multiple Benchmark for Text-to-Image and Multimodal Large Language Models on Human Emotion Analysis. Yingjie Zhou et al. arXiv 2024. [[paper](https://arxiv.org/abs/2411.11235)]
7. EmpathyAgent: Can Embodied Agents Conduct Empathetic Actions?. Xinyan Chen et al. arXiv 2025. [[paper](https://arxiv.org/abs/2503.16545)][[code&data](https://github.com/xinyan-cxy/EmpathyAgent)]

### Cognition and Reasoning <a id="Cognition-and-Reasoning"></a>

#### Cognitive and Commonsense Reasoning
1. Urbanvideo-bench: Benchmarking vision-language models on embodied intelligence with video data in urban spaces. Baining Zhao et al. arXiv 2025. [[paper](https://arxiv.org/abs/2503.06157)][[projectpage](https://embodiedcity.github.io/UrbanVideo-Bench/)][[data](https://huggingface.co/datasets/EmbodiedCity/UrbanVideo-Bench)][[code](https://github.com/EmbodiedCity/UrbanVideo-Bench.code)]
2. Rynnec: Bringing mllms into embodied world. Ronghao Dang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2508.14160)][[projectpage](https://github.com/alibaba-damo-academy/RynnEC)]
3. TinyLVLM-eHub: Towards comprehensive and efficient evaluation for large vision-language models. Wenqi Shao et al. TBD 2025. [[paper](https://ieeexplore.ieee.org/abstract/document/10858438)][[projectpage](https://github.com/OpenGVLab/Multi-Modality-Arena)]
4. Perceive, ground, reason, and act: A benchmark for general-purpose visual representation. Jiangyong Huang et al. arXiv 2022. [[paper](https://arxiv.org/abs/2211.15402)]
5. Text-Scene: A Scene-to-Language Parsing Framework for 3D Scene Understanding. Haoyuan Li et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.16721)]
6. OmniEAR: Benchmarking Agent Reasoning in Embodied Tasks. Zixuan Wang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2508.05614)][[gitub](https://github.com/ZJU-REAL/OmniEmbodied)][[projectpage](https://zju-real.github.io/OmniEmbodied)]
7. Openeqa: Embodied question answering in the era of foundation models. Arjun Majumdar et al. CVPR 2024. [[paper](https://openaccess.thecvf.com/content/CVPR2024/html/Majumdar_OpenEQA_Embodied_Question_Answering_in_the_Era_of_Foundation_Models_CVPR_2024_paper.html)][[projectpage](https://open-eqa.github.io/)]
8. VIVA+: Human-Centered Situational Decision-Making. Zhe Hu et al. EMNLP Findings 2025. [[paper](https://arxiv.org/abs/2509.23698)][[projectpage](https://derekhu.com/project_page/viva_plus_website/)]
9. CognitiveDrone: A VLA model and evaluation benchmark for real-time cognitive task solving and reasoning in UAVs. Artem Lykov et al. arXiv 2025. [[paper](https://arxiv.org/abs/2503.01378)][[projectpage](https://cognitivedrone.github.io/)]
10. Point-It-Out: Benchmarking Embodied Reasoning for Vision Language Models in Multi-Stage Visual Grounding. Haotian Xue et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.25794)][[projectpage](https://research.nvidia.com/labs/dir/pio/)][[gitub](https://github.com/xavihart/PIO)][[benchmark](https://huggingface.co/pio-benchmark/PIO)]
11. Physbench: Benchmarking and enhancing vision-language models for physical world understanding. Wei Chow et al. ICLR 2025. [[paper](https://arxiv.org/abs/2501.16411)][[projectpage](https://physbench.github.io/)]
12. SITE: towards Spatial Intelligence Thorough Evaluation. Wenqi Wang et al. ICCV 2025. [[paper](https://arxiv.org/abs/2505.05456)][[projectpage](https://wenqi-wang20.github.io/SITE-Bench.github.io/)]
13. ManipBench: Benchmarking vision-language models for low-level robot manipulation. Enyu Zhao et al. CoRL 2025. [[paper](https://arxiv.org/abs/2505.09698)][[projectpage](https://manipbench.github.io/)]
14. WorldLens: Full-Spectrum Evaluations of Driving World Models in Real World. Ao Liang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2512.10958)][[projectpage](https://worldbench.github.io/worldlens)][[gitub](https://github.com/worldbench/WorldLens)][[Leaderboard](https://huggingface.co/spaces/worldbench/WorldLens)][[data](https://huggingface.co/worldbench/datasets)]
15. From Pixels to Feelings: Aligning MLLMs with Human Cognitive Perception of Images. Yiming Chen et al. arXiv 2025. [[paper](https://arxiv.org/abs/2511.22805)][[projectpage](https://follen-cry.github.io/MLLM-Cognition-project-page/)]
16. Robocskbench: Benchmarking Embodied Commonsense Capabilities of Large Language Models. Jan-Philipp Töberg UR 2025. [[paper](https://ieeexplore.ieee.org/abstract/document/11078036)][[benchmark](https://github.com/ag-sc/Robo-CSK-Benchmark)]
17. Evaluating Multimodal Large Language Models with Daily Composite Tasks in Home Environments. Zhenliang Zhang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.17425)]
18. Cello: Causal evaluation of large vision-language models. Meiqi Chen et al. arXiv 2024. [[paper](https://arxiv.org/abs/2406.19131)][[projectpage](https://github.com/OpenCausaLab/CELLO)]
19. Et-plan-bench: Embodied task-level planning benchmark towards spatial-temporal cognition with foundation models. Lingfeng Zhang et al. arXiv 2024. [[paper](https://arxiv.org/abs/2410.14682)]
20. Urbanvideo-bench: Benchmarking vision-language models on embodied intelligence with video data in urban spaces. Baining Zhao et al. arXiv 2025. [[paper](https://arxiv.org/abs/2503.06157)][[projectpage](https://embodiedcity.github.io/UrbanVideo-Bench/)][[data](https://huggingface.co/datasets/EmbodiedCity/UrbanVideo-Bench)][[code](https://github.com/EmbodiedCity/UrbanVideo-Bench.code)]
21. Embodiedbench: Comprehensive benchmarking multi-modal large language models for vision-driven embodied agents. Rui Yang et al. ICML 2025. [[paper](https://arxiv.org/abs/2502.09560)][[projectpage](https://embodiedbench.github.io/)]
22. StarBench: A Turn-Based RPG Benchmark for Agentic Multimodal Decision-Making and Information Seeking. Haoran Zhang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2510.18483)]

#### Spatiotemporal Reasoning
1. Open3dvqa: A benchmark for comprehensive spatial reasoning with multimodal large language model in open space. Weichen Zhang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2503.11094)][[benchmark](https://github.com/EmbodiedCity/Open3D-VQA.code)]
2. Are Multimodal Large Language Models Ready for Omnidirectional Spatial Reasoning?. Zihao Dongfang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2505.11907)][[benchmark&code](https://huggingface.co/datasets/UUUserna/OSR-Bench)]
3. Evaluation of Vision-LLMs in Surveillance Video. Pascal Benschop et al. NeurIPS 2025. [[paper](https://arxiv.org/abs/2510.23190)][[evaluate](https://github.com/pascalbenschopTU/VLLM_AnomalyRecognition)]
4. Rynnec: Bringing mllms into embodied world. Ronghao Dang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2508.14160)][[projectpage](https://github.com/alibaba-damo-academy/RynnEC)]
5. MonoSR: Open-Vocabulary Spatial Reasoning from Monocular Images. Qirui Wang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2511.19119)][[projectpage](https://7rwang.github.io/MonoSR/)][[code](https://github.com/Zhantao-Gong/FSU-QA)][[data](https://huggingface.co/datasets/xxxgosh/MonoSR)]
6. Seeing Across Views: Benchmarking Spatial Reasoning of Vision-Language Models in Robotic Scenes. Zhiyuan Feng et al. arXiv 2025. [[paper](https://arxiv.org/abs/2510.19400)][[benchmark](https://github.com/microsoft/MV-RoboBench)]
7. SITE: towards Spatial Intelligence Thorough Evaluation. Wenqi Wang et al. ICCV 2025. [[paper](https://arxiv.org/abs/2505.05456)][[projectpage](https://wenqi-wang20.github.io/SITE-Bench.github.io/)]
8. Spatial reasoning with vision-language models in ego-centric multi-view scenes. Mohsen Gholami et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.06266)][[projectpage](https://vbdi.github.io/Ego3D-Bench-webpage/)][[code](https://github.com/vbdi/Ego3D-Bench)][[data](https://huggingface.co/datasets/vbdai/Ego3D-Bench)]
9. Towards Cross-View Point Correspondence in Vision-Language Models. Yipu Wang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2512.04686)][[code](https://github.com/WangYipu2002/CrossPoint)]
10. 3DLLM-Mem: Long-Term Spatial-Temporal Memory for Embodied 3D Large Language Model. Wenbo Hu et al. arXiv 2025. [[paper](https://arxiv.org/abs/2505.22657)][[projectpage](https://3dllm-mem.github.io/)]
11. Ost-bench: Evaluating the capabilities of mllms in online spatio-temporal scene understanding. JingLi Lin et al. arXiv 2025. [[paper](https://arxiv.org/abs/2507.07984)][[projectpage](https://rbler1234.github.io/OSTBench.github.io/)]
12. Out of Sight, Not Out of Context? Egocentric Spatial Reasoning in VLMs Across Disjoint Frames. Sahithya Ravi et al. EMNLP 2025. [[paper](https://aclanthology.org/2025.emnlp-main.816/)][[code&data](https://github.com/sahithyaravi/DISJOINT-3DQA)]
13. EOC-Bench: Can MLLMs Identify, Recall, and Forecast Objects in an Egocentric World?. Yuqian Yuan et al. arXiv 2025. [[paper](https://arxiv.org/abs/2506.05287)][[projectpage](https://circleradon.github.io/EOCBench/)][[code](https://github.com/alibaba-damo-academy/EOCBench)][[benchmark](https://huggingface.co/datasets/CircleRadon/EOC-Bench)]
14. Embrace-3k: Embodied reasoning and action in complex environments. Mingxian Lin et al. arXiv 2025. [[paper](https://arxiv.org/abs/2507.10548)][[projectpage](https://mxllc.github.io/EmbRACE-3K/)]
15. Robocas: A benchmark for robotic manipulation in complex object arrangement scenarios. Liming Zheng et al. arXiv 2024. [[paper](https://arxiv.org/abs/2407.06951)][[projectpage](https://github.com/notFoundThisPerson/RoboCAS-v0)]
16. RoboRefer: Towards Spatial Referring with Reasoning in Vision-Language Models for Robotics. Enshen Zhou et al. NeurIPS 2025. [[paper](https://arxiv.org/abs/2506.04308)][[projectpage](https://zhoues.github.io/RoboRefer/)]
17. SVAG-Bench: A Large-Scale Benchmark for Multi-Instance Spatio-temporal Video Action Grounding. Tanveer Hannan et al. arXiv 2025. [[paper](https://arxiv.org/abs/2510.13016)][[workshop](https://motchallenge.net/workshops/bmtt2025/)][[Codabench platform](https://www.codabench.org/competitions/9743/)]
18. AViLA: Asynchronous Vision-Language Agent for Streaming Multimodal Data Interaction. Gengyuan Zhang et al. arXiv 2025. [[paper](https://arxiv.org/abs/2506.18472)]
19. Eyes wide open: Ego proactive video-llm for streaming video. Yulin Zhang et al. NeurIPS 2025. [[paper](https://arxiv.org/abs/2510.14560)][[projectpage](https://zhangyl4.github.io/publications/eyes-wide-open/)]
20. RoboSeek: You Need to Interact with Your Objects. Yibo Peng et al. arXiv 2025. [[paper](https://arxiv.org/abs/2509.17783)][[projectpage](https://russderrick.github.io/Roboseek/)]

### Task Planning and Decision-Making <a id="Task-Planning-and-Decision-Making"></a>
#### Long-Horizon Dependency and Episodic Memory
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

#### Planning Grounding and the Execution Gap
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

#### Dynamic Adaptation and Closed-Loop Correction
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

#### Multi-Agent Collaboration and Human-Robot Trust
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

### Action Execution and Control <a id="Action-Execution-and-Control"></a>
#### Control Policies and Physical Dynamics
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

#### Object Manipulation and Navigation
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

#### Collaboration and Interactive Systems
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]


### Trustworthiness and Generalization <a id="Trustworthiness-and-Generalization"></a>
#### Safety
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

#### Robustness
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

#### Generalization
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]


## 📚 Where to evaluate <a id="Where-to-evaluate"></a>

### Simulators <a id="Simulators"></a>

#### General-Purpose Physics Simulators
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]


#### Task-Oriented Simulators
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

### Datasets <a id="Datasets"></a>
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
### Benchmarks <a id="Benchmarks"></a> 
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]

## 📚 How to evaluate <a id="How-to-evaluate"></a> 

### Core Performance Evaluation <a id="Core-Performance-Evaluation"></a> 
#### Task Performance
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
#### Efficiency and Quality
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
#### Safety and Constraints
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]
### Multidimensional and Hybrid Evaluation <a id="Multidimensional-and-Hybrid-Evaluation"></a>
- **论文全标题**. 第一作者姓名 et al. 会议/期刊名缩写 年份. [[paper](PDF链接)] [[code](代码链接)]


## 🤝 Contributing[未修改] <a id="contributing"></a> 
We welcome contributions to Embodied-AI-Eval-Survey! If you'd like to contribute, please follow these steps:

Fork the repository.
Create a new branch with your changes.
Submit a pull request with a clear description of your changes.
You can also open an issue if you have anything to add or comment.

## 📝 Citation[还未挂在axiv上面]  <a id="citation"></a> 
```bibtex
@article{your_surname202Xtitle,
  title={Your Paper Title},
  author={Your Name and Co-authors},
  journal={arXiv preprint arXiv:XXXX.XXXXX},
  year={202X}
}
```
## 🗺️ Acknowledgments  <a id="acknowledgements"></a> 
感谢