<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $\gamma=\alpha+\beta$, $E=F(\gamma)$ and $E_0=F(\gamma^p)$. By the preceding [separability criterion using a pth power](../../../../separability-criterion-using-a-pth-power.md), it suffices to prove $E=E_0$.

Since $\alpha$ is separable, $\alpha\in F(\alpha^p)$. But $\alpha^p=\gamma^p-\beta^p\in E_0(\beta)$, so $\alpha\in E_0(\beta)$. Consequently

$$
M:=F(\alpha,\beta)=E(\beta)=E_0(\beta).
$$

Let $h$ and $m$ be the monic [minimal polynomials](../../../../minimal-polynomial.md) of $\beta$ over $E_0$ and $E$, respectively. Both divide its separable minimal polynomial over $F$, so both are separable. Also $m\mid h$ in $E[T]$.

Every $c\in E=F(\gamma)$ has $c^p\in F(\gamma^p)=E_0$. Hence $m(T)^p$ has coefficients in $E_0$ and vanishes at $\beta$, forcing $h\mid m^p$ in $E_0[T]$. Since $h$ remains a [square-free polynomial](../../../../square-free-polynomial.md) over $E$, this divisibility implies $h\mid m$ in $E[T]$. Together with $m\mid h$, monicity gives $h=m$. Therefore

$$
[M:E_0]=\deg h=\deg m=[M:E].
$$

The [tower law](../../../../tower-law.md) makes $[E:E_0]=1$. Part (c) now proves that $\gamma=\alpha+\beta$ is separable over $F$. This establishes [closure of separable algebraic elements under addition](../../../../closure-of-separable-algebraic-elements-under-addition.md) without presupposing that closure as a field theorem.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the galois theory course of the University of Oxford](../../../split.md)
5. [Galois theory course of the University of Oxford](../../../../galois-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
