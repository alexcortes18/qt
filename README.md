# Opinion Summarization with Quantized Transformers

This repo contains the data and code for the paper:

> **Extractive Opinion Summarization in Quantized Transformer Spaces**,<br/>
> Stefanos Angelidis, Reinald Kim Amplayo, Yoshihiko Suhara, Xiaolan Wang, Mirella Lapata, <br/>
> _To appear: In Transactions of the Association for Computational Linguistics (TACL)_.<br/>
> [arXiv]()

## The SPACE corpus

The paper introduces SPACE (__S__ummaries of __P__opular and __A__spect-specific
__C__ustomer __E__xperiences), a large-scale opinion summarization benchmark for
the evaluation of unsupervised summarizers.

SPACE is built on TripAdvisor hotel reviews and includes a training set of
approximately 1.1 million reviews for over 11 thousand hotels.

For evaluation, we created a collection of human-written, abstractive opinion
summaries for 50 hotels, including high-level general summaries and aspect
summaries for six popular aspects: building, cleanliness, food, location, rooms,
and service. 

You can download the corpus from [this google drive url](https://drive.google.com/u/0/uc?id=1C6SaRQkas2B-9MolbwZbl0fuLgqdSKDT&export=download).

## The Quantized Transformer

The Quantized Transformer (QT) is inspired by Vector-Quantized Variational
Autoencoders, which we repurpose for popularity-driven summarization. It uses a
clustering interpretation of the quantized space and a novel extraction
algorithm to discover popular opinions among hundreds of reviews, a significant
step towards opinion summarization of practical scope. In addition, QT enables
controllable summarization without further training, by utilizing properties of
the quantized space to extract aspect-specific summaries.
