<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Suppose $X=U_1\cup\cdots\cup U_n$ with each $U_i$ an [affine open subscheme](../../../../affine-open-subscheme.md). Every [affine scheme](../../../../affine-scheme.md) is a [quasi-compact topological space](../../../../compact-space.md): a cover by [principal open subsets](../../../../principal-open-subscheme.md) $D(f_\lambda)$ means that the $f_\lambda$ generate the [unit ideal](../../../../unit-ideal.md); an expression $1=\sum_{j=1}^r a_jf_{\lambda_j}$ gives a finite subcover. Every [open cover](../../../../open-cover.md) has a refinement by [principal open subsets](../../../../principal-open-subscheme.md), so this proves the general covering property.

Restrict an arbitrary [open cover](../../../../open-cover.md) of $X$ to each $U_i$ and choose a finite subcover there. The union of these finitely many finite families covers $X$. Thus $X$ is a [quasi-compact scheme](../../../../quasi-compact-scheme.md).

Now assume $X$ is a [separated scheme](../../../../separated-scheme.md). By (c), every finite intersection of the $U_i$ is an [affine scheme](../../../../affine-scheme.md), and hence has vanishing positive [sheaf cohomology](../../../../sheaf-cohomology.md) for the [structure sheaf](../../../../structure-sheaf-of-a-scheme.md). This [affine open cover](../../../../affine-open-cover.md) therefore computes [sheaf cohomology](../../../../sheaf-cohomology.md) using its [Čech cochain complex](../../../../cech-cochain-complex.md). Its degree $p$ term is

$$
\check C^p=\prod_{1\leq i_0<\cdots<i_p\leq n}\Gamma(U_{i_0}\cap\cdots\cap U_{i_p},\mathcal O_X).
$$

There are no strictly increasing $(p+1)$-tuples when $p\geq n$, so those [Čech cochain groups](../../../../cech-cochain-group.md) vanish. Consequently

$$
\boxed{H^m(X,\mathcal O_X)=0\qquad(m\geq n).}
$$

The same argument works for every [quasi-coherent sheaf](../../../../quasi-coherent-sheaf.md). The relevant comparison requires the acyclicity of the finite intersections; the bare assertion that arbitrary [Čech cohomology](../../../../cech-cohomology.md) equals [sheaf cohomology](../../../../sheaf-cohomology.md) would be too broad.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
