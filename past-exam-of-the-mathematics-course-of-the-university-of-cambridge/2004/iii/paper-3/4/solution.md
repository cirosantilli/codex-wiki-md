<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Name the four vertices $1,2,\bar2,\bar1$ in their displayed order. This is the [crystal of the defining symplectic representation](../../../../../crystal-of-the-defining-symplectic-representation.md) in rank two, of [highest weight](../../../../../highest-weight-of-a-representation.md) $\omega_1$ for the [C2 root system](../../../../../c2-root-system.md). Its [weights](../../../../../weight-representation-theory.md) are respectively $\varepsilon_1,\varepsilon_2,-\varepsilon_2,-\varepsilon_1$, with [simple roots](../../../../../simple-root.md) $\alpha_1=\varepsilon_1-\varepsilon_2$ and $\alpha_2=2\varepsilon_2$. Each lowering arrow subtracts the corresponding simple root. Thus $\omega_1=\varepsilon_1$ and $\omega_2=\varepsilon_1+\varepsilon_2$.

Use the [crystal tensor-product rule](../../../../../crystal-tensor-product-rule.md) in which $\widetilde f_i$ acts on the first factor if $\varphi_i(a)>\varepsilon_i(b)$, and on the second factor otherwise. The raising operator $\widetilde e_i$ acts on the first factor for $\varphi_i(a)\geq\varepsilon_i(b)$, on the second otherwise. Here $\varepsilon_i(b)$ and $\varphi_i(b)$ count the raising and lowering steps available in color $i$. The data for the four vertices are

$$
\begin{array}{c|cccc}b&1&2&\bar2&\bar1\\\hline\varepsilon_1(b)&0&1&0&1\\\varphi_1(b)&1&0&1&0\\\varepsilon_2(b)&0&0&1&0\\\varphi_2(b)&0&1&0&0\end{array}.
$$

The strictness difference between raising and lowering ensures that they are inverse along each colored edge. Testing the sixteen ordered tensor vertices gives exactly three vertices killed by both raising [Kashiwara operators](../../../../../kashiwara-operator.md):

$$
1\otimes1,\qquad1\otimes2,\qquad1\otimes\bar1.
$$

Their [highest weights](../../../../../highest-weight-of-a-representation.md) are $2\varepsilon_1=2\omega_1$, $\varepsilon_1+\varepsilon_2=\omega_2$ and zero.

For completeness, successive lowering generates the following connected components of the [tensor product of crystals](../../../../../tensor-product-of-crystals.md):

- From $1\otimes1$: $1\otimes1$, $2\otimes1$, $2\otimes2$, $\bar2\otimes1$, $\bar2\otimes2$, $\bar2\otimes\bar2$, $\bar1\otimes1$, $\bar1\otimes2$, $\bar1\otimes\bar2$, $\bar1\otimes\bar1$.
- From $1\otimes2$: $1\otimes2$, $1\otimes\bar2$, $2\otimes\bar2$, $2\otimes\bar1$, $\bar2\otimes\bar1$. Their edge colors in order are $2,1,1,2$.
- The vertex $1\otimes\bar1$ is isolated.

They have sizes ten, five and one, are disjoint, and exhaust all sixteen vertices. This proves the [tensor square of the defining C2 crystal](../../../../../tensor-square-of-the-defining-c2-crystal.md) decomposition

$$
\boxed{B\otimes B\cong B(2\omega_1)\sqcup B(\omega_2)\sqcup B(0),\qquad\dim=10+5+1.}
$$

Equivalently, the representation decomposes as $L(\omega_1)^{\otimes2}=L(2\omega_1)\oplus L(\omega_2)\oplus L(0)$. The dimensions agree with the [Weyl dimension formula for C2](../../../../../weyl-dimension-formula-for-c2.md), $\dim L(a\omega_1+b\omega_2)=(a+1)(b+1)(a+b+2)(a+2b+3)/6$. The ordered highest vertices would change under the opposite tensor convention, but the irreducible decomposition would be the same.

<a id="4/image-the-ten-five-and-one-vertex-components-of-the-c2-tensor-square-crystal"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-3-crystal-components.png)

**[Figure 2](#4/image-the-ten-five-and-one-vertex-components-of-the-c2-tensor-square-crystal). The ten-, five- and one-vertex components of the C2 tensor-square crystal**.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
