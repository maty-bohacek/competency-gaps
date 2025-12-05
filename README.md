# Uncovering Competency Gaps in Large Language Models and Their Benchmarks

#### [Maty Bohacek](https://www.matybohacek.com), [Nino Scherrer](https://ninodimontalcino.github.io), [Nicholas Dufour](), [Thomas Leung](), [Christoph Bregler](), [Stephanie C.Y. Chan](https://scychan.github.io/)

The evaluation of large language models (LLMs) relies heavily on standardized benchmarks. These benchmarks provide useful aggregated metrics for a given capability, but those aggregated metrics can obscure (i) particular sub-areas where the LLMs are weak ("model gaps") and (ii) imbalanced coverage in the benchmarks themselves ("benchmark gaps"). We propose a new method that uses sparse autoencoders (SAEs) to automatically uncover both types of gaps. By extracting SAE concept activations and computing saliency-weighted performance scores across benchmark data, the method grounds evaluation in the model's internal representations and enables comparison across benchmarks. As examples demonstrating our approach, we applied the method to two popular open-source models and ten benchmarks. We found that these models consistently underperformed on concepts that stand in contrast to sycophantic behaviors (e.g., politely refusing a request or asserting boundaries) and concepts connected to safety discussions. These model gaps align with observations previously surfaced in the literature; our automated, unsupervised method was able to recover them without manual supervision. We also observed benchmark gaps: many of the evaluated benchmarks over-represented concepts related to obedience, authority, or instruction-following, while missing core concepts that should fall within their intended scope. In sum, our method offers a representation-grounded approach to evaluation, enabling concept-level decomposition of benchmark scores. Rather than replacing conventional aggregated metrics, CG complements them by providing a concept-level decomposition that can reveal why a model scored as it did and how benchmarks could evolve to better reflect their intended scope.

> Website — [Paper](TBD) — [Contact us](mailto:email@example.com)
>
> *Under review*

Code coming soon.

## Citation

If you find our work useful, please consider citing our paper.

```bibtex
@inproceedings{tbd2026competencygaps,
  title={Uncovering Competency Gaps in Large Language Models and Their Benchmarks},
  author={TBD},
  booktitle={TBD},
  year={TBD}
}
