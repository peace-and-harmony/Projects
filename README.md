# Nature articles topic modelling
Topic modelling and analysis on Nature published articles since 1873.

* Scraped around 19760 articles from 1873 to 2021.
* Performed EDA on the numerical data and concluded that the pandemic indeed boosts the related researches.
* Utilized Bertopic to the extracted abstracts to investigate the subjects evolution along the history.


<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the project](#about-the-project)

* [Results and discussion](#results-and-discussion)
  * [Topic modelling](#topic-modelling)
  * [Exploratory data analysis](#eda)
* [Conclusion](#conclusion)
* [Citation](#citation)
* [Supplimentary information](#supplimentary-info)   
  * [Notebooks](#notebooks)
  * [Scripts and tools](#scripts-and-tools)
  * [Supplementary data](#supplementary-data)
* [Contact](#contact)

<!-- ABOUT THE PROJECT -->
## About The Project

<!-- ![product-screenshot-tbc](data/example-inference.png) -->
[Nature](https://www.nature.com/) is one of the most cited scientific journals. Among different types of sections in an issue, [original research articles](https://www.nature.com/nature/articles?type=article) are original reports whose conclusions represent a substantial advance in understanding of an important problem and have immediate, far-reaching implications. The general articles information and corresponding article abstracts were obtained via a scraper. Based on these data, explotary data analysis  and topic modelling was performed for further understanding the general scope of the evolusion of human interested knowdges.

<!-- Discussion and results -->
## Results and discussion

### Topic Modelling

At the stage of information explosion era, topic modelling becomes essential for understanding of unstructured data. As one of the essence of human knowledge, nature research articles provide highly focused and trustable multidisciplinary presentation of knowledge.



Topic word score.
After fit and transform, Bertopic generated corresponding embedding space which can be utilized for further analysis. First of all, it's important to know how many topics over the 16276 articles from 1873 to 2021 of the Nature. There are around 240 topics recognized from the abstract pool. For illustration, top 6 topics and three personal interested topics are presented in Fig. 1.
>The colored areas are the dense areas of documents. Red points are outliers that do not belong to a specific cluster.
![product-screenshot-tbc](images/Topic_word_scores.png)

Pay attention to the topic word scores:
![product-screenshot-tbc](images/Topic_word_scores.png)

>Perspective for topic evolution over 148 years from 1873 to 2021.
Explore the [Bertopic](https://github.com/MaartenGr/BERTopic) generated topics over time:
![product-screenshot-tbc](images/Topics_over_time.png)

Present the generated topics among the 15000 abstracts:
![product-screenshot-tbc](images/Intertopic_distance_map.png)


And it's interesting to explore the hierarchical distribustion of the founded topics:
![product-screenshot-tbc](images/Hierarchical_clustering.png)

### Exploratory Data Analysis
Obviously, the covid-19 pandemic hindered the development of plenty areas, e.g. business, internationalism. At the beginning of the pandemic, some academic labs are closed and a lot of experiments are delayed. It's interesting to analize whether the pandemic indeed slow down the development of academia.

## Conclusion
EDA clearly suggests that instead of hindering the development of academia, the pandemic expands and accelerate areas related with SARS‑CoV‑2. 
From the results of topic modelling, it is intriguing to overview the topic evolutions over the 148 years which closely related with human beings' development and can be foreseen the futher areas that human will focused on. 

## Supplimentary information
For more details of this project, please check the information listed below.
  * [Notebooks](#notebooks)
  * [Scripts and tools](#scripts-and-tools)
  * [Supplementary data](#supplementary-data)

## Citation

```bibtex
@article{devito2020we,
  title={How we learnt to stop worrying and love web scraping},
  author={DeVito, Nicholas J and Richards, G and Inglesby, Peter},
  journal={Nature},
  volume={585},
  year={2020},
  publisher={Nature Research}
}
```

```bibtex
@misc{grootendorst2020bertopic,
  author = {Maarten Grootendorst},
  title = {BERTopic: Leveraging BERT and c-TF-IDF to create easily interpretable topics.},
  year  = 2020,
  publisher = {Zenodo},
  version = {v0.7.0},
  doi = {10.5281/zenodo.4381785},
  url = {https://doi.org/10.5281/zenodo.4381785}
}
```
## Contact
