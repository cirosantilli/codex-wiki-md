<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $\mathcal A$ in the $n$-dimensional [Boolean hypercube](../../../../../../boolean-hypercube.md), the [edge-isoperimetric inequality in the discrete cube](../../../../../../edge-isoperimetric-inequality-in-the-discrete-cube.md) is

$$
e(\mathcal A)\leq\frac{|\mathcal A|\log_2|\mathcal A|}{2},
$$

where $e(\mathcal A)$ is the number of edges spanned by $\mathcal A$. Since the cube is $n$-regular, the equivalent boundary form is

$$
|\partial_e\mathcal A|
=n|\mathcal A|-2e(\mathcal A)
\geq|\mathcal A|\log_2\frac{2^n}{|\mathcal A|}.
$$

We prove the induced-edge form by induction on $n$. Split the cube according to its last coordinate, and let the two sections have sizes $a\geq b$. At most $b$ edges of $\mathcal A$ cross between the sections. The induction hypothesis gives

$$
e(\mathcal A)\leq\frac12a\log_2a+\frac12b\log_2b+b.
$$

Put $x=b/(a+b)\leq1/2$. The required comparison with $\frac12(a+b)\log_2(a+b)$ is equivalent to

$$
H_2(x)\geq2x,
$$

where $H_2$ is the [binary entropy function](../../../../../../binary-entropy-function.md). This follows from concavity because the graph of $H_2$ lies above the chord joining $(0,0)$ to $(1/2,1)$. The induction is complete. Subcubes attain equality when $|\mathcal A|$ is a power of two.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
