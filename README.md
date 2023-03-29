# EMDE

## Achievements

:one:st place at [SIGIR eCom Challenge 2020](https://sigir-ecom.github.io/ecom20DCPapers/SIGIR_eCom20_DC_paper_1.pdf)
 
:two:nd place  and Best Paper Award at [WSDM Booking.com Challenge 2021](http://ceur-ws.org/Vol-2855/challenge_short_3.pdf)

:two:nd place at [Twitter Recsys Challenge 2021](https://recsys-twitter.com/competition_leaderboard/latest)

:three:rd place at [KDD Cup 2021](https://ogb.stanford.edu/paper/kddcup2021/mag240m_SyneriseAI.pdf)
 
## Applications

<p align="left"><img width="100" src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/Zomato_Logo.svg/2500px-Zomato_Logo.svg.png" /></p>

_We are currently using EMDE  for generating candidates to facilitate downstream recommendation systems. It generates 
recommendations using density-based rich customer representation. It allows us to trace customer look-alikes 
(‘People Like You’) to find similar users with similar cuisine/taste preferences as well as price affinity. 
We used Cleora for customer-restaurants graph data […] And to our delight, the embedding generation was superfast 
(i.e <5 minutes). For context, do remember that GraphSAGE took ~20hours for the same data in the NCR region. 
Cleora + EMDE gives us a generalised framework for recommendations […] We are exploring ways to use it in other 
applications such as search ranking, dish recommendations, etc._\
~ **Zomato.com Data Science team** 

<p align="left"><img width="150" src="https://upload.wikimedia.org/wikipedia/commons/4/48/Dailymotion_logo_%282017%29.svg" /></p>

**Dailymotion** has applied **EMDE** to personalize video recommendations in native applications, leading to improved relevance
and catalog coverage.

<p align="left"><img width="130" src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/79/Synerise_logo.svg/2560px-Synerise_logo.svg.png" /></p>

**Synerise** is using EMDE working with clients from many industries such as: 

*retail*, *ecommerce*, *banking*, *telco*, *travel*, *health*, *insurance*, *automotive*, *fashion*

for tasks including:

*recommendations*, *propensity prediction*, *churn prediction*, *anaomaly detection*, *customer scoring*, *customer 
matching*, *behavioral super-segmentation* 

# Efficient Manifold Density Estimator

**EMDE** is a framework utilizing arbitrary vector representations with the property of 
local similarity to succinctly represent smooth probability densities on Riemannian manifolds.

**EMDE** can be used to:
- create a fixed-size aggregated representation
- serve as an input and output to the neural network
- work with multi-modal data
- work with various embedding types 

**EMDE** competitive edge:
- significantly increases model performance
- shifts heavy lifting part from neural network to data representation
- results in radically smaller models and shorter training time

**In most of our use cases, we use a sparse feed-forward network with around 5 layers and trained for 2 to 5 epochs 
on a single GPU.**

## Blog posts
- [EMDE Illustrated](https://sair.synerise.com/emde-illustrated/)
- [EMDE vs Multiresolution Hash Encoding](https://sair.synerise.com/emde-vs-multiresolution-hash-encoding/)
- [Towards a multi-purpose behavioral model](https://sair.synerise.com/towards-a-multi-purpose-behavioral-model/)
## Papers
- [An efficient manifold density estimator for all recommendation systems](https://9arxiv.org/abs/2006.01894)
- [T-EMDE: Sketching-based global similarity for cross-modal retrieval](https://arxiv.org/abs/2105.04242)
- [I know why you like this movie: Interpretable Efficient Multimodal Recommender](https://arxiv.org/abs/2006.09979)

## Cite

Please cite [our paper](https://arxiv.org/abs/2006.01894):

```
@inproceedings{dkabrowski2021efficient,
  title={An efficient manifold density estimator for all recommendation systems},
  author={D{\k{a}}browski, Jacek and Rychalska, Barbara and Daniluk, Micha{\l} and Basaj, Dominika and Go{\l}uchowski, Konrad and B{\k{a}}bel, Piotr and Micha{\l}owski, Andrzej and Jakubowski, Adam},
  booktitle={Neural Information Processing: 28th International Conference, ICONIP 2021, Sanur, Bali, Indonesia, December 8--12, 2021, Proceedings, Part IV 28},
  pages={323--337},
  year={2021},
  organization={Springer}
}
```
