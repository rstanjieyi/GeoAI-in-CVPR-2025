# <p align=center>`GeoAI in CVPR 2025`</p>

:star2:**A collection of papers related to Geo-spatial Information Science in CVPR 2025.**

## 📢 Latest Updates
:fire::fire::fire: Last Updated on 2025.03.10 :fire::fire::fire:
- **2025.03.10**: Update 20 papers.


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


#### ABBSPO: Adaptive Bounding Box Scaling and Symmetric Prior based Orientation Prediction for Detecting Aerial Image Objects

> Woojin Lee, Hyugjae Chang, Jaeho Moon, Jaehyup Lee, Munchurl Kim

* Paper: None
* Project: https://kaist-viclab.github.io/ABBSPO_site/
* <details>
    <summary>Abstract (Click to expand):</summary>
    Weakly supervised Oriented Object Detection (WS-OOD) has gained attention as a cost-effective alternative to fully supervised methods, providing efficiency and high accuracy. Among weakly supervised approaches, horizontal bounding box (HBox) supervised OOD stands out for its ability to directly leverage existing HBox annotations while achieving the highest accuracy under weak supervision settings. This paper introduces adaptive bounding box scaling and symmetry-prior-based orientation prediction, called ABBSPO that is a framework for WS-OOD. Our ABBSPO addresses the limitations of previous HBox-supervised OOD methods, which compare ground truth (GT) HBoxes directly with predicted RBoxes' minimum circumscribed rectangles, often leading to inaccuracies. To overcome this, we propose: (i) Adaptive Bounding Box Scaling (ABBS) that appropriately scales the GT HBoxes to optimize for the size of each predicted RBox, ensuring more accurate prediction for RBoxes' scales; and (ii) a Symmetric Prior Angle (SPA) loss that uses the inherent symmetry of aerial objects for self-supervised learning, addressing the issue in previous methods where learning fails if they consistently make incorrect predictions for all three augmented views (original, rotated, and flipped). Extensive experimental results demonstrate that our ABBSPO achieves state-of-the-art results, outperforming existing methods.
  </details>


#### EarthDial: Turning Multi-sensory Earth Observations to Interactive Dialogues

> Sagar Soni, Akshay Dudhane, Hiyam Debary, Mustansar Fiaz, Muhammad Akhtar Munir, Muhammad Sohail Danish, Paolo Fraccaro, Campbell D Watson, Levente J Klein, Fahad Shahbaz Khan, Salman Khan

* Paper: https://arxiv.org/abs/2412.15190v1
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    Automated analysis of vast Earth observation data via interactive Vision-Language Models (VLMs) can unlock new opportunities for environmental monitoring, disaster response, and resource management. Existing generic VLMs do not perform well on Remote Sensing data, while the recent Geo-spatial VLMs remain restricted to a fixed resolution and few sensor modalities. In this paper, we introduce EarthDial, a conversational assistant specifically designed for Earth Observation (EO) data, transforming complex, multi-sensory Earth observations into interactive, natural language dialogues. EarthDial supports multi-spectral, multi-temporal, and multi-resolution imagery, enabling a wide range of remote sensing tasks, including classification, detection, captioning, question answering, visual reasoning, and visual grounding. To achieve this, we introduce an extensive instruction tuning dataset comprising over 11.11M instruction pairs covering RGB, Synthetic Aperture Radar (SAR), and multispectral modalities such as Near-Infrared (NIR) and infrared. Furthermore, EarthDial handles bi-temporal and multi-temporal sequence analysis for applications like change detection. Our extensive experimental results on 37 downstream applications demonstrate that EarthDial outperforms existing generic and domain-specific models, achieving better generalization across various EO tasks.
  </details>

#### IceDiff: High Resolution and High-Quality Arctic Sea Ice Forecasting with Generative Diffusion Prior

> Jingyi Xu, Siwei Tu, Weidong Yang, Shuhao Li, Keyi Liu, Yeqi Luo, Lipeng Ma, Ben Fei, Lei Bai

* Paper: https://arxiv.org/abs/2410.09111
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    Variation of Arctic sea ice has significant impacts on polar ecosystems, transporting routes, coastal communities, and global climate. Tracing the change of sea ice at a finer scale is paramount for both operational applications and scientific studies. Recent pan-Arctic sea ice forecasting methods that leverage advances in artificial intelligence has made promising progress over numerical models. However, forecasting sea ice at higher resolutions is still under-explored. To bridge the gap, we propose a two-staged deep learning framework, IceDiff, to forecast sea ice concentration at finer scales. IceDiff first leverages an independently trained vision transformer to generate coarse yet superior forecasting over previous methods at a regular 25km x 25km grid. This high-quality sea ice forecasting can be utilized as reliable guidance for the next stage. Subsequently, an unconditional diffusion model pre-trained on sea ice concentration maps is utilized for sampling down-scaled sea ice forecasting via a zero-shot guided sampling strategy and a patch-based method. For the first time, IceDiff demonstrates sea ice forecasting with the 6.25km x 6.25km resolution. IceDiff extends the boundary of existing sea ice forecasting models and more importantly, its capability to generate high-resolution sea ice concentration data is vital for pragmatic usages and research.
  </details>


