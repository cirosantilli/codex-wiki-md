<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[pleiotropy](../../../../pleiotropy.md) means that a single [gene](../../../../gene.md) or [genetic variant](../../../../genetic-variant.md) influences more than one distinguishable [phenotypic trait](../../../../phenotypic-trait.md). Its evolutionary consequence depends on the directions and magnitudes of those effects and on how they affect [genotype fitness](../../../../genotype-fitness.md). It must be distinguished from [genetic linkage](../../../../genetic-linkage.md), in which different causal [genetic loci](../../../../genetic-locus.md) travel together, and from [epistasis](../../../../epistasis.md), in which the effect of one [allele](../../../../allele.md) depends on another. **[pleiotropy](../../../../pleiotropy.md) can constrain [adaptation](../../../../adaptation.md), facilitate coordinated change, and maintain trade-offs; its sign is not intrinsically negative.**

For a small change in a [phenotypic trait](../../../../phenotypic-trait.md) [vector](../../../../vector.md) $\mathbf z$, write its effect as $\mathbf a$ and define the [phenotypic selection gradient](../../../../phenotypic-selection-gradient.md) $\boldsymbol\beta=\nabla_{\mathbf z}\log w$. A first-order [Taylor polynomial](../../../../taylor-polynomial.md) gives

$$
\Delta\log w\approx\boldsymbol\beta^{\mathsf T}\mathbf a.
$$

A [mutation](../../../../mutation.md) that improves one component can therefore be harmful overall if its other effects oppose sufficiently strong [natural selection](../../../../natural-selection.md). For an illustrative two-trait case, $\boldsymbol\beta=(1,1)$ and $\mathbf a=(0.2,-0.3)$ give $\Delta\log w\approx-0.1$. With $\mathbf a=(0.2,0.1)$, the same approximation gives $0.3$. What matters is the full effect [vector](../../../../vector.md), not whether the [mutation](../../../../mutation.md) has been called “large” or “pleiotropic”. Near an optimum the first-order term can vanish, making curvature important.

