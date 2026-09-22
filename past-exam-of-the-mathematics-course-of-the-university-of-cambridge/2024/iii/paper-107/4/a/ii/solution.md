<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $v=\log u_\varepsilon$, so $Dv=Du/u_\varepsilon$. Choose a cutoff $\eta$ which equals one on $B_\rho(z)\cap B_1$, is supported in a comparable ball inside $B_2$, and satisfies $|D\eta|\leq C/\rho$. Repeating the calculation from part (i) with $\eta^2$ and using $|q|\leq\mu$ gives the [Caccioppoli inequality](../../../../../../../caccioppoli-inequality.md)

$$
\int\eta^2|Dv|^2
\leq C\int|D\eta|^2+C\mu\int\eta^2
\leq C(n,\mu)\rho^{n-2}.
$$

The same construction works for balls meeting $\partial B_1$ because the cutoff is supported in $B_2$. Hence

$$
\boxed{\rho^{2-n}\int_{B_\rho(z)\cap B_1}
\frac{|Du_\varepsilon|^2}{u_\varepsilon^2}\leq K(n,\mu).}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 107](../../../../paper-107-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
