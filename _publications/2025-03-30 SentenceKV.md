---
title: "SentenceKV: Efficient LLM Inference via Sentence-Level Semantic KV Caching"
collection: publications
permalink: /publication/2025-03-30 SentenceKV
excerpt: "Yuxuan Zhu, Ali Falahati, David H Yang, Mohammad Mohammadi Amiri.<br/><img src='/images/sentencekv.png' width='600'>"
# excerpt: ''
date: 2025-03-30
venue: 'Arxiv'
paperurl: 'https://arxiv.org/abs/2504.00970'
# citation: 'Zhong Li, Yuxuan Zhu, Matthijs Van Leeuwen'
---

Large language models face significant computational and memory challenges when processing long contexts. During inference, efficient management of the key-value (KV) cache, which stores intermediate activations for autoregressive generation, is critical to reducing memory overhead and improving computational efficiency. Traditional token-level efficient KV caching methods overlook semantic information, treating tokens independently without considering their semantic relationships. Meanwhile, existing semantic-preserving KV cache management approaches often suffer from substantial memory usage and high time-to-first-token. To address these limitations, we propose SentenceKV, a novel sentence-level semantic KV caching approach designed to enhance inference efficiency while preserving semantic coherence. During prefilling, SentenceKV groups tokens based on sentence-level semantic similarity, compressing sentence representations into concise semantic vectors stored directly on the GPU, while individual KV pairs are offloaded to CPU. During decoding, SentenceKV generates tokens by selectively retrieving semantically relevant sentence-level KV entries, leveraging the semantic similarity between the prefilling-stage semantic vectors and decoding-stage queries. This ensures efficient and contextually accurate predictions, minimizing the loading of redundant or irrelevant data into GPU memory and significantly reducing memory overhead while maintaining stable inference latency, even for extremely long contexts. Extensive evaluations on benchmarks including PG-19, LongBench, and Needle-In-A-Haystack demonstrate that SentenceKV significantly outperforms state-of-the-art methods in both efficiency and memory usage, without compromising model accuracy.
