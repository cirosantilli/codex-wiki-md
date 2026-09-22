<h1 id="2i/solution">Solution</h1>

↑ **Parent:** [2I](../2i.md)

Chebyshev's equal-ripple criterion says that a [polynomial](../../../../../polynomial-split.md) $q$ of degree at most $m$ is a best uniform approximation to a [continuous function](../../../../../continuous-function.md) $F$ if and only if the error $F-q$ attains alternating extrema of maximum magnitude at $m+2$ ordered points.

Since $T_n$ has leading coefficient $2^{n-1}$, the [polynomial](../../../../../polynomial-split.md) $2^{1-n}T_n$ is monic and alternates between $\pm2^{1-n}$ at $t_j=\cos(j\pi/n)$. Therefore

$$
\boxed{q_*(t)=t^n-2^{1-n}T_n(t),\qquad
\min_{\deg q<n}\lVert t^n-q\rVert_\infty=2^{1-n}.}
$$

At each $t_j$, both $T_n-f$ and $T_n+f$ have sign $(-1)^j$, because $|f(t_j)|<1$. Each has a root in every interval between consecutive extrema, hence all its at most $n$ roots lie in $(-1,1)$. For $t>1$ both [polynomials](../../../../../polynomial-split.md) remain positive, giving $|f(t)|<T_n(t)$. For $t<-1$ both have sign $(-1)^n$, giving $|f(t)|<|T_n(t)|$. On $[-1,1]$ the hypothesis gives $|f|<1$. Thus

$$
\boxed{|f(t)|<\max\{1,|T_n(t)|\}\quad(t\in\mathbb R).}
$$

## ↑ Ancestors (10)

1. [2I](../2i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
