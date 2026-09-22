<h1 id="13e/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $N(t)$ count roots in the open [unit disk](../../../../../../unit-disk.md). A boundary crossing can occur only at the real values $0,\pm1,\pm2$ found above, so the count is constant between them. Also $N(-t)=N(t)$, because the [polynomial](../../../../../../polynomial-split.md) is odd. At $t=0$, $p(z)=z(z^4+1)$ has one root inside and four on the [circle](../../../../../../circle.md), giving $N(0)=1$.

For small positive $t$, the root near zero stays inside. At each boundary root $\zeta^4=-1$, $p'(\zeta)=-4$, so implicit differentiation gives $z(t)=\zeta-t/4+O(t^2)$. The [radial crossing test for polynomial root counts](../../../../../../radial-crossing-test-for-polynomial-root-counts.md) is

$$
\left.\frac d{dt}\log|z(t)|\right|_{t=0}=-\frac{\operatorname{Re}\zeta}{4}.
$$

The two roots with positive real part enter and the other two leave. Hence $N(t)=3$ for $0<t<1$.

At $t=1$, the boundary roots are $\zeta=e^{\pm i\pi/3}$. Since $\zeta p'(\zeta)=5t-4\zeta$, their radial derivative is $\operatorname{Re}(1/(5-4\zeta))=1/7>0$. Both leave as $t$ increases, so the count becomes one; at $t=1$ itself they are excluded, also leaving one interior root. At $t=2$, the remaining boundary root $z=1$ has radial derivative $1/6>0$ and leaves. For $t\ge2$ no interior root is possible, since $|p(z)|\le |z|^5+|z|<2$ in the open [disk](../../../../../../disk-mathematics.md). Combining these facts and odd symmetry gives

$$
\boxed{N(t)=\begin{cases}
3,&0<|t|<1,\\
1,&t=0\ \text{or}\ 1\le|t|<2,\\
0,&|t|\ge2.
\end{cases}}
$$

This also gives the corresponding [winding numbers](../../../../../../winding-number.md) of the [image](../../../../../../image-of-a-function.md) [contour](../../../../../../complex-integration-contour.md) away from its crossings. Boundary roots are excluded at the crossing values; using a nearby [winding number](../../../../../../winding-number.md) at $t=0$ would incorrectly count two extra roots.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [13E](../../13e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
