# <p align=center>`GeoAI in CVPR 2025`</p>

:star2:**A collection of papers related to Geo-spatial Information Science in CVPR 2025.**

## 📢 Latest Updates
:fire::fire::fire: Last Updated on 2025.02.28 :fire::fire::fire:
- **2025.02.28**: Update 1 paper.


## :memo: CVPR 2025 Accepted Paper List


#### RANGE: Retrieval Augmented Neural Fields for Multi-Resolution Geo-Embeddings

> Aayush Dhakal, Srikumar Sastry, Subash Khanal, Adeel Ahmad, Eric Xing, Nathan Jacobs

* Paper: https://arxiv.org/abs/2502.19781
* Dataset and code: None
* <details>
    <summary>Abstract (Click to expand):</summary>
    The choice of representation for geographic location significantly impacts the accuracy of models for a broad range of geospatial tasks, including fine-grained species classification, population density estimation, and biome classification. Recent works like SatCLIP and GeoCLIP learn such representations by contrastively aligning geolocation with co-located images. While these methods work exceptionally well, in this paper, we posit that the current training strategies fail to fully capture the important visual features. We provide an information theoretic perspective on why the resulting embeddings from these methods discard crucial visual information that is important for many downstream tasks. To solve this problem, we propose a novel retrieval-augmented strategy called RANGE. We build our method on the intuition that the visual features of a location can be estimated by combining the visual features from multiple similar-looking locations. We evaluate our method across a wide variety of tasks. Our results show that RANGE outperforms the existing state-of-the-art models with significant margins in most tasks. We show gains of up to 13.1% on classification tasks and 0.145 $R^2$ on regression tasks. All our code will be released on GitHub. Our models will be released on HuggingFace.
  </details>

#### SegEarth-OV: Towards Training-Free Open-Vocabulary Segmentation for Remote Sensing Images

> Kaiyu Li, Xiangyong Cao, Yupeng Deng, Chao Pang, Zepeng Xin, Deyu Meng, Zhi Wang

* Paper: https://arxiv.org/abs/2501.12931
* Project: https://likyoo.github.io/DynamicEarth/
* <details>
    <summary>Abstract (Click to expand):</summary>
    Remote sensing image plays an irreplaceable role in fields such as agriculture, water resources, military, and disaster relief. Pixel-level interpretation is a critical aspect of remote sensing image applications; however, a prevalent limitation remains the need for extensive manual annotation. For this, we try to introduce open-vocabulary semantic segmentation (OVSS) into the remote sensing context. However, due to the sensitivity of remote sensing images to low-resolution features, distorted target shapes and ill-fitting boundaries are exhibited in the prediction mask. To tackle this issue, we propose a simple and general upsampler, SimFeatUp, to restore lost spatial information in deep features in a training-free style. Further, based on the observation of the abnormal response of local patch tokens to [CLS] token in CLIP, we propose to execute a straightforward subtraction operation to alleviate the global bias in patch tokens. Extensive experiments are conducted on 17 remote sensing datasets spanning semantic segmentation, building extraction, road detection, and flood detection tasks. Our method achieves an average of 5.8%, 8.2%, 4.0%, and 15.3% improvement over state-of-the-art methods on 4 tasks. All codes are released.
  </details>
