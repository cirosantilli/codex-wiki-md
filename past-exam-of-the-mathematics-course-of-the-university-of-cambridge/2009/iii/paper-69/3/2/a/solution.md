<h1 id="3/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For unit-spaced knots, the [quadratic cardinal B-spline](../../../../../../../quadratic-cardinal-b-spline.md) is a translate of

$$
N_{j,3}(t)=
\begin{cases}
(t-j)^2/2,&j\le t\le j+1,\\
3/4-(t-j-3/2)^2,&j+1\le t\le j+2,\\
(j+3-t)^2/2,&j+2\le t\le j+3,\\
0,&\text{otherwise}.
\end{cases}
$$

For example, the [Cox-de Boor recurrence](../../../../../../../cox-de-boor-recursion-formula.md) gives $N_{j,3}(t)=(t-j)N_{j,2}(t)/2+(j+3-t)N_{j+1,2}(t)/2$ from the two linear hats. Substituting their linear pieces gives the three expressions above. At $x_i=i+3/2$, only the [B-splines](../../../../../../../b-spline.md) with indices $j=i-1,i,i+1$ have nonzero values, and their values are respectively

$$
\boxed{N_j(x_i)=
\begin{cases}
3/4,&j=i,\\
1/8,&|j-i|=1,\\
0,&|j-i|\ge2.
\end{cases}}
$$

Only indices $1\le j\le n$ belong to the given [basis](../../../../../../../basis.md), so entries outside that range are omitted at the boundary.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 69](../../../../paper-69-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
