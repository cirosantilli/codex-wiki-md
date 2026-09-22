<h1 id="b/6/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The operator is **well-defined in every dimension**: $|\cos w|\leq1$ gives

$$
|\langle A(w,u),v\rangle|\leq\|\nabla u\|_2\|\nabla v\|_2\leq\|u\|_{H^1}\|v\|_{H^1}.
$$

For fixed $w$, its monotonicity condition is

$$
\langle A(w,u)-A(w,z),u-z\rangle=\int_\Omega\cos(w)|\nabla(u-z)|^2\geq0.
$$

Thus $\cos w\geq0$ [almost everywhere](../../../../../../almost-everywhere.md) is sufficient. It is also necessary, by the [positivity criterion for a scalar gradient form](../../../../../../positivity-criterion-for-a-scalar-gradient-form.md). Indeed, if the bounded coefficient $c=\cos w$ is negative on a set of positive measure, choose a [Lebesgue point](../../../../../../lebesgue-point.md) $x_0$ with $c(x_0)<0$ and a nonconstant compactly supported smooth $\psi$. Set $z_\varepsilon(x)=\varepsilon\psi((x-x_0)/\varepsilon)$, supported inside $\Omega$. Then

$$
\varepsilon^{-n}\int_\Omega c(x)|\nabla z_\varepsilon(x)|^2\,dx\longrightarrow c(x_0)\int|\nabla\psi|^2<0,
$$

contradicting monotonicity. Therefore $\boxed{A(w,\cdot)\text{ is monotone exactly when }\cos w\geq0\text{ almost everywhere}}$. In particular it is not monotone for every $w$: the admissible constant $w\equiv\pi$ makes it the negative Dirichlet form.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [B](../../../../b.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the methods of applied functional analysis course of the University of Oxford](../../../../../split.md)
7. [Methods of applied functional analysis course of the University of Oxford](../../../../../../methods-of-applied-functional-analysis-course-of-the-university-of-oxford.md)
8. [Year 4 of the mathematics course of the University of Oxford](../../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
