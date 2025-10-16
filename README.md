# Uncovering Competency Gaps in Large Language Models and Their Benchmarks

#### [Maty Bohacek](https://www.matybohacek.com), [Nino Scherrer](https://ninodimontalcino.github.io), [Nicholas Dufour](), [Thomas Leung](), [Christoph Bregler](), [Stephanie C.Y. Chan](https://scychan.github.io/)

The evaluation of large language models (LLMs) relies heavily on standardized benchmarks. While these provide useful aggregated metrics, they can obscure particular sub-areas where LLMs are weak ("model gaps") and imbalanced coverage in the benchmarks themselves ("benchmark gaps"). This paper proposes a method called **Competency Gaps (CG)**, which uses sparse autoencoders (SAEs) to automatically uncover both types of gaps. By extracting SAE concept activations and computing saliency-weighted performance scores, our method grounds evaluation in the model's internal representations and enables comparison across models and benchmarks. We apply this method to popular open-source models and diverse benchmarks, uncovering meaningful imbalances. Our findings show that popular benchmarks often miss concepts central to their intended scope (e.g., logical or social reasoning) while over-representing concepts related to authority and instruction-following. The method also automatically surfaces model weaknesses anecdotally noted in prior work (e.g., reasoning with time, palindromes, and arithmetic), enabling developers to identify and address shortcomings in how model capabilities are currently assessed.

> [Website](TBD) — [Paper](TBD) — [Contact us](mailto:email@example.com)
>
> *Under review*

## Modules

This repository is organized into three main modules. To replicate our analysis or apply it to a new model, please use them in the order presented.

### 1. Competency Gap (CG) Calculation

This module contains the core implementation of our SAE-based method. It includes scripts to process benchmark data, extract concept activations, and compute the final benchmark gap and model gap scores as described in the paper.

### 2. Gap Analysis & Visualization

This module includes a collection of notebooks and scripts for analyzing the results from the first module. It allows you to identify over/underrepresented concepts, find the best/worst performing concepts for a model, and generate the plots and tables presented in our paper.

### 3. Interactive Exploratory Tool

We provide the source code for the web-based exploratory tool that allows for interactive inspection of benchmark coverage and model performance on a per-concept basis. This tool was used to surface many of the qualitative insights in our work.

## Getting Started

To get started, clone the repository and set up the required environment. We recommend using Python 3.10.

```shell
git clone [https://github.com/your-username/competency-gaps.git](https://github.com/your-username/competency-gaps.git)
cd competency-gaps
pip install -r requirements.txt
