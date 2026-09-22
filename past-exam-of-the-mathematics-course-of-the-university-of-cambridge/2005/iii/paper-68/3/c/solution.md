<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

As printed in the original PDF, this claim is false for $n\geq2$. The displayed frequency is one, so the function already belongs to the space of [trigonometric polynomials](../../../../../../trigonometric-polynomial.md) of degree at most $n-1$. Its best approximation is then the function itself, with zero error; for example, $\alpha=1,\beta=0$ gives a zero-approximant error $\int_0^{2\pi}|\cos x|\,dx=4$ instead. For $n=1$, zero is indeed the best constant approximation. Thus the literal answer is

$$
\boxed{p_*=f\quad(n\geq2),\qquad p_*=0\quad(n=1).}
$$

The natural intended version has frequency $n$. Set $g(y)=\alpha\cos y+\beta\sin y$ and $f_n(x)=g(nx)$. The sign function $h(y)=\operatorname{sign}g(y)$ is integrable and satisfies $h(y+\pi)=-h(y)$, so its [mean](../../../../../../expected-value.md) is zero. Part (b) makes $h(nx)=\operatorname{sign}f_n(x)$ orthogonal to every degree-at-most-$n-1$ [trigonometric polynomial](../../../../../../trigonometric-polynomial.md). Part (a), with $p_*=0$, now proves

$$
\boxed{\text{The best approximation to }\alpha\cos(nx)+\beta\sin(nx)
\text{ from }\mathcal T_{n-1}\text{ in }L^1\text{ is }0.}
$$

The error is $4\sqrt{\alpha^2+\beta^2}$ for the unnormalized integral over a period.

The best approximant is unique. If the amplitude is nonzero and another continuous [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) $p$ has the same optimal error, equality in part (a)'s pointwise inequality holds almost everywhere. Near each zero of $f_n$, the function changes sign; if $p$ did not vanish at that zero, continuity would force an interval on one side where $f_n-p$ has the wrong sign, making the integral inequality strict. Thus $p$ vanishes at all $2n$ distinct zeros of $f_n$. A nonzero [trigonometric polynomial](../../../../../../trigonometric-polynomial.md) of degree at most $n-1$ has at most $2n-2$ zeros in one period, since multiplication by $e^{i(n-1)x}$ turns it into a [polynomial](../../../../../../polynomial-split.md) in $e^{ix}$ of degree at most $2n-2$. Hence $p=0$. Zero amplitude is immediate. The same reasoning proves the literal frequency-one assertion when $n=1$, while retaining the counterexample for larger $n$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
