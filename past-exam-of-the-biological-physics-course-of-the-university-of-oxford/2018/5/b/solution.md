<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [single-block DNA zipper partition function](../../../../single-block-dna-zipper-partition-function.md) retains one contiguous paired block and ignores multiple separated bubbles. A block of $j\ge1$ paired bases can start at any of $N-j+1$ positions. Its first pair has initiation weight $\kappa$, and the remaining $j-1$ pairs each have propagation weight $s$. Thus

$$
\boxed{q=\kappa\sum_{j=1}^N(N-j+1)s^{j-1}.}
$$

The source's symbol $k$ in the displayed expressions denotes the same initiation constant as $\kappa$, not Boltzmann's constant. Association and other reference-state factors are absorbed into that statistical weight; the model treats the propagation weights as uniform despite the actual sequence's different bases.

Put $r=j-1$. Since $N-r$ counts how many terms of a finite [geometric series](../../../../geometric-series.md) contain $s^r$,

$$
\sum_{r=0}^{N-1}(N-r)s^r=\sum_{\ell=0}^{N-1}\sum_{r=0}^{\ell}s^r
=\frac1{s-1}\left[\frac{s(s^N-1)}{s-1}-N\right].
$$

Consequently

$$
\boxed{q=\frac{\kappa[s^{N+1}-(N+1)s+N]}{(s-1)^2}\quad(s\ne1).}
$$

The apparent singularity is removable: at $s=1$, the original sum gives $q=\kappa N(N+1)/2$, which is $45\kappa$ for these nine bases.

At $s\gg1$, the longest block dominates:

$$
\boxed{q\simeq\kappa s^{N-1}\left(1+\frac2s+\frac3{s^2}+\cdots\right),\qquad
q_{N=9}\simeq\kappa s^8.}
$$

Conditional on at least one pair, the fully paired [probability](../../../../probability.md) approaches one, with leading correction of order $2/s$. If a fully unpaired reference state of weight one is included, the full [partition function](../../../../canonical-partition-function.md) is $Q=1+q$, so a large propagation constant alone does not guarantee predominant duplex if $\kappa s^{N-1}$ is still very small.

The given sequence contains five A–T and four G–C pairs when fully complementary. Real duplex [stability](../../../../stability-of-a-numerical-method.md) also depends strongly on stacking, sequence context, [salt](../../../../salt-chemistry.md) and [temperature](../../../../temperature-split.md); it cannot be calculated just by counting two versus three [hydrogen bonds](../../../../hydrogen-bond.md). All else comparable, sequences with greater duplex propagation [stability](../../../../stability-of-a-numerical-method.md) resist bubble opening more strongly, while easier-to-open, often A–T-rich start-site regions facilitate initiation. The homogeneous-$s$ zipper demonstrates that principle but does not resolve a quantitative sequence-specific melting profile or polymerase's active stabilization of the open state.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
