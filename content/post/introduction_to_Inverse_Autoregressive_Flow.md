---
title: "Introduction to Inverse Autoregressive Flow (IAF)"
description: ""
tags: ["normalizing flow"]
date: 2017-12-18T01:16:43+08:00
topics: ["Paper introduction","machine learning"]
draft: false
---

今天我們要來探討[Improving Variational Inference with Inverse Autoregressive Flow](https://arxiv.org/abs/1606.04934)這篇論文，而這是我第一次撰寫介紹文，若大家在閱讀時有發現錯誤或有任何疑問，歡迎在下方的討論區提出，謝謝大家(希望大家鞭小力點XD)。討論這篇論文的原因主要是為了延續下一篇介紹文[Introduction to Parallel Wavenet](/post/introduction_to_parallel_wavenet)，[Parallel Wavenet](https://arxiv.org/abs/1711.10433)目前應該算是語音合成眾多技術中的"State of the art"，而在GAN的相關研究近乎氾濫的情況下，Parallel Wavenet算是一股清流，透過Probability Density Distillation，改善第一代[Autoregressive Model -- Wavenet](https://arxiv.org/abs/1609.03499)需要接續地生成一個個語音samples (sequential generation)的問題。而Parallel Wavenet希望運用IAF (Inverse Autoregressive Flow)能夠parallel sample的特性，改善語音合成的速度。

## 前情提要
為了讓L.V.0的初心者也能從零開始踏入Machine Learning這個異世界，所以我簡要地介紹幾個和這篇論文息息相關的名詞和概念

* Posterior
* Variational Inference of Posterior over Latent Variable
* Normalizing Flow
* Autoregreesive model



