<h1 id="m/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

[Independence](../../../../independent-random-variables.md) means $\Pr(X\in A,Y\in B)=\Pr(X\in A)\Pr(Y\in B)$ for all [Borel sets](../../../../borel-set.md) $A,B$. For variables with a [joint density](../../../../joint-probability-density.md) this is equivalent to factorization of that density into the two marginal densities [almost everywhere](../../../../almost-everywhere.md).

The inverse transformation is $x=uv$, $y=(1-u)v$, on $0<u<1$, $v>0$. Its absolute [Jacobian determinant](../../../../jacobian-determinant.md) is $v$. Multiplying the independent gamma densities by it gives

$$
f_{U,V}(u,v)=\frac{\lambda^{\alpha+\beta}}{\Gamma(\alpha)\Gamma(\beta)}
u^{\alpha-1}(1-u)^{\beta-1}v^{\alpha+\beta-1}e^{-\lambda v}.
$$

The density is zero outside that [support](../../../../support.md). Integrating in $v$ with the [gamma integral](../../../../gamma-integral.md) gives

$$
\boxed{f_U(u)=\frac{\Gamma(\alpha+\beta)}{\Gamma(\alpha)\Gamma(\beta)}
u^{\alpha-1}(1-u)^{\beta-1},\quad0<u<1.}
$$

It is a beta density. Its normalization also proves the [beta integral](../../../../beta-integral.md) $\int_0^1u^{\alpha-1}(1-u)^{\beta-1}du=\Gamma(\alpha)\Gamma(\beta)/\Gamma(\alpha+\beta)$. The [joint density](../../../../joint-probability-density.md) consequently factors as this normalized beta density times

$$
\boxed{f_V(v)=\frac{\lambda^{\alpha+\beta}}{\Gamma(\alpha+\beta)}v^{\alpha+\beta-1}e^{-\lambda v},\quad v>0.}
$$

Thus $V$ is gamma with shape $\alpha+\beta$ and rate $\lambda$, and $U,V$ are independent.

Finally $X=UV$. All relevant first moments are finite, and [independence](../../../../independent-random-variables.md) gives $\mathbb E X=\mathbb E U\,\mathbb E V$, while $\mathbb E V=\mathbb E X+\mathbb E Y>0$. Hence

$$
\boxed{\mathbb E\frac X{X+Y}=\frac{\mathbb E X}{\mathbb E X+\mathbb E Y}=\frac\alpha{\alpha+\beta}.}
$$

This identity follows from the particular [beta-gamma independence](../../../../beta-gamma-independence.md) here; a general ratio of [random variables](../../../../random-variable-split.md) would not permit moving [expectation](../../../../expected-value-split.md) through division.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [M](../../m.md)
3. [2005](../../../2005-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
