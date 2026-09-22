<h1 id="34d/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Differentiating the [grand potential](../../../../../../../grand-potential.md) gives

$$
N=kVT^bf'(y),\qquad S=kVT^b[(b+1)f(y)-yf'(y)],\qquad
\frac SN=(b+1)\frac{f(y)}{f'(y)}-y.
$$

A reversible adiabatic change in an isolated gas keeps $S$ and $N$ fixed. To infer constant $y$, one must check that this ratio is one-to-one, rather than merely assuming it.

Put $q=y/k$, $n(x)=1/(1+e^{x-q})$, $F_j=\int_0^\infty x^jn(x)\,dx$ and $M_j=\int_0^\infty x^{a+j}n(x)(1-n(x))\,dx$ for $j=0,1,2$. [Integration by parts](../../../../../../../integration-by-parts.md) gives $M_1=bF_a$ and $M_2=(b+1)F_{a+1}$, and

$$
\frac S{kN}=\frac{b+1}{b}\frac{F_{a+1}}{F_a}-q,\qquad
\frac d{dq}\frac S{kN}=b\left(1-\frac{M_0M_2}{M_1^2}\right)<0.
$$

The strict inequality is the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) for the positive weight $x^an(x)(1-n(x))$, since $x$ is not constant on its support. This proves [strict monotonicity of Fermi gas entropy per particle](../../../../../../../strict-monotonicity-of-fermi-gas-entropy-per-particle.md) and hence $\mu/T$ is constant. Then $N=kVT^bf'(y)$ gives $VT^b$ constant, and $P=kT^{b+1}f(y)$ gives

$$
\boxed{VT^c=\text{constant},\quad PV^d=\text{constant},\qquad c=a+1,\quad d=\frac{a+2}{a+1}.}
$$

This [adiabatic scaling of a Fermi gas with power-law density of states](../../../../../../../adiabatic-scaling-of-a-fermi-gas-with-power-law-density-of-states.md) concerns positive temperature; the zero-temperature [limit](../../../../../../../limit-of-a-function.md) is a separate limiting case.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [34D](../../../34d.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
