# <p align=center>`GeoAI in CVPR 2025`</p>

:star2:**A collection of papers related to Geo-spatial Information Science in CVPR 2025.**

## 📢 Latest Updates
:fire::fire::fire: Last Updated on 2025.02.28 :fire::fire::fire:
- **2025.02.28**: Update 3 paper.


## :memo: CVPR 2025 Accepted Paper List



#### AnySat: An Earth Observation Model for Any Resolutions, Scales, and Modalities

> Guillaume Astruc, Nicolas Gonthier, Clement Mallet, Loic Landrieu.

* Paper: https://arxiv.org/abs/2412.14123
* project: https://gastruc.github.io/anysat
* Code: https://github.com/gastruc/AnySat
* <details>
    <summary>Abstract (Click to expand):</summary>
    Geospatial models must adapt to the diversity of Earth observation data in terms of resolutions, scales, and modalities. However, existing approaches expect fixed input configurations, which limits their practical applicability. We propose AnySat, a multimodal model based on joint embedding predictive architecture (JEPA) and resolution-adaptive spatial encoders, allowing us to train a single model on highly heterogeneous data in a self-supervised manner. To demonstrate the advantages of this unified approach, we compile GeoPlex, a collection of 5 multimodal datasets with varying characteristics and 11 distinct sensors. We then train a single powerful model on these diverse datasets simultaneously. Once fine-tuned, we achieve better or near state-of-the-art results on the datasets of GeoPlex and 4 additional ones for 5 environment monitoring tasks: land cover mapping, tree species identification, crop type classification, change detection, and flood segmentation. The code and models are available at this https [URL](https://github.com/gastruc/AnySat).
  </details>

#### Open-Canopy: Towards Very High Resolution Forest Monitoring

> Fajwel Fogel, Yohann Perron, Nikola Besic, Laurent Saint-André, Agnès Pellissier-Tanon, Martin Schwartz, Thomas Boudras, Ibrahim Fayad, Alexandre d’Aspremont, Loic Landrieu, Phillipe Ciais

* Paper: https://arxiv.org/pdf/2407.09392
* Code: https://github.com/fajwel/Open-Canopy
* Data: https://huggingface.co/datasets/AI4Forest/Open-Canopy
* <details>
    <summary>Abstract (Click to expand):</summary>
    Estimating canopy height and its changes at meter resolution from satellite imagery is a significant challenge in computer vision with critical environmental applications. However, the lack of open-access datasets at this resolution hinders the reproducibility and evaluation of models. We introduce Open-Canopy, the first open-access, country-scale benchmark for very high-resolution (1.5 m) canopy height estimation, covering over 87,000 km2 across France with 1.5 m resolution satellite imagery and aerial LiDAR data. Additionally, we present Open-Canopy-Δ, a benchmark for canopy height change detection between images from different years at tree level-a challenging task for current computer vision models. We evaluate state-of-the-art architectures on these benchmarks, highlighting significant challenges and opportunities for improvement. Our datasets and code are publicly available at this https [URL](https://github.com/fajwel/Open-Canopy).
  </details>


#### Around the World in 80 Timesteps: A Generative Approach to Global Visual Geolocation

> Nicolas Dufour, David Picard, Vicky Kalogeiton, Loic Landrieu. 

* Paper: https://arxiv.org/abs/2412.06781
* Project: https://nicolas-dufour.github.io/plonk
* Code: https://github.com/nicolas-dufour/plonk
* Demo: https://huggingface.co/spaces/nicolas-dufour/Plonk
* <details>
    <summary>Abstract (Click to expand):</summary>
    Global visual geolocation predicts where an image was captured on Earth. Since images vary in how precisely they can be localized, this task inherently involves a significant degree of ambiguity. However, existing approaches are deterministic and overlook this aspect. In this paper, we aim to close the gap between traditional geolocalization and modern generative methods. We propose the first generative geolocation approach based on diffusion and Riemannian flow matching, where the denoising process operates directly on the Earth's surface. Our model achieves state-of-the-art performance on three visual geolocation benchmarks: OpenStreetView-5M, YFCC-100M, and iNat21. In addition, we introduce the task of probabilistic visual geolocation, where the model predicts a probability distribution over all possible locations instead of a single point. We introduce new metrics and baselines for this task, demonstrating the advantages of our diffusion-based approach. Codes and models are [available.](https://nicolas-dufour.github.io/plonk)
  </details>

#### RANGE: Retrieval Augmented Neural Fields for Multi-Resolution Geo-Embeddings

> Aayush Dhakal, Srikumar Sastry, Subash Khanal, Adeel Ahmad, Eric Xing, Nathan Jacobs

* Paper: https://arxiv.org/abs/2502.19781
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    The choice of representation for geographic location significantly impacts the accuracy of models for a broad range of geospatial tasks, including fine-grained species classification, population density estimation, and biome classification. Recent works like SatCLIP and GeoCLIP learn such representations by contrastively aligning geolocation with co-located images. While these methods work exceptionally well, in this paper, we posit that the current training strategies fail to fully capture the important visual features. We provide an information theoretic perspective on why the resulting embeddings from these methods discard crucial visual information that is important for many downstream tasks. To solve this problem, we propose a novel retrieval-augmented strategy called RANGE. We build our method on the intuition that the visual features of a location can be estimated by combining the visual features from multiple similar-looking locations. We evaluate our method across a wide variety of tasks. Our results show that RANGE outperforms the existing state-of-the-art models with significant margins in most tasks. We show gains of up to 13.1% on classification tasks and 0.145 $R^2$ on regression tasks. All our code will be released on GitHub. Our models will be released on HuggingFace.
  </details>

#### SegEarth-OV: Towards Training-Free Open-Vocabulary Segmentation for Remote Sensing Images

> Kaiyu Li, Ruixun Liu, Xiangyong Cao, Xueru Bai, Feng Zhou, Deyu Meng, Zhi Wang

* Paper: https://arxiv.org/abs/2410.01768
* Project: https://likyoo.github.io/SegEarth-OV/
* <details>
    <summary>Abstract (Click to expand):</summary>
    Remote sensing image plays an irreplaceable role in fields such as agriculture, water resources, military, and disaster relief. Pixel-level interpretation is a critical aspect of remote sensing image applications; however, a prevalent limitation remains the need for extensive manual annotation. For this, we try to introduce open-vocabulary semantic segmentation (OVSS) into the remote sensing context. However, due to the sensitivity of remote sensing images to low-resolution features, distorted target shapes and ill-fitting boundaries are exhibited in the prediction mask. To tackle this issue, we propose a simple and general upsampler, SimFeatUp, to restore lost spatial information in deep features in a training-free style. Further, based on the observation of the abnormal response of local patch tokens to [CLS] token in CLIP, we propose to execute a straightforward subtraction operation to alleviate the global bias in patch tokens. Extensive experiments are conducted on 17 remote sensing datasets spanning semantic segmentation, building extraction, road detection, and flood detection tasks. Our method achieves an average of 5.8%, 8.2%, 4.0%, and 15.3% improvement over state-of-the-art methods on 4 tasks. All codes are released.
  </details>

#### Towards Satellite Image Road Graph Extraction: A Global-Scale Dataset and A Novel Method

> Pan Yin, Kaiyu Li, Xiangyong Cao, Jing Yao, Lei Liu, Xueru Bai, Feng Zhou, Deyu Meng

* Paper: https://arxiv.org/abs/2411.16733
* Dataset and code: https://github.com/earth-insights/samroadplus
* <details>
    <summary>Abstract (Click to expand):</summary>
    Recently, road graph extraction has garnered increasing attention due to its crucial role in autonomous driving, navigation, etc. However, accurately and efficiently extracting road graphs remains a persistent challenge, primarily due to the severe scarcity of labeled data. To address this limitation, we collect a global-scale satellite road graph extraction dataset, i.e. Global-Scale dataset. Specifically, the Global-Scale dataset is ∼20× larger than the largest existing public road extraction dataset and spans over 13,800 km2 globally. Additionally, we develop a novel road graph extraction model, i.e. SAM-Road++, which adopts a node-guided resampling method to alleviate the mismatch issue between training and inference in SAM-Road, a pioneering state-of-the-art road graph extraction model. Furthermore, we propose a simple yet effective ``extended-line'' strategy in SAM-Road++ to mitigate the occlusion issue on the road. Extensive experiments demonstrate the validity of the collected Global-Scale dataset and the proposed SAM-Road++ method, particularly highlighting its superior predictive power in unseen regions. The dataset and code are available at https://github.com/earth-insights/samroadplus.
  </details>


#### RSAR: Restricted State Angle Resolver and Rotated SAR Benchmark

> Xin Zhang, Xue Yang, Yuxuan Li, Jian Yang, Ming-Ming Cheng, Xiang Li

* Paper: https://arxiv.org/abs/2501.04440
* Dataset and code: https://github.com/zhasion/RSAR
* <details>
    <summary>Abstract (Click to expand):</summary>
    Rotated object detection has made significant progress in the optical remote sensing. However, advancements in the Synthetic Aperture Radar (SAR) field are laggard behind, primarily due to the absence of a large-scale dataset. Annotating such a dataset is inefficient and costly. A promising solution is to employ a weakly supervised model (e.g., trained with available horizontal boxes only) to generate pseudo-rotated boxes for reference before manual calibration. Unfortunately, the existing weakly supervised models exhibit limited accuracy in predicting the object's angle. Previous works attempt to enhance angle prediction by using angle resolvers that decouple angles into cosine and sine encodings. In this work, we first reevaluate these resolvers from a unified perspective of dimension mapping and expose that they share the same shortcomings: these methods overlook the unit cycle constraint inherent in these encodings, easily leading to prediction biases. To address this issue, we propose the Unit Cycle Resolver, which incorporates a unit circle constraint loss to improve angle prediction accuracy. Our approach can effectively improve the performance of existing state-of-the-art weakly supervised methods and even surpasses fully supervised models on existing optical benchmarks (i.e., DOTA-v1.0 dataset). With the aid of UCR, we further annotate and introduce RSAR, the largest multi-class rotated SAR object detection dataset to date. Extensive experiments on both RSAR and optical datasets demonstrate that our UCR enhances angle prediction accuracy. Our dataset and code can be found at: https://github.com/zhasion/RSAR.
  </details>


#### AeroGen: Enhancing Remote Sensing Object Detection with Diffusion-Driven Data Generation

> Datao Tang, Xiangyong Cao, Xuan Wu, Jialin Li, Jing Yao, Xueru Bai, Dongsheng Jiang, Yin Li, Deyu Meng

* Paper: https://arxiv.org/abs/2411.15497
* Dataset and code: https://github.com/Sonettoo/AeroGen
* <details>
    <summary>Abstract (Click to expand):</summary>
    Remote sensing image object detection (RSIOD) aims to identify and locate specific objects within satellite or aerial imagery. However, there is a scarcity of labeled data in current RSIOD datasets, which significantly limits the performance of current detection algorithms. Although existing techniques, e.g., data augmentation and semi-supervised learning, can mitigate this scarcity issue to some extent, they are heavily dependent on high-quality labeled data and perform worse in rare object classes. To address this issue, this paper proposes a layout-controllable diffusion generative model (i.e. AeroGen) tailored for RSIOD. To our knowledge, AeroGen is the first model to simultaneously support horizontal and rotated bounding box condition generation, thus enabling the generation of high-quality synthetic images that meet specific layout and object category requirements. Additionally, we propose an end-to-end data augmentation framework that integrates a diversity-conditioned generator and a filtering mechanism to enhance both the diversity and quality of generated data. Experimental results demonstrate that the synthetic data produced by our method are of high quality and diversity. Furthermore, the synthetic RSIOD data can significantly improve the detection performance of existing RSIOD models, i.e., the mAP metrics on DIOR, DIOR-R, and HRSC datasets are improved by 3.7%, 4.3%, and 2.43%, respectively. The code is available at https://github.com/Sonettoo/AeroGen.
  </details>

#### PEACE: Empowering Geologic Map Holistic Understanding with MLLMs

> Yangyu Huang, Tianyi Gao, Haoran Xu, Qihao Zhao, Yang Song, Zhipeng Gui, Tengchao Lv, Hao Chen, Lei Cui, Scarlett Li, Furu Wei

* Paper: https://arxiv.org/abs/2501.06184
* Dataset and code: https://github.com/microsoft/PEACE
* <details>
    <summary>Abstract (Click to expand):</summary>
    Geologic map, as a fundamental diagram in geology science, provides critical insights into the structure and composition of Earth's subsurface and surface. These maps are indispensable in various fields, including disaster detection, resource exploration, and civil engineering. Despite their significance, current Multimodal Large Language Models (MLLMs) often fall short in geologic map understanding. This gap is primarily due to the challenging nature of cartographic generalization, which involves handling high-resolution map, managing multiple associated components, and requiring domain-specific knowledge. To quantify this gap, we construct GeoMap-Bench, the first-ever benchmark for evaluating MLLMs in geologic map understanding, which assesses the full-scale abilities in extracting, referring, grounding, reasoning, and analyzing. To bridge this gap, we introduce GeoMap-Agent, the inaugural agent designed for geologic map understanding, which features three modules: Hierarchical Information Extraction (HIE), Domain Knowledge Injection (DKI), and Prompt-enhanced Question Answering (PEQA). Inspired by the interdisciplinary collaboration among human scientists, an AI expert group acts as consultants, utilizing a diverse tool pool to comprehensively analyze questions. Through comprehensive experiments, GeoMap-Agent achieves an overall score of 0.811 on GeoMap-Bench, significantly outperforming 0.369 of GPT-4o. Our work, emPowering gEologic mAp holistiC undErstanding (PEACE) with MLLMs, paves the way for advanced AI applications in geology, enhancing the efficiency and accuracy of geological investigations.
  </details>

#### Point2RBox-v2: Rethinking Point-supervised Oriented Object Detection with Spatial Layout Among Instances

> Yi Yu, Botao Ren, Peiyuan Zhang, Mingxin Liu, Junwei Luo, Shaofeng Zhang, Feipeng Da, Junchi Yan, Xue Yang

* Paper: https://arxiv.org/abs/2502.04268
* Code: https://github.com/VisionXLab/point2rbox-v2
* Zhihu: https://zhuanlan.zhihu.com/p/21748498041
* <details>
    <summary>Abstract (Click to expand):</summary>
    With the rapidly increasing demand for oriented object detection (OOD), recent research involving weakly-supervised detectors for learning OOD from point annotations has gained great attention. In this paper, we rethink this challenging task setting with the layout among instances and present Point2RBox-v2. At the core are three principles: 1) Gaussian overlap loss. It learns an upper bound for each instance by treating objects as 2D Gaussian distributions and minimizing their overlap. 2) Voronoi watershed loss. It learns a lower bound for each instance through watershed on Voronoi tessellation. 3) Consistency loss. It learns the size/rotation variation between two output sets with respect to an input image and its augmented view. Supplemented by a few devised techniques, e.g. edge loss and copy-paste, the detector is further enhanced. To our best knowledge, Point2RBox-v2 is the first approach to explore the spatial layout among instances for learning point-supervised OOD. Our solution is elegant and lightweight, yet it is expected to give a competitive performance especially in densely packed scenes: 62.61%/86.15%/34.71% on DOTA/HRSC/FAIR1M. 
  </details>

  
