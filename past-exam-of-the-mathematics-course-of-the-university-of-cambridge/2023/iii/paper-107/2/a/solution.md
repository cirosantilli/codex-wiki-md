<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $c\leq0$, the coefficients are bounded, and $u$ is bounded above. Choose $\kappa$ so large that the bounded positive function $q(y)=e^{\kappa y}$ satisfies

$$
Lq=(a^{nn}\kappa^2+y\kappa+c)q\geq m>0.
$$

Also set $\psi(x)=\log(1+|x|^2)$. Boundedness of the coefficients, $x\mathbin\cdot D\psi\leq2$, and $c\leq0$ give a global upper bound $L\psi\leq C$.

For $\varepsilon>0$ and $0<\delta<\varepsilon m/C$, the function

$$
v=u+\varepsilon q-\delta\psi
$$

tends to $-\infty$ as $|x|\to\infty$ and satisfies $Lv>0$. If $v$ exceeded both zero and its values on $y=\pm1$, it would attain a positive interior maximum. At that point $Dv=0$ and $D^2v\leq0$, whence $Lv\leq cv\leq0$, a contradiction. Letting $\delta\downarrow0$ and then $\varepsilon\downarrow0$ proves

$$
\sup_\Omega u\leq\max\{0,\sup_{\partial\Omega}u\}.
$$

This is the [weak maximum principle for elliptic operators](../../../../../../weak-maximum-principle-for-elliptic-operators.md) on the slab. The boundedness or a comparable growth condition is necessary because the domain is unbounded.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
