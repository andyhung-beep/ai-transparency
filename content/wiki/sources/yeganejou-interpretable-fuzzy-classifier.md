# Interpretable Deep Convolutional Fuzzy Classifier

**Source file**: [Original article](../../raw/Yeganejou et al._Interpretable_Deep_Convolutional_Fuzzy_Classifier.pdf)

**Summary**: Proposes a hybrid architecture combining convolutional neural networks with fuzzy logic classifiers to improve the interpretability of deep learning models, demonstrating that transparency can be introduced at modest accuracy cost through an explanation mechanism based on cluster medoids and saliency maps.

**Sources**: Yeganejou et al._Interpretable_Deep_Convolutional_Fuzzy_Classifier.txt

**Research questions addressed**: RQ1, RQ2

**Last updated**: 2026-04-18

---

## Overview

Published in *IEEE Transactions on Fuzzy Systems* (Vol. 28, No. 7, July 2020), this paper by Mojtaba Yeganejou, Scott Dick, and James Miller (University of Alberta) addresses the "black box" problem of deep neural networks by hybridising them with fuzzy logic. The core argument is that users will not trust or rely on AI systems whose decisions cannot be explained, and that fuzzy systems offer a natural interpretability mechanism.

The proposed architecture (termed "deep fuzzy system") uses a CNN as an automated feature extractor, passes the last convolutional layer's output to a fuzzy clustering algorithm (FCM or Gustafson–Kessel), and then uses Rocchio's algorithm for classification. An explanation mechanism is constructed by identifying the medoid of each fuzzy cluster and using guided backpropagation, Taylor decomposition, and layerwise relevance propagation (LRP) to generate saliency maps showing which image pixels are most relevant to each classification.

Experiments were conducted on three benchmark computer-vision datasets: MNIST (handwritten digits), Fashion MNIST (garment images), and CIFAR-10 (RGB objects).

## Key Findings

- The deep fuzzy classifier consistently achieves lower accuracy than the base CNN across all datasets and architectures, but the gap is modest (typically under 1.5 percentage points in better-performing configurations). [domain: computer vision / technical AI]
- Deep feature extraction substantially improves fuzzy classifier accuracy compared to applying the fuzzy classifier directly in the original image space. [domain: computer vision / technical AI]
- The fuzzy clustering approach generalises across multiple CNN architectures (LeNet variants, AlexNet, ResNets), indicating broad applicability. [domain: computer vision / technical AI]
- The GK clustering algorithm (hyperellipsoidal clusters) consistently outperforms FCM (hyperspherical clusters) for the benchmark datasets tested. [domain: computer vision / technical AI]
- The proposed explanation mechanism — saliency maps for cluster medoid representatives — provides intuitive visual accounts of correct and incorrect classifications on MNIST, with guided backpropagation yielding the most interpretable heat maps. [domain: computer vision / technical AI]
- The authors explicitly note that interpretability has not been formally evaluated with users and call for user studies to test whether explanations are comprehensible to non-expert populations. [domain: computer vision / technical AI]
- The paper references the EU "right to explanation" regulation as a key motivation for XAI research. [domain: policy / regulatory]

## Transparency Constructs

This paper operationalises [[explainability]] as a system design property, specifically through **interpretability-by-design** (making the classifier component inherently inspectable rather than adding a post-hoc overlay). The explanation mechanism produces:
- **Cluster-level explanations**: each fuzzy cluster has a medoid representative whose classification logic is visualisable.
- **Pixel-level saliency maps** (guided backpropagation, Taylor decomposition, LRP): showing which parts of an input image are most relevant to the predicted class.

This approach aligns with [[process-transparency]] — revealing how the model reaches its conclusion — rather than [[outcome-transparency]] (merely reporting the output).

The paper also touches on [[algorithmic-transparency]] in the broader sense, arguing that transparent models are necessary for verifiability, comparative model judgments, knowledge discovery, and legal compliance.

## Trust Constructs

The paper frames user trust as a precondition for adoption. The opening argument cites prior research showing that users will not act on decisions from a model they cannot explain, directly linking interpretability to [[behavioural-trust]] (willingness to use/rely on the model). The paper does not empirically measure trust; rather, it treats trust as the motivating problem that interpretability solves.

No formal user study is conducted, so claims about trust impact are theoretical/motivational rather than empirical.

## Relevance to Research Questions

**RQ1**: Contributes to conceptualisation and operationalisation of explainability/interpretability. The paper distinguishes interpretability-by-design from post-hoc explanation, and proposes cluster medoid saliency maps as a specific operationalisation. It frames the explainability–trust connection as foundational to deployment. (source: Yeganejou et al._Interpretable_Deep_Convolutional_Fuzzy_Classifier.txt)

**RQ2**: Implicitly addresses the transparency–trust relationship by arguing that users require explanations as a prerequisite for trust and adoption of AI decision support (citing Ribeiro et al. 2016, Caruana et al. 2015). The paper does not empirically test this relationship but treats it as established prior work. The accuracy–interpretability trade-off is quantified and found to be modest. (source: Yeganejou et al._Interpretable_Deep_Convolutional_Fuzzy_Classifier.txt)

**RQ3**: Not addressed. The paper is a technical ML contribution and does not consider user roles, expertise, or AI literacy.

## Related pages

- [[explainability]]
- [[algorithmic-transparency]]
- [[process-transparency]]
- [[behavioural-trust]]
- [[rq1-conceptualizations]]
- [[rq2-relationships]]