#### Adaptive Rectangular Convolution for Remote Sensing Pansharpening

> Xueyang Wang, Zhixin Zheng, Jiandong Shao, Yule Duan, Liang-Jian Deng

* Paper: https://arxiv.org/abs/2503.00467v1
* Dataset and code: https://github.com/WangXueyang-uestc/ARConv
* <details>
    <summary>Abstract (Click to expand):</summary>
    Recent advancements in convolutional neural network (CNN)-based techniques for remote sensing pansharpening have markedly enhanced image quality. However, conventional convolutional modules in these methods have two critical drawbacks. First, the sampling positions in convolution operations are confined to a fixed square window. Second, the number of sampling points is preset and remains unchanged. Given the diverse object sizes in remote sensing images, these rigid parameters lead to suboptimal feature extraction. To overcome these limitations, we introduce an innovative convolutional module, Adaptive Rectangular Convolution (ARConv). ARConv adaptively learns both the height and width of the convolutional kernel and dynamically adjusts the number of sampling points based on the learned scale. This approach enables ARConv to effectively capture scale-specific features of various objects within an image, optimizing kernel sizes and sampling locations. Additionally, we propose ARNet, a network architecture in which ARConv is the primary convolutional module. Extensive evaluations across multiple datasets reveal the superiority of our method in enhancing pansharpening performance over previous techniques. Ablation studies and visualization further confirm the efficacy of ARConv.
  </details>
  
