<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A unitary family with the required [Weyl relations](../../../../../../weyl-relations.md) is

$$
\boxed{(W(x,y)f)(t)=e^{ixy+2iyt}f(t+x).}
$$

Translations preserve the $L^2$ [norm](../../../../../../norm.md) and the multiplier has modulus one. Multiplication of two such operators leaves the phase $x_1y_2-y_1x_2$ after extracting $W(x_1+x_2,y_1+y_2)$, proving the relation. Translation and modulation are strongly continuous, first on compactly supported [smooth function](../../../../../../smooth-function.md)s by direct estimates, then on all of $L^2$ by density and unitarity.

If a [bounded operator](../../../../../../continuous-linear-operator.md) $A$ commutes with all $W$, it commutes with translations and every modulation $e^{2iyt}$. The [spectral theorem](../../../../../../spectral-theorem.md) for the multiplication coordinate therefore makes it commute with all bounded multiplication operators and interval projections. One can see its form directly: on a finite interval $I$, set $h_I=A1_I$. For bounded $\phi$ supported in $I$, commutation gives $A\phi=\phi h_I$. Testing characteristic functions shows $|h_I|\leq\|A\|$ almost everywhere. On increasing intervals these functions agree on overlaps and yield a single $h\in L^\infty$ with $A=M_h$.

Commutation with translations says $h(t+x)=h(t)$ almost everywhere for every $x$. Convolving with a smooth [approximate identity](../../../../../../approximate-identity.md) produces [smooth function](../../../../../../smooth-function.md)s invariant under every translation, hence constants. Passing to the local $L^1$ limit makes $h$ constant almost everywhere. Therefore **$A$ is a scalar operator**, and the unitary family acts irreducibly.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