#### PointSR: Self-regularized Point Supervision for Drone-view Object Detection

> Weizhuo Li, Yue Xi, Wenjing Jia, zehao zhang, Fei Li, Xiangzeng Liu, Qiguang Miao

* Paper: https://faculty.xidian.edu.cn/LIUXIANGZENG/zh_CN/lwcg/405906/content/281985.htm
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    Point-Supervised Object Detection (PSOD) in a discriminative style has recently gained significant attention for its impressive detection performance and cost-effectiveness.However, accurately predicting high-quality pseudo-box labels for drone-view images, which often feature densely packed small objects, remains a challenge. This difficulty arises primarily from the limitation of rigid sampling strategies, which hinder the optimization of pseudo-boxes. To address this, we propose PointSR, an effective and robust point-supervised object detection framework with self-regularized sampling that integrates temporal and informative constraints throughout the pseudo-box generation process. Specifically, the framework comprises three key components: Temporal-Ensembling Encoder (TE Encoder), Coarse Pseudo-box Prediction, and Pseudo-box Refinement. The TE Encoder builds an anchor prototype library by aggregating temporal information for dynamic anchor adjustment. In Coarse Pseudo-box Prediction, anchors are refined using the prototype library, and a set of informative samples is collected for subsequent refinement. During Pseudo-box Refinement, these informative negative sam-
ples are used to suppress low-confidence candidate positive samples, thereby improving the quality of the pseudo boxes. Experimental results on benchmark datasets demonstrate that PointSR significantly outperforms state-of-the-art methods, achieving up to 3.3%~ 7.2% higher AP50 using only point supervision. Additionally, it exhibits strong robustness to perturbation in human-labeled points.
  </details>


#### Hazy Low-Quality Satellite Video Restoration Via Learning Optimal Joint Degradation Patterns and Continuous-Scale Super-Resolution Reconstruction

> Ning Ni, Libao Zhang

* Paper: None
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>

#### MFogHub: Bridging Multi-Regional and Multi-Satellite Data for Global Marine Fog Detection and Forecasting

> Mengqiu XU, Kaixin Chen, Heng Guo, Yixiang Huang, Ming Wu, Zhenwei Shi, Chuang Zhang, Jun Guo

* Paper: None
* Code: https://github.com/kaka0910/MFogHub
* <details>
    <summary>Abstract (Click to expand):</summary>
    We introduce the MFogHub dataset—the first multi-regional, multi-satellite dataset for global marine fog detection and forecasting. MFogHub contains over 68,000 samples, and spans 15 coastal fog-prone regions, consolidating 693 marine fog events. The dataset captures multi-band meteorological data from 6 geostationary satellites. The minimum time interval is 30 minutes, with a spatial resolution of 1 km and a size of 1024 × 1024 pixels. Additionally, more than 11,600 samples are meticulously annotated at the pixel level by meteorological experts.
  </details>


#### AlphaPre: Amplitude-Phase Disentanglement Model for Precipitation Nowcasting

> Kenghong Lin, Baoquan Zhang, Demin Yu, Wenzhi Feng, Shidong Chen, Feifan Gao, Xutao Li, Yunming Ye

* Paper: None
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>


#### Satellite to GroundScape - Large-scale Consistent Ground View Generation from Satellite Views

> Ningli Xu, Rongjun Qin

* Paper: None
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>


#### Gaussian Splatting for Efficient Satellite Image Photogrammetry

> Luca Savant Aira, Gabriele Facciolo, Thibaud Ehret

* Paper: None
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>


#### SGFormer: Satellite-Ground Fusion for 3D Semantic Scene Completion

> Xiyue Guo, Jiarui Hu, Junjie Hu, Hujun Bao, Guofeng Zhang

* Paper: None
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>


#### Satellite Observations-guided Diffusion Model for Accurate Meteorological States at Arbitrary Resolution

> Siwei Tu, Ben Fei, Weidong Yang, Fenghua Ling, Hao Chen, Zili Liu, Kun Chen, Hang Fan, Wanli Ouyang, Lei Bai

* Paper: https://arxiv.org/abs/2502.07814v1
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    Accurate acquisition of surface meteorological conditions at arbitrary locations holds significant importance for weather forecasting and climate simulation. Due to the fact that meteorological states derived from satellite observations are often provided in the form of low-resolution grid fields, the direct application of spatial interpolation to obtain meteorological states for specific locations often results in significant discrepancies when compared to actual observations. Existing downscaling methods for acquiring meteorological state information at higher resolutions commonly overlook the correlation with satellite observations. To bridge the gap, we propose Satellite-observations Guided Diffusion Model (SGD), a conditional diffusion model pre-trained on ERA5 reanalysis data with satellite observations (GridSat) as conditions, which is employed for sampling downscaled meteorological states through a zero-shot guided sampling strategy and patch-based methods. During the training process, we propose to fuse the information from GridSat satellite observations into ERA5 maps via the attention mechanism, enabling SGD to generate atmospheric states that align more accurately with actual conditions. In the sampling, we employed optimizable convolutional kernels to simulate the upscale process, thereby generating high-resolution ERA5 maps using low-resolution ERA5 maps as well as observations from weather stations as guidance. Moreover, our devised patch-based method promotes SGD to generate meteorological states at arbitrary resolutions. Experiments demonstrate SGD fulfills accurate meteorological states downscaling to 6.25km.
  </details>