#### Cross-Rejective Open-Set SAR Image Registration

> 毛莎莎，路世明，杜召龙，焦李成，缑水平，牟伦田，鲁学权，熊霖，张艺蒙

* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    合成孔径雷达（SAR）图像配准是遥感科学应用中的一项关键上游任务，通常以两幅图像预提取的关键点作为观测对象进行匹配点对搜索。通常，配准被视为一种典型的闭集分类问题，即强制将每个关键点归类到已知类别中，却忽视了大量冗余关键点超出预设类别的本质问题，这不可避免地会导致捕捉到错误的匹配点对。基于此，我们提出了一种跨域拒绝开集SAR图像配准方法，简称CroR-OSIR。在这项工作中，冗余关键点被视为分布外(OOD)样本，将配准问题重新定义为一种特殊的开集任务。该算法主要包含两个模块：监督对比特征提取模块(SupCon)和跨域拒绝开集识别模块(CroR-OSR)。区别于传统开放集识别，CroR-OSR模块中所有样本(包括OOD样本)均可用于训练，并在两幅图像的独立开集域中进行闭集分类，通过设计跨域拒绝机制，利用置信度和一致性对样本点进行评估，有效排除非配准点对的OOD样本。此外，将CroR-OSR模块输出的跨域估计标签反馈至SupCon模块，以增强关键点特征的判别性。实验结果表明，所提出的方法在配准精度上优于当前最先进的方法。
  </details>

