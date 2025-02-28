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
The choice of representation for geographic location significantly impacts the accuracy of models for a broad range of geospatial tasks, including fine-grained species classification, population density estimation, and biome classification. Recent works like SatCLIP and GeoCLIP learn such representations by contrastively aligning geolocation with co-located images. While these methods work exceptionally well, in this paper, we posit that the current training strategies fail to fully capture the important visual features. We provide an information theoretic perspective on why the resulting embeddings from these methods discard crucial visual information that is important for many downstream tasks. To solve this problem, we propose a novel retrieval-augmented strategy called RANGE. We build our method on the intuition that the visual features of a location can be estimated by combining the visual features from multiple similar-looking locations. We evaluate our method across a wide variety of tasks. Our results show that RANGE outperforms the existing state-of-the-art models with significant margins in most tasks. We show gains of up to 13.1\% on classification tasks and 0.145 $R^2$ on regression tasks. All our code will be released on GitHub. Our models will be released on HuggingFace.
  </details>

