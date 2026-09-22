<h1 id="11c/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the auxiliary [point charge](../../../../../../point-charge.md) of strength $q\ne0$ at the origin, with potential $\phi_2=q/(4\pi\varepsilon_0r)$ from part (a). Apply the [electrostatic reciprocity identity](../../../../../../electrostatic-reciprocity-identity.md) of part (b) to the exterior region $a<r<R$, then let $R\to\infty$. Its inner boundary has outward normal $-\mathbf e_r$, and $\rho_2=0$ everywhere in this exterior region. The outer boundary terms vanish under the stipulated decay assumption.

On $r=a$, $\phi_1=\Phi$ and

$$
\nabla\phi_2\cdot(-\mathbf e_r)=\frac{q}{4\pi\varepsilon_0a^2}.
$$

Thus the surviving boundary term on the left is $\Phi q/\varepsilon_0$. On the right, $\phi_2$ is constant on the inner sphere, so its boundary term is

$$
\frac{q}{4\pi\varepsilon_0a}\int_{r=a}\nabla\phi_1\cdot(-\mathbf e_r)\,dS=0.
$$

Indeed, $\nabla\phi_1=-\mathbf E_1$, and this integral is the outward electric flux from the interior ball, whose enclosed charge is zero by the hypothesis and [Gauss's law](../../../../../../gauss-s-law.md). No symmetry of the exterior charge distribution is needed.

The [electrostatic reciprocity identity](../../../../../../electrostatic-reciprocity-identity.md) now reduces to

$$
\frac{q\Phi}{\varepsilon_0}
=\frac1{\varepsilon_0}\int_{r>a}\frac{q\rho_1(\mathbf x)}{4\pi\varepsilon_0r}\,dV.
$$

Canceling $q/\varepsilon_0$ gives

$$
\boxed{\Phi=\frac1{4\pi\varepsilon_0}\int_{r>a}\frac{\rho_1(\mathbf x)}{r}\,dV.}
$$

The inward normal on the inner boundary is essential to the positive sign in this result.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
