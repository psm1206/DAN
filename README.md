# Why is Normalization Necessary for Linear Recommenders? (SIGIR'25)
This is the official code for DAN in the paper "[Why is Normalization Necessary for Linear Recommenders?](https://dl.acm.org/doi/10.1145/3726302.3730116)", [The 48th International ACM SIGIR Conference on Research and Development in Information Retrieval](https://sigir2025.dei.unipd.it/).

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/why-is-normalization-necessary-for-linear/collaborative-filtering-on-gowalla)](https://paperswithcode.com/sota/collaborative-filtering-on-gowalla?p=why-is-normalization-necessary-for-linear)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/why-is-normalization-necessary-for-linear/collaborative-filtering-on-yelp2018)](https://paperswithcode.com/sota/collaborative-filtering-on-yelp2018?p=why-is-normalization-necessary-for-linear)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/why-is-normalization-necessary-for-linear/collaborative-filtering-on-amazon-book)](https://paperswithcode.com/sota/collaborative-filtering-on-amazon-book?p=why-is-normalization-necessary-for-linear)

[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/why-is-normalization-necessary-for-linear/recommendation-systems-on-gowalla)](https://paperswithcode.com/sota/recommendation-systems-on-gowalla?p=why-is-normalization-necessary-for-linear)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/why-is-normalization-necessary-for-linear/recommendation-systems-on-yelp2018)](https://paperswithcode.com/sota/recommendation-systems-on-yelp2018?p=why-is-normalization-necessary-for-linear)
[![PWC](https://img.shields.io/endpoint.svg?url=https://paperswithcode.com/badge/why-is-normalization-necessary-for-linear/recommendation-systems-on-amazon-book)](https://paperswithcode.com/sota/recommendation-systems-on-amazon-book?p=why-is-normalization-necessary-for-linear)

## Introduction
Despite their simplicity, linear autoencoder (LAE)-based models have shown comparable or even better performance with faster inference speed than neural recommender models. However, LAEs face two critical challenges:

1. **Popularity bias**: LAEs tend to recommend popular items excessively
2. **Neighborhood bias**: LAEs overly focus on capturing local item correlations

To address these issues, we propose **Data-Adaptive Normalization (DAN)**, a versatile normalization solution that flexibly controls the popularity and neighborhood biases by adjusting item- and user-side normalization to align with unique dataset characteristics.

Note that a summary of our paper is on [our lab blog](https://dial.skku.edu/blog/2025_dan) (in Korean).

## Requirements
```
pip install -r requirements.txt
```

## How to run
- Run LAE with DAN
```
sh dan_lae.sh
```
- Run EASE with DAN
```
sh dan_ease.sh
```
- Run RLAE with DAN
```
sh dan_rlae.sh
```

## TODO
- [ ] Add strong generalization protocol


## Citation

If you find our work useful for your research, please cite our paper:
```
@inproceedings{park2025dan,
  title={Why is Normalization Necessary for Linear Recommenders?},
  author={Seongmin Park and
          Mincheol Yoon and
          Hye-young Kim and
          Jongwuk Lee},
  booktitle={Proceedings of the 48th International ACM SIGIR Conference on Research and Development in Information Retrieval},
  year={2025}
}
```