#### Exact: Exploring Space-Time Perceptive Clues for Weakly Supervised Satellite Image Time Series Semantic Segmentation

> Hao Zhu, Yan Zhu, Jiayu Xiao, Tianxiang Xiao, Yike Ma, Yucheng Zhang, Feng Dai

* Paper: https://arxiv.org/abs/2412.03968
* Code: https://github.com/MiSsU-HH/Exact
* <details>
    <summary>Abstract (Click to expand):</summary>
    Automated crop mapping through Satellite Image Time Series (SITS) has emerged as a crucial avenue for agricultural monitoring and management. However, due to the low resolution and unclear parcel boundaries, annotating pixel-level masks is exceptionally complex and time-consuming in SITS. This paper embraces the weakly supervised paradigm (i.e., only image-level categories available) to liberate the crop mapping task from the exhaustive annotation burden. The unique characteristics of SITS give rise to several challenges in weakly supervised learning: (1) noise perturbation from spatially neighboring regions, and (2) erroneous semantic bias from anomalous temporal periods. To address the above difficulties, we propose a novel method, termed exploring space-time perceptive clues (Exact). First, we introduce a set of spatial clues to explicitly capture the representative patterns of different crops from the most class-relative regions. Besides, we leverage the temporal-to-class interaction of the model to emphasize the contributions of pivotal clips, thereby enhancing the model perception for crop regions. Build upon the space-time perceptive clues, we derive the clue-based CAMs to effectively supervise the SITS segmentation network. Our method demonstrates impressive performance on various SITS benchmarks. Remarkably, the segmentation network trained on Exact-generated masks achieves 95% of its fully supervised performance, showing the bright promise of weakly supervised paradigm in crop mapping scenario.
  </details>



#### Benchmarking Object Detectors under Real-World Distribution Shifts in Satellite Imagery

> Sara Al-Emadi, Yin Yang, Ferda Ofli

* Paper: None
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>


#### The Change You Want To Detect: Semantic Change Detection In Earth Observation With Hybrid Data Generation

> Yanis Benidir, Nicolas Gonthier, Clement Mallet

* Paper: None
* Code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
   
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

#### XLRS-Bench: Could Your Multimodal LLMs Understand Extremely Large Ultra-High-Resolution Remote Sensing Imagery?

> Fengxiang Wang, hongzhen wang, Zonghao Guo, Di Wang, Yulin Wang, Mingshuo Chen, Qiang Ma, Long Lan, Wenjing Yang, Jing Zhang, Zhiyuan Liu, Maosong Sun

* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>


#### SkySense-O: Towards Open-World Remote Sensing Interpretation with Vision-Centric Visual-Language Modeling

> Qi Zhu, Jiangwei Lao, Deyi Ji, Junwei Luo, Kang Wu, Yingying Zhang, Lixiang Ru, Jian Wang, Ming Yang, Dong Liu, Feng Zhao

* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>


#### HyperFree: A Channel-adaptive and Tuning-free Foundation Model for Hyperspectral Remote Sensing Imagery

> Yingyi Liu, XINYU WANG, Yunning Peng, Chen Sun, Shaoyu Wang, Zhendong Sun, Tian Ke, Tangwei Lu, Anran Zhao, Yanfei Zhong

* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>

#### Effective Cloud Removal for Remote Sensing Images by an Improved Mean-Reverting Denoising Model with Elucidated Design Space

> Yi Liu, Wengen Li, Jihong Guan, Shuigeng Zhou, Yichao Zhang

* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>


#### RobSense: A Robust Multi-modal Foundation Model for Remote Sensing with Static, Temporal, and Incomplete Data Adaptability

> Kha Do, Kang Han, Phu Lai, Khoa T. Phan, Wei Xiang

* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>

#### RSVOS-SAM: High-Quality Interactive Segmentation for Remote Sensing Video Object

> Zhe Shan, Yang Liu, Lei Zhou, Cheng Yan, Heng Wang, Xia Xie

* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

  </details>

#### A General Adaptive Dual-level Weighting Mechanism for Remote Sensing Pansharpening

> Jie Huang, Haorui Chen, Jiaxuan Ren, Siran Peng, Liang-Jian Deng

* Paper: None
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>

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

> Qi Zang, Dong Zhao, Shuang Wang, Dou Quan, Licheng Jiao, Zhun Zhong
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

