<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose the normalization constant real and positive; its otherwise arbitrary phase is physically immaterial. Orthogonality of the [Fock states](../../../fock-state.md) gives

$$
1=|k|^2\sum_{n=0}^{\infty}\frac{|\alpha|^{2n}}{n!}=|k|^2e^{|\alpha|^2},\qquad\boxed{k=e^{-|\alpha|^2/2}.}
$$

Acting with the [annihilation operator](../../../annihilation-operator.md) and shifting the summation index gives

$$
\hat a|\alpha\rangle=k\sum_{n\ge1}\frac{\alpha^n\sqrt n}{\sqrt{n!}}|n-1\rangle=\alpha k\sum_{m\ge0}\frac{\alpha^m}{\sqrt{m!}}|m\rangle=\boxed{\alpha|\alpha\rangle.}
$$

Thus a [coherent state](../../../coherent-state.md) is an annihilation-operator eigenket. It is not also an eigenket of the [creation operator](../../../creation-operator.md): a common eigenket would make $[\hat a,\hat a^\dagger]$ annihilate it, contradicting $[\hat a,\hat a^\dagger]=I$. Taking the adjoint of the annihilation-operator equation instead gives the distinct, valid bra relation

$$
\boxed{\langle\alpha|\hat a^\dagger=\alpha^*\langle\alpha|.}
$$

With $\hat n=\hat a^\dagger\hat a$, the [photon number](../../../photon-number.md) [expected value](../../../expected-value-split.md) is $\mu=|\alpha|^2$. Normal ordering $\hat n^2=(\hat a^\dagger)^2\hat a^2+\hat a^\dagger\hat a$ gives $\langle n^2\rangle=\mu^2+\mu$. Therefore

$$
\boxed{\langle n\rangle=\mu,\qquad\Delta n=\sqrt\mu=|\alpha|,\qquad\frac{\Delta n}{\langle n\rangle}=\frac1{\sqrt\mu}\quad(\mu>0).}
$$

At large mean photon number the relative fluctuations vanish, giving a classical-field limit even though quantum fluctuations remain. For the vacuum $\mu=0$, the relative ratio itself is undefined.

The [Born rule](../../../born-rule.md) applied to the number-state coefficient gives the [Poisson distribution](../../../poisson-distribution.md)

$$
\boxed{\Pr(n)=e^{-\mu}\frac{\mu^n}{n!},\qquad n=0,1,2,\ldots.}
$$

It depends on the single parameter $\mu=\langle n\rangle$, and has equal [expected value](../../../expected-value-split.md) and [variance](../../../variance-split.md), consistent with the preceding moments.

For a [Fock state](../../../fock-state.md) $|n\rangle$, raising or lowering the number makes an orthogonal state, so the [optical quadrature](../../../optical-quadrature.md) has $\langle\hat X\rangle=0$. Expanding its square gives

$$
\hat X^2=\frac12[\hat a^2+(\hat a^\dagger)^2+\hat a\hat a^\dagger+\hat a^\dagger\hat a],\qquad\boxed{\langle n|\hat X^2|n\rangle=n+\frac12.}
$$

The first two terms have zero diagonal matrix elements, while the last two contribute $n+1$ and $n$. In particular, the vacuum retains quadrature [variance](../../../variance-split.md) $1/2$.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [2016](../../2016-split.md)
3. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../split.md)
4. [Laser science and quantum information processing course of the University of Oxford](../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