This geometric constraint is explicit in [Fisher's geometric model](../../../../fisher-s-geometric-model.md). Put the optimum at the origin and let $\mathbf z$ denote the current displacement. A step $\mathbf a$ improves an isotropic quadratic measure of [genotype fitness](../../../../genotype-fitness.md) exactly when

$$
\|\mathbf z+\mathbf a\|^2<\|\mathbf z\|^2
\quad\Longleftrightarrow\quad
2\mathbf z\mathbin{\cdot}\mathbf a+\|\mathbf a\|^2<0.
$$

A step toward improvement in one component may damage many other components. In models where a step has random direction across many independent selected dimensions, the set of favorable directions can become restricted: this motivates a [cost of complexity](../../../../cost-of-complexity.md). But the prediction depends on how total step size, per-trait effect size and the number of affected [phenotypic traits](../../../../phenotypic-trait.md) scale. Organismal complexity is not automatically equal to the number of dimensions affected by every [mutation](../../../../mutation.md).

At the population level, the [multivariate breeder's equation](../../../../multivariate-breeder-s-equation.md) is

$$
\Delta\overline{\mathbf z}=\mathbf G\boldsymbol\beta,
$$

where $\mathbf G$ is the [additive genetic covariance matrix](../../../../additive-genetic-covariance-matrix.md). This is a local approximation under the relevant inheritance and weak-selection assumptions.[Evolution 33, pp. 402–416; multivariate response to selection](../../../../quantitative-genetic-analysis-of-multivariate-evolution-applied-to-brain-body-size-allometry-by-russell-lande.md) The off-diagonal entries cause correlated responses. For example,

$$
\mathbf G=\begin{pmatrix}1&-0.8\\-0.8&1\end{pmatrix},\qquad
\boldsymbol\beta=\begin{pmatrix}1\\1\end{pmatrix}
\quad\Longrightarrow\quad
\Delta\overline{\mathbf z}=\begin{pmatrix}0.2\\0.2\end{pmatrix}.
$$

There is abundant [genetic variance](../../../../genetic-variance.md) for each [phenotypic trait](../../../../phenotypic-trait.md) separately, yet their negative [genetic covariance](../../../../genetic-covariance.md) slows simultaneous increase. For $\boldsymbol\beta=(1,-1)^{\mathsf T}$, the response instead becomes $(1.8,-1.8)^{\mathsf T}$: the same covariance facilitates this direction. A singular $\mathbf G$ can make an instantaneous response unavailable, but present covariance does not establish an eternal constraint. Moreover, [genetic linkage](../../../../genetic-linkage.md) can also produce [genetic covariance](../../../../genetic-covariance.md); estimating $\mathbf G$ alone does not demonstrate [pleiotropy](../../../../pleiotropy.md).

[antagonistic pleiotropy](../../../../antagonistic-pleiotropy.md) arises when effects favor different outcomes in different components of [genotype fitness](../../../../genotype-fitness.md), environments, sexes or life stages. An [allele](../../../../allele.md) that increases early reproduction but reduces late survival can be favored if its early benefit receives greater reproductive weighting. This provides a possible route to [senescence](../../../../senescence.md), without implying that deterioration is itself selected for. Sex-specific benefits and costs can produce [sexual antagonism](../../../../sexual-antagonism.md). Such conflicts may maintain variation under some combinations of [dominance](../../../../dominance-genetics.md), demography and environmental variation, but opposite effects alone do not guarantee a protected [polymorphism](../../../../polymorphism.md). The invasion success of each alternative when rare must be checked.

[pleiotropy](../../../../pleiotropy.md) can also promote [adaptation](../../../../adaptation.md) by coordinating changes that work well together. A developmental regulator can change a group of interacting structures; a single physiological change can improve several measures of performance. [natural selection](../../../../natural-selection.md) may favor [developmental modularity](../../../../developmental-modularity.md), tissue-specific regulation or [gene duplication](../../../../gene-duplication.md) when they reduce costly coupling. The pelvic [enhancer](../../../../enhancer.md) example in question 2 illustrates how [cis-regulatory evolution](../../../../cis-regulatory-evolution.md) can localize an effect; it does not establish a universal privilege of regulatory over coding [mutations](../../../../mutation.md).

Empirical measurement requires care. Screens of yeast, nematode and mouse mutants found strongly modular relationships between [genes](../../../../gene.md) and measured [phenotypic traits](../../../../phenotypic-trait.md), challenging assumptions of universal equal-effect [pleiotropy](../../../../pleiotropy.md).[Results on the degree of pleiotropy and modularity; Figures 1–3](../../../../genomic-patterns-of-pleiotropy-and-the-evolution-of-complexity-by-zhi-wang-and-others.md) A deletion can nevertheless have more severe and widespread effects than a naturally segregating regulatory [allele](../../../../allele.md); unmeasured environments and [phenotypic traits](../../../../phenotypic-trait.md) hide effects, whereas multiple correlated measurements can inflate apparent dimensionality. To test causal [pleiotropy](../../../../pleiotropy.md), introduce the same precise [genetic variant](../../../../genetic-variant.md) into matched [genetic backgrounds](../../../../genetic-background.md), measure multiple prespecified [phenotypic traits](../../../../phenotypic-trait.md) across environments and life stages, and use recombinant or edited lines to exclude a neighboring causal [genetic locus](../../../../genetic-locus.md). Assay [genotype fitness](../../../../genotype-fitness.md) as well as convenient laboratory [phenotypic traits](../../../../phenotypic-trait.md). **The evolutionary constraint is the alignment between available heritable effects and current selection, not the mere count of affected [phenotypic traits](../../../../phenotypic-trait.md).**

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 4](../../paper-4-split.md)
3. [2025](../../split.md)
4. [Past exam of the genetics course of the University of Cambridge](../../../split.md)
5. [Genetics course of the University of Cambridge](../../../../genetics-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
