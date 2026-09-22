<h1 id="21g/solution">Solution</h1>

↑ **Parent:** [21G](../21g.md)

The [spectrum of a bounded operator](../../../../../spectrum-of-a-bounded-operator.md) is $\sigma(T)=\{\lambda\in\mathbb C:T-\lambda I\text{ has no bounded everywhere-defined inverse}\}$. Initially define $T$ on finite linear combinations of the [orthonormal basis](../../../../../orthonormal-basis.md). The [bilateral shift operator](../../../../../bilateral-shift-operator.md) $Se_n=e_{n+1}$ preserves the [Hilbert space](../../../../../hilbert-space-split.md) norm and extends to a unitary operator on $H$; its inverse is $S^*e_n=e_{n-1}$. Thus $T=S+S^*$ extends uniquely by density, is bounded with norm at most two, and is [self-adjoint](../../../../../self-adjoint-operator.md).

For $v_N=(2N+1)^{-1/2}\sum_{n=-N}^Ne_n$, $\|v_N\|=1$ and the only nonzero coefficients of $(T-2I)v_N$ occur at $-N-1,-N,N,N+1$. Hence

$$
\|(T-2I)v_N\|^2=\frac4{2N+1}\longrightarrow0.
$$

It follows that $\|Tv_N\|\to2$, proving $\boxed{\|T\|=2}$. Also $\boxed{2\in\sigma(T)}$: a bounded inverse of $T-2I$ would give $1\leq\|(T-2I)^{-1}\|\,\|(T-2I)v_N\|\to0$. Thus two belongs to the [approximate point spectrum](../../../../../approximate-point-spectrum.md).

An [eigenvector](../../../../../eigenvector.md) $x=\sum x_ne_n$ would satisfy $\lambda x_n=x_{n-1}+x_{n+1}$. Self-adjointness and the norm bound force $\lambda\in[-2,2]$. If $|\lambda|<2$, write $\lambda=2\cos\theta$ with $0<\theta<\pi$; the general complex solution of the [linear recurrence relation](../../../../../linear-recurrence-relation.md) is

$$
x_n=Ae^{in\theta}+Be^{-in\theta}.
$$

The Cesàro mean of $|x_n|^2$ over $n=-N,\ldots,N$ tends to $|A|^2+|B|^2$, since the mixed geometric sum divided by $2N+1$ tends to zero. For an $\ell^2$ sequence the same mean tends to zero. Therefore $A=B=0$. At $\lambda=\pm2$, the general solution is $(A+Bn)(\pm1)^n$, again square summable only when zero. This also covers $\lambda=0$ through $\theta=\pi/2$. Thus $\boxed{T\text{ has no eigenvectors}}$.

Finally the bounded sequence $e_{3j}$ has images $Te_{3j}=e_{3j-1}+e_{3j+1}$ with pairwise disjoint supports. Distinct images have distance two, so no subsequence converges. Hence $\boxed{T\text{ is not compact}}$.

## ↑ Ancestors (10)

1. [21G](../21g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
