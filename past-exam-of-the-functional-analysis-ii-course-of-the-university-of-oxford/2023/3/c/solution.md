<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $u(t)=e^t$ and $v(t)=e^{-t}$. Both lie in the [Hilbert space](../../../../hilbert-space-split.md) $L^2(-\pi,\pi)$, and the [integral operator](../../../../integral-operator.md) factors as the [rank-one operator](../../../../rank-one-operator.md)

$$
Tf=\langle f,v\rangle u.
$$

The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) gives $\|Tf\|\leq\|u\|\|v\|\|f\|$, and equality is attained at $f=v/\|v\|$. Hence the [operator norm](../../../../operator-norm.md) is $\|T\|=\|u\|\|v\|$. Direct integration gives

$$
\|u\|^2=\int_{-\pi}^{\pi}e^{2t}\,dt
=\frac{e^{2\pi}-e^{-2\pi}}2=\sinh(2\pi),\qquad
\|v\|^2=\sinh(2\pi).
$$

For any [Hilbertian basis](../../../../hilbertian-basis.md) $(h_k)$, the [Parseval identity for a Hilbertian basis](../../../../parseval-identity-for-a-hilbertian-basis.md) gives

$$
\|T\|_2^2=\sum_k\|\langle h_k,v\rangle u\|^2
=\|u\|^2\sum_k|\langle h_k,v\rangle|^2
=\|u\|^2\|v\|^2.
$$

This is the general formula for the [norms of a rank-one operator](../../../../norms-of-a-rank-one-operator.md). In particular $T$ is a [Hilbert-Schmidt operator](../../../../hilbert-schmidt-operator.md), and

$$
\boxed{\|T\|=\|T\|_2=\sinh(2\pi)=\frac{e^{2\pi}-e^{-2\pi}}2.}
$$

This computation needs no explicit [Fourier basis](../../../../fourier-basis.md). The printed optional basis formula omits the variable $t$: the intended [Hilbertian basis](../../../../hilbertian-basis.md) is $e_n(t)=(2\pi)^{-1/2}e^{int}$, $n\in\mathbb Z$. Taken literally, the printed expressions are constant [functions](../../../../function-split.md) and cannot form an [orthonormal basis](../../../../orthonormal-basis.md) of $L^2(-\pi,\pi)$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the functional analysis II course of the University of Oxford](../../../split.md)
5. [Functional analysis II course of the University of Oxford](../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
