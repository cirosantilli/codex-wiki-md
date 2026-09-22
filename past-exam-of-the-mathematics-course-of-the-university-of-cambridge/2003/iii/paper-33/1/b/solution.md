<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The multidimensional [Itô formula](../../../../../../ito-s-lemma.md) for continuous [semimartingales](../../../../../../semimartingale.md) states that a $C^2$ transformation has first-order stochastic and finite-variation integrals plus one-half its Hessian contracted with the [quadratic covariations](../../../../../../quadratic-covariation.md). A continuous [finite-variation process](../../../../../../finite-variation-process.md) has zero [quadratic variation](../../../../../../quadratic-variation.md) and zero quadratic covariation with a continuous local martingale. Thus in the present case

$$
f(M_t,A_t)=f(M_0,A_0)+\int_0^t f_x(M_s,A_s)\,dM_s+\int_0^t f_y(M_s,A_s)\,dA_s+\frac12\int_0^t f_{xx}(M_s,A_s)\,d[M]_s.
$$

The first integrand is continuous adapted, hence [predictable](../../../../../../predictable-process.md), and locally bounded by stopping the two coordinate paths on exiting compact sets. The standard construction of the [Itô integral](../../../../../../ito-integral.md) then makes this integral a zero-starting [continuous local martingale](../../../../../../continuous-local-martingale.md). The remaining integrals are pathwise [Lebesgue-Stieltjes integrals](../../../../../../lebesgue-stieltjes-integration.md). On each compact time interval their integrands are bounded along the continuous paths, so their total variations are bounded by a constant times $V_t(A)+[M]_t$, which is finite. Therefore the normalized terms are

$$
\boxed{M_t^f=f(M_0,A_0)+\int_0^t f_x(M_s,A_s)\,dM_s,\qquad A_t^f=\int_0^t f_y(M_s,A_s)\,dA_s+\frac12\int_0^t f_{xx}(M_s,A_s)\,d[M]_s.}
$$

The process $A^f$ is continuous adapted of finite variation and $A_0^f=0$. When $f(M_0,A_0)$ is integrable, $M^f$ is a local martingale in the definition of part (a). Uniqueness follows from part (a): the difference of two normalized decompositions is both a continuous local martingale and a continuous finite-variation process starting at zero, hence vanishes.

**An initial-value qualification is necessary under that definition.** The printed assumptions do not themselves guarantee $\mathbb E|f(M_0,A_0)|<\infty$. Take $M=0$, $A_t=G$ with $G$ a standard [normal random variable](../../../../../../gaussian-random-variable.md) known at time zero, and $f(x,a)=e^{a^2}$. All path assumptions hold, but $\mathbb E e^{G^2}=\infty$. Any decomposition with $A_0^f=0$ would force the nonintegrable value $M_0^f=e^{G^2}$, contradicting the local-martingale definition. Without an integrability hypothesis, the always-valid [continuous semimartingale decomposition](../../../../../../continuous-semimartingale-decomposition.md) is $X=X_0+N+A^f$, with $N$ the zero-starting integral above. Alternatively one may use the convention that a local martingale permits an arbitrary finite initial value and localizes its centered increments. With deterministic initial data, as in part (c), there is no issue. This is [initial-value integrability in normalized semimartingale decompositions](../../../../../../initial-value-integrability-in-normalized-semimartingale-decompositions.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
