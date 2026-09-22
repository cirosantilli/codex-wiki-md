<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The spherically symmetric [Laplace equation](../../../../../../laplace-equation.md) with $\widetilde\phi(R)=\delta(R)$ and $\widetilde\phi(\infty)=\varepsilon$ has solution

$$
\widetilde\phi(r)=\varepsilon+[\delta(R)-\varepsilon]\frac Rr.
$$

Thus

$$
J_r(R^+)=-M\partial_r\mu|_{R^+}
=-\frac{\alpha M}{R}[\varepsilon-\delta(R)].
$$

Conservation at the moving interface, whose composition jump is $2\phi_B$, gives $2\phi_B\dot R=-J_r(R^+)$ and hence

$$
\boxed{\dot R=\frac{\alpha M}{2\phi_BR}[\varepsilon-\delta(R)].}
$$

Since $\delta(R)=C/R$, the right side is proportional to $\varepsilon/R-C/R^2$. It is negative for $R<R^*$, zero at $R^*=C/\varepsilon$, positive for $R>R^*$, and approaches zero from above for large $R$. Thus $R^*$ is the unstable [critical nucleus](../../../../../../critical-nucleus.md): smaller droplets dissolve, while larger droplets grow.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
