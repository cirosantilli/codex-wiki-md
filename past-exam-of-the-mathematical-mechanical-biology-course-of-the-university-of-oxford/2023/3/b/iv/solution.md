<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For the [neo-Hookean solid](../../../../../neo-hookean-solid.md), the axial [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) under the unloaded lateral [boundary conditions](../../../../../boundary-condition.md) is

$$
t_3=\mu(\alpha^2-\alpha^{-1}).
$$

With $K,\mu>0$, the spring balance is equivalent, after multiplication by $\alpha>0$, to the [cubic equation](../../../../../cubic-equation.md)

$$
\boxed{(K\gamma+\mu)\alpha^3-K\alpha^2-\mu=0.}
$$

For a fixed $\gamma\ge1$, write its left side as $h(\alpha)$. It obeys $h(0)=-\mu<0$ and tends to $+\infty$ as $\alpha\to\infty$. Moreover

$$
h'(\alpha)=\alpha\big[3(K\gamma+\mu)\alpha-2K\big].
$$

Thus $h$ first decreases from a negative value and then increases strictly, crossing zero exactly once on $\alpha>0$. For $\gamma>1$,

$$
h(1)=K(\gamma-1)>0,\qquad
h(1/\gamma)=\mu(\gamma^{-3}-1)<0,
$$

so the unique equilibrium has $1/\gamma<\alpha<1$. The tissue is elastically compressed, while its actual length $\alpha\gamma$ exceeds one and compresses the spring.

To determine the large-growth limit without presuming a power law, solve for $\gamma$:

$$
\gamma=\frac1\alpha+\frac\mu K(\alpha^{-3}-1).
$$

This is a strictly decreasing function of $\alpha>0$, since its [derivative](../../../../../derivative.md) is

$$
-\alpha^{-2}-\frac{3\mu}{K}\alpha^{-4}<0.
$$

It tends to $+\infty$ only as $\alpha\to0^+$. Consequently unlimited growth forces $\alpha\to0^+$, and

$$
\boxed{t_3=\mu(\alpha^2-\alpha^{-1})\to-\infty.}
$$

More precisely, the [dominant balance](../../../../../dominant-balance.md) is $K\gamma\alpha^3\sim\mu$, giving

$$
\boxed{\alpha\sim\left(\frac\mu{K\gamma}\right)^{1/3},\qquad
t_3\sim-\mu^{2/3}(K\gamma)^{1/3}.}
$$

The surrounding spring softens the divergence relative to rigid confinement but does not bound the compressive [stress](../../../../../stress.md). Both axial extension and lateral expansion help accommodate growth:

$$
\ell=\alpha\gamma\sim\left(\frac\mu K\right)^{1/3}\gamma^{2/3},\qquad
\mathcal A=\alpha^{-1}\sim\left(\frac K\mu\right)^{1/3}\gamma^{1/3},
$$

whose product is the total volume $\gamma$, as required by [elastic incompressibility](../../../../../elastic-incompressibility.md) and the imposed [growth tensor](../../../../../growth-tensor.md).

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the mathematical mechanical biology course of the University of Oxford](../../../../split.md)
6. [Mathematical mechanical biology course of the University of Oxford](../../../../../mathematical-mechanical-biology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
