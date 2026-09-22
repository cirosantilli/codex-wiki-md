<h1 id="12g/solution">Solution</h1>

↑ **Parent:** [12G](../12g.md)

An [analytic branch of a square root](../../../../../analytic-branch-of-a-square-root.md) determined by the branch $\ell$ is

$$
\boxed{\psi(z)=\exp\!\left(\frac12\ell(z)\right)}.
$$

If $\psi_1$ and $\psi_2$ are two such branches, their ratio $h=\psi_1/\psi_2$ is analytic and satisfies $h^2=1$. Since a domain is connected and $h$ takes values in the discrete set $\{1,-1\}$, $h$ is constant. Thus $\psi_1=\psi_2$ throughout $D$ or $\psi_1=-\psi_2$ throughout $D$.

For $z=re^{i\theta}$, the [principal square root](../../../../../principal-square-root-of-a-complex-number.md) is

$$
\sigma_1(z)=\sqrt r\,e^{i\theta/2},
\qquad -\pi<\theta<\pi.
$$

On $D_2$, one may instead take

$$
\sigma_2(z)=\sqrt r\,e^{i\theta/2},
\qquad 0<\theta<2\pi.
$$

The respective removed half-axes are their [branch cuts](../../../../../branch-cut.md).

On $\mathbb C\setminus[-1,1]$, define

$$
\boxed{\varphi(z)=-iz\,\sigma_1\!\left(1-\frac1{z^2}\right)}.
$$

It is analytic there, its square is $1-z^2$, and

$$
\varphi(2i)=-i(2i)\sqrt{1+\frac14}=\sqrt5,
$$

so it is the required branch. Substitution gives, for $0<|z|<1$,

$$
\varphi(1/z)=-\frac{i}{z}\sigma_1(1-z^2).
$$

The [binomial series](../../../../../binomial-series.md) yields

$$
\sigma_1(1-z^2)=1-\frac12z^2-\frac18z^4+O(z^6),
$$

hence the first three terms of the [Laurent series](../../../../../laurent-series.md) are

$$
\boxed{\varphi(1/z)=-\frac{i}{z}+\frac{i}{2}z+\frac{i}{8}z^3+O(z^5)}.
$$

Since

$$
g(z)=\frac{\varphi(1/z)}{1+z^2},
$$

its [residue](../../../../../residue.md) at zero is $-i$. Under the change of variable $z=1/\zeta$, the two orientation reversals cancel, and the [residue theorem](../../../../../residue-theorem.md) gives

$$
\boxed{\int_{|z|=2}f(z)\,dz
=\int_{|\zeta|=1/2}g(\zeta)\,d\zeta
=2\pi i(-i)=2\pi}.
$$

## ↑ Ancestors (10)

1. [12G](../12g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
