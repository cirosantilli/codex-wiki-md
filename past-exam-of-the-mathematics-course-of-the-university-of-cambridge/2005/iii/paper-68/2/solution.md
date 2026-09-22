<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Put $x=\cos\theta$. The trigonometric identity

$$
\cos((n+1)\theta)+\cos((n-1)\theta)=2\cos\theta\cos(n\theta)
$$

gives

$$
\boxed{T_{n+1}(x)=2xT_n(x)-T_{n-1}(x).}
$$

Starting with $T_0=1$ and $T_1=x$, this recurrence proves inductively that each [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) is a [polynomial](../../../../../polynomial-split.md). For $n\geq1$, the highest-degree term in $2xT_n$ cannot cancel against $T_{n-1}$, so the degree increases by one and its [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) doubles. Thus

$$
\boxed{\deg T_n=n,\qquad \operatorname{lc}(T_n)=2^{n-1}\quad(n\geq1).}
$$

The constant [polynomial](../../../../../polynomial-split.md) $T_0$ has [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) one.

For $n\geq1$, the points $x_j=\cos(j\pi/n)$, $j=0,\ldots,n$, give $T_n(x_j)=(-1)^j$. They are all the points where $|T_n|=1$, since $|\cos(n\theta)|=1$ exactly when $n\theta$ is an integer multiple of $\pi$. Therefore there are **$n+1$ equioscillation points**, including the two endpoints. Reversing their order makes an increasing alternating sequence. For $n=0$ the [polynomial](../../../../../polynomial-split.md) is constant: every point has unit value, but an alternating sequence has at most one point.

Now take $n\geq1$ and $c=2^{1-n}$. Since $cT_n$ is monic, $p_0(x)=x^n-cT_n(x)$ has degree at most $n-1$, and $\|x^n-p_0\|_\infty=c$. This proves the upper bound for the best error.

For the lower bound, suppose a [polynomial](../../../../../polynomial-split.md) $p$ of degree at most $n-1$ had $\|x^n-p\|_\infty<c$. At each of the $n+1$ ordered extrema, $h=p-p_0$ must have the same strictly nonzero sign as $T_n$: if $cT_n=c$, then $|c-h|<c$ gives $h>0$, and if $cT_n=-c$, then $|-c-h|<c$ gives $h<0$. Between every consecutive pair, the [intermediate value theorem](../../../../../intermediate-value-theorem.md) gives a zero of $h$. These are $n$ distinct zeros, impossible for a nonzero [polynomial](../../../../../polynomial-split.md) of degree at most $n-1$; $h=0$ is incompatible with the strict error improvement. This first-principles sign argument proves the [monic Chebyshev extremal polynomial](../../../../../monic-chebyshev-extremal-polynomial.md) bound without using the alternation theorem:

$$
\boxed{E_{n-1}(x^n)=2^{1-n}.}
$$

The displayed $p_0$ supplies an actual best approximating [polynomial](../../../../../polynomial-split.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
