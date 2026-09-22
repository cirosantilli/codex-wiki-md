<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the following precise form of the [Friedgut-Kalai sharp threshold theorem](../../../../../../friedgut-kalai-sharp-threshold-theorem.md). There is an absolute $C$ such that, for a nontrivial [transitive increasing event](../../../../../../transitive-increasing-event.md) $A\subseteq\{0,1\}^n$, $n\geq2$, and $0<\varepsilon<1/2$, its success [probability](../../../../../../probability.md) increases from $\varepsilon$ to $1-\varepsilon$ over an interval of length at most

$$
\boxed{\frac{C\log((1-\varepsilon)/\varepsilon)}{\log n}.}
$$

In particular, $\mu_p(A)>\varepsilon$ and $q-p\geq C\log((1-\varepsilon)/\varepsilon)/\log n$, with $p<q<1$, imply $\mu_q(A)>1-\varepsilon$. Here $\mu_p$ denotes independent bits equal to one with [probability](../../../../../../probability.md) $p$. Symmetry means invariance under a permutation group acting transitively on the $n$ coordinates, not necessarily invariance under all coordinate permutations.

Use the allowed weighted-cube influence theorem in this exact form: an absolute $c>0$ exists such that, for every $n\geq2$, $0<p<1$, and zero-one [Boolean function](../../../../../../boolean-function.md) of mean $u$ under $\mu_p$, some coordinate has pivotal probability at least $cu(1-u)\log n/n$. A coordinate's pivotal event is determined by the other coordinates and means that the two possible values of that coordinate give different outputs. This uniform form is a consequence of the weighted [Kahn-Kalai-Linial theorem](../../../../../../kahn-kalai-linial-theorem.md); it applies to nonsymmetric functions as well.

Write $u(p)=\mu_p(A)$. Differentiating the finite product expression for $u(p)$, one coordinate at a time, gives

$$
u'(p)=\sum_{i=1}^n\mathbb E_p[f(x^{i\to1})-f(x^{i\to0})]=\sum_{i=1}^n I_i^{(p)}(f).
$$

The last equality uses monotonicity, so each summand is the pivotal probability. This derives the [Margulis–Russo formula](../../../../../../margulis-russo-formula.md) in the normalization being used. Transitivity makes all the [influences](../../../../../../influence-of-a-variable.md) equal; applying the weighted influence theorem therefore yields

$$
u'(p)\geq c\,u(p)(1-u(p))\log n.
$$

Nontriviality ensures $0<u(p)<1$ throughout $(0,1)$. Dividing and integrating the derivative of the log odds gives

$$
\log\frac{u(q)}{1-u(q)}-\log\frac{u(p)}{1-u(p)}\geq c(q-p)\log n.
$$

At the two specified quantiles the left side is $2\log((1-\varepsilon)/\varepsilon)$. Taking $C=2/c$ proves the window bound and, with a strict starting inequality, the asserted strict final inequality. This is the [sharp threshold](../../../../../../sharp-threshold.md) conclusion, rather than an assumption about a discontinuous finite-$n$ probability curve.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