#### Feature Spectrum Learning for Remote Sensing Change Detection

> 臧琪，赵栋，王爽，权豆，焦李成，钟准
* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    变化检测（CD）对地球观测具有重要意义，其中由成像环境因素引起的双时相图像之间的伪变化是关键挑战。现有的方法主要将伪变化视为一种风格转移，并通过使用生成对抗网络（GANs）将双时相图像转化为相同风格来缓解这一问题。然而，这些方法的努力受到优化GANs复杂性和缺乏物理属性指导的限制。本文发现，谱变换（ST）有潜力通过在频域中对齐承载风格的信息来减轻伪变化。然而，ST的优势在很大程度上受到两个缺点的制约：1）有限的变换空间和2）低效的参数搜索。为了解决这些限制，我们提出了特征谱学习（FeaSpect），在潜在空间中自适应地消除伪变化。针对缺点1），FeaSpect通过特征谱变换（FST）引导变换走向风格对齐的判别性特征。针对缺点2），FeaSpect使得FST可以训练，从而通过自适应注意力提取框和可学习步幅提取框高效地发现最优参数。大量实验表明，我们的方法显著优于现有方法，并在准确性和效率之间实现了良好的权衡。更重要的是，我们的方法可以轻松地嵌入到其他框架中，获得一致的提升。
  </details>


