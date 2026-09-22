<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For odd $p$, write $e_p(t)=e^{2\pi it/p}$ and use the [discrete paraboloid](../../../../../discrete-paraboloid.md)

$$
P=\{(u,v,u^2+v^2):u,v\in\mathbb F_p\},\qquad \sigma=p^{-2}1_P.
$$

Here surface integration means $p^{-2}\sum_P$, whereas ambient [norms](../../../../../norm.md) below use unnormalized counting measure on $\mathbb F_p^3$. With the negative-phase transform convention,

$$
\widehat\sigma(x)=p^{-2}\sum_{u,v}e_p(-x_1u-x_2v-x_3(u^2+v^2)).
$$

When $x_3=0$, additive-[orthogonality of characters](../../../../../character-orthogonality.md) makes this one at $x=0$ and zero at all other points of that plane. When $x_3\ne0$, completing the two squares gives

$$
\widehat\sigma(x)=p^{-2}e_p\left(\frac{x_1^2+x_2^2}{4x_3}\right)G(-x_3)^2,\qquad G(t)=\sum_u e_p(tu^2).
$$

The [Quadratic Gauss sum](../../../../../quadratic-gauss-sum.md) identity is $G(t)^2=\chi(-1)p$, where $\chi$ is the [Legendre symbol](../../../../../legendre-symbol.md). For completeness, counting the preimages of a square gives $G(t)=\chi(t)G(1)$ for nonzero $t$. Also $|G(1)|^2=\sum_{u,v}e_p(u^2-v^2)=p$, by the invertible change $(u,v)\mapsto(u-v,u+v)$ and [orthogonality of characters](../../../../../character-orthogonality.md). Since $\overline{G(1)}=G(-1)=\chi(-1)G(1)$, the asserted square identity follows. Thus for $p\equiv3\pmod4$,

$$
\boxed{\widehat\sigma(x)=\begin{cases}1,&x=0,\\0,&x_3=0,\ x\ne0,\\-p^{-1}e_p((x_1^2+x_2^2)/(4x_3)),&x_3\ne0.\end{cases}}
$$

Using positive phase instead changes the sign inside the character, not the magnitude or any [norm](../../../../../norm.md) estimate.

Define $Eg(x)=p^{-2}\sum_{\xi\in P}g(\xi)e_p(x\cdot\xi)$, and define $R^*(2\to q)$ as the smallest constant for

$$
\|Eg\|_{\ell^q(\mathbb F_p^3)}\leq R^*(2\to q)\left(p^{-2}\sum_{\xi\in P}|g(\xi)|^2\right)^{1/2}.
$$

The adjoint relative to these measures is $E^*h(\xi)=\sum_xh(x)e_p(-x\cdot\xi)$. Consequently $EE^*h=h*\widehat\sigma(-\cdot)$, where convolution is the unnormalized ambient sum. Put $K=\widehat\sigma(-\cdot)-1_{\{0\}}$. Its supremum is at most $p^{-1}$, so convolution by $K$ has $\ell^1\to\ell^\infty$ [norm](../../../../../norm.md) at most $p^{-1}$.

Under the unnormalized ambient [Fourier transform on a finite group](../../../../../fourier-transform-on-a-finite-group.md), the convolution multiplier of $\widehat\sigma(-\cdot)$ is $p^3\sigma=p1_P$, up to the harmless reflection convention. Thus the multiplier of $K$ is $p1_P-1$, with maximum absolute value at most $p$. The [Plancherel theorem](../../../../../plancherel-theorem.md) gives $\ell^2\to\ell^2$ [norm](../../../../../norm.md) at most $p$. The [Riesz-Thorin interpolation theorem](../../../../../riesz-thorin-theorem.md) between these two bounds gives $\ell^{4/3}\to\ell^4$ [norm](../../../../../norm.md) at most one for convolution by $K$. Convolution by $1_{\{0\}}$ is the identity, whose $\ell^{4/3}\to\ell^4$ [norm](../../../../../norm.md) is at most one for counting measure. Hence $\|EE^*h\|_4\leq2\|h\|_{4/3}$.

By [Lp duality](../../../../../lp-duality-on-an-arbitrary-measure-space.md) and [Hölder's inequality](../../../../../holder-s-inequality.md), $\|E^*h\|_{L^2(\sigma)}^2=\langle EE^*h,h\rangle\leq2\|h\|_{4/3}^2$. Taking adjoints proves the [finite-field paraboloid fourth-moment extension estimate](../../../../../finite-field-paraboloid-fourth-moment-extension-estimate.md)

$$
\boxed{R^*(2\to4)\leq\sqrt2<10.}
$$

In fact this argument works for both residue classes of odd primes.

If $p\equiv1\pmod4$, choose $i\in\mathbb F_p$ with $i^2=-1$. The complete line $\ell=\{(t,it,0):t\in\mathbb F_p\}$ lies in $P$. For $g=1_\ell$ the normalized surface $L^2$ [norm](../../../../../norm.md) is $p^{-1/2}$, and [orthogonality of characters](../../../../../character-orthogonality.md) gives $Eg(x)=p^{-1}1_{\{x_1+ix_2=0\}}$. That annihilator plane has $p^2$ points, so the [isotropic-line obstruction to finite-field restriction](../../../../../isotropic-line-obstruction-to-finite-field-restriction.md) gives

$$
\boxed{R^*(2\to q)\geq\frac{p^{2/q-1}}{p^{-1/2}}=p^{2/q-1/2}.}
$$

This tends to infinity along these primes for every $q<4$, as required.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
