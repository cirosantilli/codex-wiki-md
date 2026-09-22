<h1 id="39b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $k_0=\lceil(n+1)/2\rceil$, $\theta=\pi/(n+1)$, and define the high-frequency endpoint parameters

$$
a=1-\cos(k_0\theta),\qquad b=1+\cos\theta.
$$

They obey $1\leq a\leq b<2$ (with equality of endpoints for a single high mode). Since $|1-\omega t|$ is convex in $t$ and the endpoint modes are included, the exact high-frequency attenuation is

$$
\mu_\omega=\max\{|1-\omega a|,|1-\omega b|\}.
$$

The minimax choice balances the endpoint values with opposite signs. If they were not balanced, moving $\omega$ toward their balancing point would lower the larger endpoint value. Thus

$$
\boxed{\omega_*^{(n)}=\frac2{a+b},\qquad
\mu_*^{(n)}=\frac{b-a}{a+b}.}
$$

For odd $n$, $a=1$, giving $\omega_*=2/(2+\cos\theta)$ and $\mu_*=\cos\theta/(2+\cos\theta)$. For even $n$, $a=1+\sin(\theta/2)$, giving

$$
\omega_*^{(n)}=\frac2{2+\cos\theta+\sin(\theta/2)},\qquad
\mu_*^{(n)}=\frac{\cos\theta-\sin(\theta/2)}{2+\cos\theta+\sin(\theta/2)}.
$$

These give the [exact finite-grid high-frequency Jacobi smoothing optimum](../../../../../../exact-finite-grid-high-frequency-jacobi-smoothing-optimum.md), including complete annihilation when there is only one high-frequency mode. Their grid-independent limits are **$\boxed{\omega_*=2/3,\ \mu_*=1/3}$**. Choosing $2/3$ damps every high mode by at most $1/3$ on every grid, while its low-mode factor remains $1-O(n^{-2})$. Thus high frequencies decay geometrically much faster. The familiar $2/3,1/3$ pair is the optimal uniform-in-grid smoother; it need not be the exact optimum on a particular finite sine-mode grid.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [39B](../../39b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
