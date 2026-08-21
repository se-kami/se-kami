# Hi, I'm Karlo 👋

I explore machine learning by turning papers and ideas into working PyTorch
implementations. My main interest is **domain adaptation**: training models that
can transfer what they learn from one dataset or visual domain to another, even
when labeled target data is limited or unavailable.

Alongside domain adaptation, this profile collects experiments in natural
language processing, foundational deep-learning architectures, reusable dataset
loaders, and the small tools that make up my Linux development environment.

## Current focus

- Unsupervised and adversarial domain adaptation
- Reproducing machine-learning papers in PyTorch
- Facial-expression recognition under uncertainty
- Character-level language models and Transformer-based translation
- Reusable datasets, training templates, and experiment utilities

My path into the field has moved through **mathematics → physics → data science
→ machine learning → deep learning**. That progression still shapes how I work:
understand the idea, implement the mechanism, and test it on a concrete problem.

## Featured domain-adaptation projects

### [DANN — Domain-Adversarial Neural Networks](https://github.com/se-kami/dann)

An unofficial PyTorch implementation of *Unsupervised Domain Adaptation by
Backpropagation*. DANN learns features that remain useful for the source task
while becoming difficult for a domain classifier to distinguish. A gradient
reversal layer makes this adversarial objective trainable with ordinary
backpropagation.

The repository includes configurations and results for digit-transfer tasks such
as MNIST → MNIST-M, SVHN → MNIST, and synthetic digits → SVHN or GTSRB. MNIST
and SVHN can be downloaded automatically; other datasets are configured through
the project's data directory.

### [ADDA — Adversarial Discriminative Domain Adaptation](https://github.com/se-kami/ADDA)

A PyTorch implementation of ADDA built around four components: a source feature
extractor, a target feature extractor, a classifier, and a domain discriminator.
Training happens in two stages. First, the source encoder and classifier learn
from labeled source images. Then, adversarial training aligns the target encoder
with the source representation before the target images are classified.

The included experiments cover transfers between MNIST, USPS, and SVHN.

### [LAMDA — Label Matching Deep Domain Adaptation](https://github.com/se-kami/lamda)

An unofficial implementation of LAMDA, a method designed to handle both domain
shift and label shift. The repository provides experiment configurations for
Office-31 and digit adaptation tasks, visualizes learned embeddings, records
training runs, and reports benchmark results alongside the original paper.

### [Domain-adaptation datasets](https://github.com/se-kami/da_datasets)

Reusable PyTorch dataset loaders for common adaptation benchmarks. The package
provides a shared interface for domains and split strategies, including full,
train/test, list-based, and *n*-shot splits.

Supported collections include:

- Digits: MNIST, MNIST-M, SVHN, Synthetic Digits, and USPS
- ImageCLEF
- Natural Scene datasets based on CIFAR and STL
- Office-31 and Office-Home
- VisDA 2017

## Facial-expression learning

### [CAFEL — Confidence-Aware Uncertainty Balancing](https://github.com/se-kami/cvpr-2023-abaw-expr)

A collaborative facial-expression recognition project for the CVPR 2023
Affective Behavior Analysis in-the-Wild Expression Classification Challenge. The
implementation combines a modified POSTER_V2 model with an anchor-label
correction network to make learning more robust to uncertainty in facial
expression labels.

The repository includes training instructions, pretrained-backbone integration,
configuration for the Aff-Wild2 dataset, an architecture overview, and reported
F1 results.

## Natural language processing

The [NLP collection](https://github.com/se-kami/NLP) uses PyTorch and torchtext
to explain language-modeling ideas through compact, practical exercises:

- RNN tasks that demonstrate when recurrent memory is—and is not—needed
- Character-level name classification by nationality
- Character-level name generation conditioned on a language
- RNN, LSTM, and Transformer encoder/decoder experiments
- Neural machine translation with tokenization, vocabularies, padding, masking,
  teacher-forced training, and autoregressive inference

These projects emphasize the full path from raw text and batching to model
training and generation, rather than treating preprocessing as a black box.

## Paper implementations and learning projects

The [paper implementation collection](https://github.com/se-kami/papers) contains
small PyTorch studies of influential architectures and optimization methods:

- [Adam](https://github.com/se-kami/papers/tree/master/adam)
- [AlexNet](https://github.com/se-kami/papers/tree/master/alexnet)
- [EfficientNet](https://github.com/se-kami/papers/tree/master/efficientnet)
- [InceptionNet](https://github.com/se-kami/papers/tree/master/inceptionnet)
- [LeNet](https://github.com/se-kami/papers/tree/master/lenet)
- [Multiplicative LSTM](https://github.com/se-kami/papers/tree/master/m-lstm)
- [ResNet](https://github.com/se-kami/papers/tree/master/resnet)
- [Transformer / Attention Is All You Need](https://github.com/se-kami/papers/tree/master/attention-is-all-you-need)
- [VGG](https://github.com/se-kami/papers/tree/master/vgg)
- [Vision Transformer](https://github.com/se-kami/papers/tree/master/vit)

The separate [GAN repository](https://github.com/se-kami/GAN) implements the
original *Generative Adversarial Nets* paper and includes a visualization of the
generator's training progress.

For reusable building blocks, the
[PyTorch collection](https://github.com/se-kami/pytorch-collection) gathers
training snippets, templates, and small examples that can be adapted for new
experiments.

## Development environment

I also keep my daily Linux setup in public repositories. It is intentionally
small and keyboard-driven:

- **Shell:** [Zsh utilities](https://github.com/se-kami/shell-utils)
- **Editor:** [Neovim configuration](https://github.com/se-kami/nvim)
- **Terminal:** [st configuration](https://github.com/se-kami/st)
- **Window manager:** [dwm](https://github.com/se-kami/dwm),
  [dmenu](https://github.com/se-kami/dmenu), and
  [dwmblocks modules](https://github.com/se-kami/dwmblocks-modules)
- **Linux:** [Artix installation notes and scripts](https://github.com/se-kami/artix-install)

## Get in touch

- [GitHub](https://github.com/se-kami)
- [LinkedIn](https://www.linkedin.com/in/%C5%A1ekarlo/)
- [Email](mailto:serbetar.karlo.p@protonmail.com)

If you are interested in domain adaptation, PyTorch paper implementations, or
practical deep-learning experiments, feel free to explore the repositories or
get in touch.
