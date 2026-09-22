<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [completed Dirichlet L-function](../../../../../../completed-dirichlet-l-function.md) is

$$
\Lambda(s,\chi)=\left(\frac q\pi\right)^{(s+a)/2}\Gamma\left(\frac{s+a}{2}\right)L(s,\chi).
$$

For nonprincipal [primitive Dirichlet characters](../../../../../../primitive-dirichlet-character.md), termwise [Mellin transformation](../../../../../../mellin-transform.md) initially in $\Re s>1$ gives

$$
\Lambda(s,\chi)=\frac12\int_0^\infty\theta_\chi(x)x^{(s+a)/2}\,\frac{dx}{x}.
$$

The [Dirichlet character theta function](../../../../../../dirichlet-character-theta-function.md) decays exponentially at infinity; its transformation makes it decay faster than any power at zero. Hence the integral is entire in $s$. For even parity, substitute $x=1/y$ and the theta transformation to obtain

$$
\boxed{\Lambda(s,\chi)=\varepsilon_\chi\Lambda(1-s,\overline\chi).}
$$

The same calculation with the extra $x^{-1}$ power gives the odd [functional equation](../../../../../../functional-equation.md) with its corresponding root number.

The [gamma function](../../../../../../gamma-function.md) has no zeros and has [simple poles](../../../../../../simple-pole.md) at nonpositive [integers](../../../../../../integer.md). Thus the nontrivial zeros of $L$ and $\Lambda$ coincide with multiplicities. The [trivial zeros of a Dirichlet L-function](../../../../../../trivial-zero-of-a-dirichlet-l-function.md) are $0,-2,-4,\ldots$ for a nonprincipal even character, and $-1,-3,-5,\ldots$ for an odd character. They cancel the gamma [poles](../../../../../../pole.md) and are not zeros of $\Lambda$: the [functional equation](../../../../../../functional-equation.md) takes these points to the zero-free right-hand region, including the standard [nonvanishing of nonprincipal Dirichlet L-functions at one](../../../../../../nonvanishing-of-a-nonprincipal-dirichlet-l-function-at-one.md) at the even endpoint. The canceled zeros are simple.

The principal [primitive Dirichlet character](../../../../../../primitive-dirichlet-character.md) has [conductor of a Dirichlet character](../../../../../../conductor-of-a-dirichlet-character.md) equal to one and $L=\zeta$. In that case $\Lambda=\pi^{-s/2}\Gamma(s/2)\zeta(s)$ is [meromorphic](../../../../../../meromorphic-function.md) with [poles](../../../../../../pole.md) at zero and one. Its canceled trivial zeros begin at $-2$, while $\zeta(0)=-1/2$ is not zero. Multiplication by $s(s-1)/2$ produces the entire [Riemann xi function](../../../../../../riemann-xi-function.md) used below.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
