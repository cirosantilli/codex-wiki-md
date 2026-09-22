<h1 id="4/c/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Combining parts (iii) and (iv), then multiplying by $1+\varepsilon$, gives

$$
H(A|B)_\sigma-H(A|B)_\rho
\leq\varepsilon\bigl(H(A|B)_{\Delta'}-H(A|B)_\Delta\bigr)
+(1+\varepsilon)H\!\left(\frac{\varepsilon}{1+\varepsilon}\right).
$$

The [dimension bound for quantum conditional entropy](../../../../../../../dimension-bound-for-quantum-conditional-entropy.md) is

$$
-\log d_A\leq H(A|B)_\tau\leq\log d_A.
$$

Indeed, [Subadditivity of Von Neumann entropy](../../../../../../../subadditivity-of-von-neumann-entropy.md) gives $H(A|B)_\tau\leq S(\tau_A)\leq\log d_A$, while the [Araki–Lieb inequality](../../../../../../../araki-lieb-inequality.md) gives $H(A|B)_\tau\geq-S(\tau_A)\geq-\log d_A$. Hence

$$
H(A|B)_\sigma-H(A|B)_\rho
\leq2\varepsilon\log d_A
+(1+\varepsilon)H\!\left(\frac{\varepsilon}{1+\varepsilon}\right).
$$

Interchanging $\rho$ and $\sigma$ proves the [continuity bound for quantum conditional entropy](../../../../../../../continuity-bound-for-quantum-conditional-entropy.md):

$$
\boxed{|H(A|B)_\rho-H(A|B)_\sigma|
\leq2\varepsilon\log d_A
+(1+\varepsilon)H\!\left(\frac{\varepsilon}{1+\varepsilon}\right)}.
$$

## ↑ Ancestors (12)

1. [V](../v.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
