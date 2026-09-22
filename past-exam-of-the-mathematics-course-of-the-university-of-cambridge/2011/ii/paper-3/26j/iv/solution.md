<h1 id="26j/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $P=N(t)\sim\operatorname{Poisson}(x)$, where $x=\lambda t$. Deleting odd arrivals leaves $M=\lfloor P/2\rfloor$. Put $Q=\mathbf1_{\{P\text{ odd}\}}$, so $M=(P-Q)/2$. From the [probability generating function](../../../../../../probability-generating-function.md) $\mathbb Ez^P=e^{x(z-1)}$,

$$
q:=\mathbb EQ=\frac{1-e^{-2x}}2,\qquad\mathbb E[P(-1)^P]=-xe^{-2x},\qquad\mathbb E(PQ)=\frac{x+xe^{-2x}}2.
$$

Thus $\operatorname{Var}Q=(1-e^{-4x})/4$ and $\operatorname{Cov}(P,Q)=xe^{-2x}$. Therefore

$$
\boxed{\mathbb EM=\frac{2x+e^{-2x}-1}{4},\qquad\operatorname{Var}M=\frac{4x-8xe^{-2x}-e^{-4x}+1}{16}.}
$$

To establish strict underdispersion for every $x>0$, subtract the mean:

$$
16(\operatorname{Var}M-\mathbb EM)=f(x):=5-4x-(8x+4)e^{-2x}-e^{-4x}.
$$

Here $f(0)=0$ and $f'(x)=4[-1+4xe^{-2x}+e^{-4x}]<0$ for $x>0$, because $4xe^{-2x}<1-e^{-4x}$ is equivalent to $2x<\sinh(2x)$. Hence

$$
\boxed{\operatorname{Var}M(t)<\mathbb EM(t)\quad(t>0,\lambda>0),}
$$

which excludes a doubly-stochastic Poisson representation by part (iii).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [26J](../../26j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
