<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the uniformly filled narrowing vessel of the preceding part. A bubble within its uniform bubbly region sees

$$
\phi(t)=\frac{\phi_0e^{ct}}{1-\phi_0+\phi_0e^{ct}},\qquad c=2\beta V_s.
$$

Its material rise speed is $\dot\eta=V_s(1-\phi(t))$, not the concentration-characteristic speed. Integrating from $\eta(0)=0$ gives

$$
\boxed{\eta(t)=V_st-\frac1{2\beta}\log\left(1-\phi_0+\phi_0e^{2\beta V_st}\right)
=-\frac1{2\beta}\log\left[\phi_0+(1-\phi_0)e^{-2\beta V_st}\right].}
$$

The cylindrical limit $\beta\to0$ is $\eta=V_s(1-\phi_0)t$, as required. The bottom clearing front follows this same position by the local [Rankine-Hugoniot condition](../../../../../../rankine-hugoniot-conditions.md). In the narrowing vessel the formula applies until the bubble leaves at $z_0+\eta=H$, or a boundary interaction changes the uniform state. Its formal large-time limit is $\eta_\infty=\log(1/\phi_0)/(2\beta)$, while $\phi\to1$. Crowding and liquid backflow invalidate the assumed dilute, negligible-liquid-velocity closure before this limit is a reliable prediction of a real tankard.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