#### ROS-SAM: High-Quality Interactive Segmentation for Remote Sensing Moving Object

> Zhe Shan et.al
* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    针对高质量分割遥感视频中运动目标展开研究，提出一种名为ROS-SAM的模型框架。ROS-SAM建立在三个关键创新之上：（1）基于LoRA的微调，在保持SAM泛化能力的同时注入特定的遥感领域知识。（2）增强深度网络层以提高提取特征的可区分性，减少对易混淆物体的误分类。（3）在掩码解码器中将全局上下文与局部边界细节集成以生成高质量的分割掩码。此外，我们重新设计了训练和推理框架，以确保模型在训练过程中能够更好地处理不同尺度的对象，同时在推理过程中专注于高质量的预测。
  </details>

  
#### Towards Generalizable Scene Change Detection

> Jaewoo Kim, Uehwan Kim
* Paper: https://arxiv.org/abs/2409.06214
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    While current state-of-the-art Scene Change Detection (SCD) approaches achieve impressive results in well-trained research data, they become unreliable under unseen environments and different temporal conditions; in-domain performance drops from 77.6% to 8.0% in a previously unseen environment and to 4.6% under a different temporal condition -- calling for generalizable SCD and benchmark. In this work, we propose the Generalizable Scene Change Detection Framework (GeSCF), which addresses unseen domain performance and temporal consistency -- to meet the growing demand for anything SCD. Our method leverages the pre-trained Segment Anything Model (SAM) in a zero-shot manner. For this, we design Initial Pseudo-mask Generation and Geometric-Semantic Mask Matching -- seamlessly turning user-guided prompt and single-image based segmentation into scene change detection for a pair of inputs without guidance. Furthermore, we define the Generalizable Scene Change Detection (GeSCD) benchmark along with novel metrics and an evaluation protocol to facilitate SCD research in generalizability. In the process, we introduce the ChangeVPR dataset, a collection of challenging image pairs with diverse environmental scenarios -- including urban, suburban, and rural settings. Extensive experiments across various datasets demonstrate that GeSCF achieves an average performance gain of 19.2% on existing SCD datasets and 30.0% on the ChangeVPR dataset, nearly doubling the prior art performance. We believe our work can lay a solid foundation for robust and generalizable SCD research.
  </details>

