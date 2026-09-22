<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\delta\notin2\pi\mathbb Z$, the finite [geometric series](../../../../geometric-series.md) gives

$$
\sum_{n=1}^N e^{in\delta}
=\frac{e^{i\delta}(1-e^{iN\delta})}{1-e^{i\delta}}
=e^{i(N+1)\delta/2}\frac{\sin(N\delta/2)}{\sin(\delta/2)}.
$$

The exponential prefactor has [modulus](../../../../modulus.md) one. Thus

$$
\boxed{\left|\sum_{n=1}^N e^{in\delta}\right|
=\begin{cases}|\sin(N\delta/2)/\sin(\delta/2)|,&\delta\notin2\pi\mathbb Z,\\N,&\delta\in2\pi\mathbb Z.\end{cases}}
$$

At an excluded phase every summand is one, which supplies the removable limiting value directly. Here $N$ is a positive [integer](../../../../integer-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
