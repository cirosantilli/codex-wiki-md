<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

After [modified minimal subtraction](../../../../../../modified-minimal-subtraction-scheme.md), the surviving logarithm in the given [fermion self-energy](../../../../../../fermion-self-energy.md) is $\log[\mu^2/((1-x)(m^2-p^2x))]$. For a one-loop mass shift, set $p^2=m^2$ and let $\not p$ act as $m$ on an on-shell spinor inside that correction; changing these arguments by the mass shift contributes only at order $e^4$. Thus

$$
\Sigma_R\big|_{\not p=m}
=\frac{e^2m}{8\pi^2}\int_0^1(x-2)\left[\log\frac{\mu^2}{m^2}-2\log(1-x)\right]dx.
$$

The needed integrals are

$$
\int_0^1(x-2)dx=-\frac32,\qquad
\int_0^1(x-2)\log(1-x)dx=\frac54.
$$

For the second, put $u=1-x$ and use $\int_0^1\log u\,du=-1$ and $\int_0^1u\log u\,du=-1/4$. Consequently

$$
\Sigma_R\big|_{\not p=m}=-\frac{e^2m}{16\pi^2}\left(5+3\log\frac{\mu^2}{m^2}\right).
$$

The [pole mass](../../../../../../pole-mass.md) condition $m_{\rm phys}-m+\Sigma_R=0$ gives $m_{\rm phys}=m[1+e^2(5+3\log(\mu^2/m^2))/(16\pi^2)]+O(e^4)$. Invert this relation and replace $m$ by $m_{\rm phys}$ inside the already one-loop term to obtain

$$
\boxed{m=m_{\rm phys}\left[1-\frac{e^2}{16\pi^2}\left(5+3\log\frac{\mu^2}{m_{\rm phys}^2}\right)\right]+O(e^4).}
$$

**The negative sign in the running-mass conversion follows from the explicitly chosen self-energy convention.** Subtracting poles alone, instead of the overbarred combination, would leave additional $\log4\pi-\gamma_E$ terms.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
