<h1 id="13c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Extend the forcing oddly across the boundary:

$$
f_{\rm odd}(y,s)=
\begin{cases}
f(y,s),&y\geq0,\\
-f(-y,s),&y<0.
\end{cases}
$$

The initial displacement $\sin x$ is already odd, so its homogeneous evolution on the line is $\sin x\cos(ct)$. Applying [Duhamel's principle](../../../../../../duhamel-s-principle.md) to the odd extension gives

$$
\boxed{
u(x,t)=\sin x\cos(ct)
+\frac1{2c}\int_0^t
\int_{x-c(t-s)}^{x+c(t-s)}
f_{\rm odd}(y,s)\,dy\,ds }.
$$

The odd-reflection method makes $u(0,t)=0$. At $t=0$ the double integral vanishes together with its first time derivative, so the prescribed initial displacement and velocity are also satisfied.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [13C](../../13c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
