---
layout: project
type: project
image: img/project1.png
title: "Text to Speech Diffusion Model"
date: 10-2024 to 02-2025
published: true
labels:
  - Diffusion
  - Llama3.2
  - GradTTS
summary: "Developed a text-to-speech diffusion model to process audio from text data. Fine-tuning the diffusion model using these datasets. Performing an extensive evaluation of the model to determine its efficacy, supervised by Dr. Mojtaba Nayyeri"
---

<img class="img-fluid" src="../img/text2speechBanner.png">

We have developed a text-to-speech diffusion model to process audio from text data. We performed fine-tuning the diffusion model using the dataset from IIT Madras and performed an extensive evaluation of the model to determine its efficacy.

Text-to-Speech (TTS) systems have seen significant advancements with the advent of deep learning,
 enabling natural and expressive voice synthesis. Diffusion probabilistic models, known for their
 f
 lexibility and ability to model complex data distributions, have emerged as a powerful framework in
 generative modeling. This paper presents a novel approach to TTS synthesis using a diffusion-based
 model inspired by Grad-TTS [1], leveraging the strengths of diffusion processes to achieve high
quality speech synthesis. Our method incorporates a noise-to-speech generative process conditioned
 on text embeddings, allowing the model to iteratively refine noisy audio representations in form of
 mel-spectrograms into natural speech. We explore architectural improvements and optimizations to
 enhance the efficiency and performance of the Grad-TTS [1]framework, addressing limitations such
 as feature ignorance. Extensive evaluations on publicly available datasets demonstrate that our model
 achieves significant results in terms of naturalness, intelligibility, and speaker consistency, while
 maintaining competitive synthesis speeds. The proposed approach highlights the potential of diffusion
based models in advancing TTS technologies, paving the way for more robust and adaptable systems
 in real-world applications. 

  Generative models have become a cornerstone of modern artificial intelligence research, with applications spanning
 across diverse fields. From large language models (LLMs) such as GPTs to diffusion models, their ability to generate
 high-quality outputs has driven advancements in various domains. Among these, Text-to-Speech (TTS) systems have
 seen remarkable improvements, particularly in generating clear, natural, and expressive speech while maintaining fast
 inference times.
 Existing TTS models, such as Google TTS, are widely used in everyday life for applications ranging from virtual
 assistants and accessibility tools to content creation and customer service. These systems typically consist of two
 primary components:
 Feature Generator: This module converts text embeddings into time-frequency domain acoustic representations, such as
 mel-spectrograms.
 Vocoder: The vocoder synthesizes raw audio waveforms from the acoustic features, producing the final speech output.
 While current models perform well in many scenarios, challenges such as pronunciation errors, latency, naturalness,
 and waveform synthesis quality remain critical areas of improvement. Addressing these limitations, we propose an
 innovative TTS architecture that integrates cutting-edge techniques which takes into account the accent of the speaker
 and we do the training on the specific accent of the speaker for inference we use many state-of-Art models, including
A PREPRINT- FEBRUARY 19, 2025
 LLama 3.2 [2] for text generation, Glow-TTS [3], for feature extraction, and HiFi-GAN [4] for high-quality waveform
 synthesis.
 Glow-TTS leveraging normalizing flows, provides an efficient non-autoregressive solution for feature generation,
 reducing latency and pronunciation issues. Additionally, HiFi-GAN, a state-of-the-art vocoder, ensures high-fidelity
 waveform synthesis with minimal computational overhead. Together with a post-processing block to refine the generated
 waveforms, the proposed architecture aims to set a new benchmark in TTS quality and efficiency


