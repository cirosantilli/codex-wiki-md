<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**The printed proximity integral is missing a factor $1/(2\pi)$.** Denote that literal integral by $m_{\mathrm{print}}$ and write $\overline m=m_{\mathrm{print}}/(2\pi)$. The correct [Annular spherical Jensen formula](../../../../../annular-spherical-jensen-formula.md), with the printed definitions of $N$ and $T$, is

$$
\boxed{T(r)=I(a)\log(1/r)+N(r;a)+\overline m(r;a).}
$$

The following derivation proves this identity and also isolates the normalization issue.

For the [chordal metric](../../../../../chordal-metric.md) put $u_a(z)=-\log k(f(z),a)$ and let $M_a(s)=(2\pi)^{-1}\int_0^{2\pi}u_a(se^{i\theta})\,d\theta$. In a finite target coordinate,

$$
u_a=\tfrac12\log(1+|f|^2)-\log|f-a|+\tfrac12\log(1+|a|^2).
$$

For $a=\infty$ use $u_\infty=\tfrac12\log(1+|f|^2)$. Differentiating away from the preimages of $a$ gives half the squared [spherical derivative of a meromorphic function](../../../../../spherical-derivative-of-a-meromorphic-function.md). At an $a$-point of local degree $d$, $u_a=-d\log|z-z_0|+O(1)$; the second [distributional derivatives](../../../../../distributional-derivative.md) give the Laplacian of $\log|z-z_0|$ is $2\pi\delta_{z_0}$. Thus, including [poles](../../../../../pole.md) by changing spherical coordinates,

$$
\Delta u_a=\frac12\left(\frac{2|f'|}{1+|f|^2}\right)^2-2\pi\sum_{f(z)=a}\deg_z(f)\,\delta_z.
$$

Because $a$ is off the image of $|z|=1$, $u_a$ is smooth near that circle and $I(a)=M_a'(1)$ is finite and independent of $r$.

Apply [Green's second identity](../../../../../green-second-identity.md) to the harmonic weight $w(z)=\log(|z|/r)$ on $r<|z|<1$. On the outer boundary $w=\log(1/r)$ and $\partial_nw=1$; on the inner boundary $w=0$ and $\partial_nw=-1/r$. Hence

$$
\int_{r<|z|<1}w\Delta u_a\,dA=2\pi\left[M_a'(1)\log(1/r)+M_a(r)-M_a(1)\right].
$$

The distributional formula makes the left side $2\pi T(r)-2\pi N(r;a)$, and $M_a(r)-M_a(1)=\overline m(r;a)$, proving the corrected [Annular spherical Jensen formula](../../../../../annular-spherical-jensen-formula.md). Initially take an inner circle avoiding $a$-points. Logarithmic singularities have continuous angular means, and a point on the inner circle has zero logarithmic counting weight, so continuity extends the identity to every $0<r\le1$.

There is no way to absorb the missing factor into a different constant $I(a)$. For the [holomorphic function](../../../../../holomorphic-function.md) $f(z)=z$ and $a=\infty$, direct integration gives

$$
N(r;\infty)=0,\qquad m_{\mathrm{print}}(r;\infty)=\pi\log\frac{1+r^2}{2},\qquad T(r)=\frac12\log\frac1r+\frac12\log\frac{1+r^2}{2}.
$$

The value of $(T-m_{\mathrm{print}})/\log(1/r)$ tends to $1/2$ as $r\downarrow0$ and to $\pi$ as $r\uparrow1$. Therefore **the literal printed identity has no constant $I(\infty)$**, whereas the corrected identity has $I(\infty)=1/2$.

For the singularity criterion, define the nondecreasing normalized spherical area

$$
s(t)=\frac1{4\pi}\int_{e^{-t}<|z|<1}\left(\frac{2|f'|}{1+|f|^2}\right)^2dA,\qquad t\ge0.
$$

[Tonelli's theorem](../../../../../tonelli-theorem.md) applied to the logarithmic weight gives $T(e^{-l})=\int_0^l s(t)\,dt$. Averages of a nondecreasing function converge to its supremum: for fixed $t_0<l$, $(1-t_0/l)s(t_0)\le T(e^{-l})/l\le s(l)$. Thus the limit, not just the lower limit, exists in $[0,\infty]$ and equals

$$
\boxed{\lim_{r\downarrow0}\frac{T(r)}{\log(1/r)}=\frac1{4\pi}\int_{0<|z|<1}\left(\frac{2|f'|}{1+|f|^2}\right)^2dA.}
$$

If $f$ has a [removable singularity](../../../../../removable-singularity.md) or [pole](../../../../../pole.md) at zero, it extends as a [holomorphic map](../../../../../holomorphic-map.md) to the [Riemann sphere](../../../../../riemann-sphere.md); the pulled-back spherical density is smooth and bounded on the closed disk, hence its area is finite. Conversely an [essential singularity](../../../../../essential-singularity.md) gives, by the meromorphic version of the [Great Picard theorem](../../../../../great-picard-theorem.md), infinitely many preimages of every spherical target with at most two exceptions in each punctured neighborhood. The [area formula](../../../../../area-formula-geometric-measure-theory.md) gives

$$
\int_{0<|z|<1}(f^{\#}_{\mathrm{round}})^2dA=\int_{\mathbb S^2}n_f(a)\,dA_{\mathbb S^2}(a)=\infty.
$$

The formula follows by applying [change of variables](../../../../../change-of-variables-formula.md) on inverse-function neighborhoods away from the discrete critical points, then summing with [multiplicity](../../../../../multiplicity-mathematics.md); the countable critical values have area zero. This proves the [finite spherical area criterion for an isolated singularity](../../../../../finite-spherical-area-criterion-for-an-isolated-singularity.md) and the requested **equivalence between a finite lower limit and a removable singularity or pole**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
