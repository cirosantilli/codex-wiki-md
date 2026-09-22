<h1 id="a/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Writing matrices in $2\times2$ blocks, the defining relation gives

$$
L=\left\{\begin{pmatrix}A&B\\C&-A^T\end{pmatrix}:B^T=-B,\ C^T=-C\right\}.
$$

The [trace](../../../../../matrix-trace.md) is automatically zero. The relation is linear, and if $as=-sa^T$, $bs=-sb^T$, then

$$
[a,b]s=s(a^Tb^T-b^Ta^T)=-s[a,b]^T.
$$

Thus $L$ is closed under the [commutator](../../../../../commutator.md) and is a [Lie subalgebra](../../../../../lie-subalgebra.md) of $\mathfrak{sl}_4(F)$.

Its diagonal subalgebra is

$$
H=\{D(a,b)=\operatorname{diag}(a,b,-a,-b):a,b\in F\}.
$$

Put $\varepsilon_1(D(a,b))=a$, $\varepsilon_2(D(a,b))=b$. Since $[D,E_{ij}]=(D_{ii}-D_{jj})E_{ij}$, the required block decomposition is

$$
\boxed{\begin{aligned}
L={}&H\oplus F(E_{12}-E_{43})\oplus F(E_{21}-E_{34})\\
&\oplus F(E_{14}-E_{23})\oplus F(E_{32}-E_{41}).
\end{aligned}}
$$

The four lines have respective characters $\varepsilon_1-\varepsilon_2$, $-\varepsilon_1+\varepsilon_2$, $\varepsilon_1+\varepsilon_2$, $-\varepsilon_1-\varepsilon_2$. They are distinct and nonzero because $\operatorname{char}F\ne2$. The two-dimensional summand $H$ has two trivial composition factors. These five submodules therefore have exactly the factor-grouping properties of part (b). Their dimensions sum to $6$, the [dimension](../../../../../dimension-vector-space.md) obtained from four free entries in $A$ and one each in the skew-symmetric blocks $B,C$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../split.md)
6. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
