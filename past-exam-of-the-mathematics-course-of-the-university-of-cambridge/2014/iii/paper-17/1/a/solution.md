<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathcal A^{p,q}(X)$ be the space of smooth complex [differential forms](../../../../../../differential-form-split.md) of type $(p,q)$. The [Dolbeault operator](../../../../../../dolbeault-operator.md) satisfies $\bar\partial^2=0$, and the [Dolbeault cohomology](../../../../../../dolbeault-cohomology.md) is

$$
 \boxed{H_{\bar\partial}^{p,q}(X)=
 \frac{\ker(\bar\partial:\mathcal A^{p,q}\to\mathcal A^{p,q+1})}
 {\operatorname{im}(\bar\partial:\mathcal A^{p,q-1}\to\mathcal A^{p,q})}.}
$$

For $q=0$ the denominator is zero; forms outside the dimension range are zero.

A sequence of [sheaves](../../../../../../sheaf-mathematics.md) is an [exact sequence of sheaves](../../../../../../exact-sequence-of-sheaves.md) precisely when its sequence of [stalks](../../../../../../stalk-of-a-sheaf.md) at every point is exact. Here this means the first map is injective on [stalks](../../../../../../stalk-of-a-sheaf.md), the last is surjective on [stalks](../../../../../../stalk-of-a-sheaf.md), and the image equals the kernel at the middle [stalk](../../../../../../stalk-of-a-sheaf.md). In particular, a section of the last [sheaf](../../../../../../sheaf-mathematics.md) need only have local lifts; surjectivity on all global sections is not required.

The associated [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) of [Čech cohomology](../../../../../../cech-cohomology.md), understood in the direct limit over open covers, is

$$
 \begin{aligned}
 0&\longrightarrow\check H^0(X,\mathcal F)
 \longrightarrow\check H^0(X,\mathcal E)
 \longrightarrow\check H^0(X,\mathcal G)
 \xrightarrow{\delta_0}\check H^1(X,\mathcal F)\longrightarrow\cdots\\
 &\longrightarrow\check H^q(X,\mathcal F)
 \longrightarrow\check H^q(X,\mathcal E)
 \longrightarrow\check H^q(X,\mathcal G)
 \xrightarrow{\delta_q}\check H^{q+1}(X,\mathcal F)\longrightarrow\cdots.
 \end{aligned}
$$

The degree-zero groups are global sections. The connecting map is obtained by locally lifting a [Čech cocycle](../../../../../../cech-cocycle-condition.md) to the middle [sheaf](../../../../../../sheaf-mathematics.md) and taking its [Čech coboundary](../../../../../../cech-coboundary.md), which takes values in the first [sheaf](../../../../../../sheaf-mathematics.md). Different lifts change it by a [Čech coboundary](../../../../../../cech-coboundary.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
