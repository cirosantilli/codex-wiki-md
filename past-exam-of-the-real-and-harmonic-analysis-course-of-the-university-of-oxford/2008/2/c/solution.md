<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [regular outer measure](../../../../regular-outer-measure.md) has a measurable hull of equal [outer measure](../../../../outer-measure.md) for every set: for each $A$ there is measurable $G\supseteq A$ with $\mathcal L^*(G)=\mathcal L^*(A)$. [Lebesgue outer measure](../../../../lebesgue-outer-measure.md) has even a Borel hull. If its value on $A$ is finite, choose open-box covers of total cost below $\mathcal L^*(A)+1/j$, and let $U_j$ be their open unions. Then $G=\bigcap_jU_j$ is Borel and

$$
\mathcal L^*(A)\leq\mathcal L^*(G)\leq\mathcal L^*(U_j)\leq\mathcal L^*(A)+1/j.
$$

For infinite [outer measure](../../../../outer-measure.md) the whole space is a suitable hull. Thus **[Lebesgue outer measure](../../../../lebesgue-outer-measure.md) is regular**.

If $A$ is measurable, additivity immediately gives the requested equality. Conversely suppose the equality holds. Choose a measurable hull $G$ of $A$ and put $B=G\cap M$. Then $A\subseteq B\subseteq M$ and $\mathcal L(B)=\mathcal L^*(A)$. Since $B$ is measurable, its splitting of $M\setminus A$ gives

$$
\mathcal L^*(M\setminus A)=\mathcal L(M\setminus B)+\mathcal L^*(B\setminus A).
$$

The assumed equality and $\mathcal L(M)=\mathcal L(B)+\mathcal L(M\setminus B)$ imply $\mathcal L^*(B\setminus A)=0$. These subtractions are legitimate because $\mathcal L(M)<\infty$. Outer-[measure](../../../../measure-split.md)-[null sets](../../../../null-set.md) are measurable by the [Caratheodory criterion](../../../../caratheodory-s-criterion.md). Hence $A=B\setminus(B\setminus A)$ is measurable, proving **the equivalence**.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
