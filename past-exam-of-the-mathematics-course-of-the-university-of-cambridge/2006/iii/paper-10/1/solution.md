<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [normal family](../../../../../normal-family.md) is a family such that every sequence has a subsequence converging locally uniformly in the spherical metric to a meromorphic limit, possibly the constant infinity. For a family uniformly bounded in modulus, the possible limits are finite [holomorphic functions](../../../../../holomorphic-function.md), and ordinary locally uniform convergence suffices. The limit need not take values in the open [unit disc](../../../../../unit-disc.md); a sequence of constants can approach its boundary.

Here is a direct compactness proof for disc-valued maps. For each [compact subset](../../../../../compact-space.md) $K\subset\Omega$, choose a slightly larger compact neighborhood contained in $\Omega$. The [Cauchy estimate](../../../../../cauchy-estimate.md) on a fixed-radius disk around each point bounds $|f'|$ independently of $f$ because $|f|<1$. A finite covering of $K$ yields uniform boundedness and equicontinuity there. The [Arzelà-Ascoli theorem](../../../../../arzela-ascoli-theorem.md), applied successively to a [compact exhaustion](../../../../../compact-exhaustion.md) and followed by a diagonal subsequence, gives a limit uniformly on every compact. The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) passes to that limit on small circles, proving it is a [holomorphic function](../../../../../holomorphic-function.md). This proves the required [normal family](../../../../../normal-family.md) assertion rather than just invoking [Montel theorem](../../../../../montel-s-theorem.md).

Every $g_n(z)=g(z/n)$ is a [holomorphic function](../../../../../holomorphic-function.md) on the [complex upper half-plane](../../../../../upper-half-plane-complex-analysis.md) with values in the [unit disc](../../../../../unit-disc.md), so the same argument makes $(g_n)$ a [normal family](../../../../../normal-family.md). If a subsequence converges locally uniformly to $h$, then for every $t>0$,

$$
h(it)=\lim_j g(it/n_j)=\ell.
$$

The [identity theorem for holomorphic functions](../../../../../identity-theorem.md) gives $h\equiv\ell$. Since every convergent subsequence has this same limit, the whole sequence converges locally uniformly to $\ell$: otherwise a compact set and a subsequence with a fixed positive discrepancy would have a further locally uniformly convergent subsequence, a contradiction.

To obtain the [nontangential limit](../../../../../nontangential-limit.md), take any $z_j=x_j+iy_j\to0$ with $|x_j|\leq A y_j$ and $y_j>0$. Put $n_j=\lfloor1/y_j\rfloor$. Then $n_j\to\infty$, $n_jy_j\to1$, and the points $\zeta_j=n_jz_j$ lie, for large $j$, in a fixed compact rectangle inside the half-plane. Therefore

$$
\boxed{g(z_j)=g_{n_j}(\zeta_j)\longrightarrow\ell.}
$$

This is the [normal-family proof of angular boundary convergence](../../../../../normal-family-proof-of-angular-boundary-convergence.md); using integer rescalings requires this step because the points need not lie exactly on one fixed scaled ray.

For a tangential counterexample, use

$$
\boxed{g(z)=e^{-i/z}.}
$$

If $z=x+iy$ with $y>0$, then $\operatorname{Re}(-i/z)=-y/(x^2+y^2)<0$, so $g$ is a [holomorphic function](../../../../../holomorphic-function.md) and $|g|<1$. Also $g(iy)=e^{-1/y}\to0$. But

$$
z_n=\frac1{2\pi n-i/n}\in\mathbb H,\qquad z_n\to0,\qquad g(z_n)=e^{-1/n}\to1.
$$

Their ratio $|\operatorname{Re}z_n|/\operatorname{Im}z_n=2\pi n^2$ tends to infinity. Thus the [nontangential limit](../../../../../nontangential-limit.md) is zero while the unrestricted boundary limit does not exist.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
