<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Identify $\mathfrak t$ with the coordinate vector $t=(t_1,\ldots,t_n)$ through $H(t)$. A [root reflection](../../../../../../root-reflection.md) is $s_\alpha(H)=H-\alpha(H)\alpha^\vee$. Since $(\varepsilon_i\pm\varepsilon_j)^\vee=H_i\pm H_j$, for $i<j$ the two possibilities are

$$
\boxed{\begin{aligned}s_{\varepsilon_i-\varepsilon_j}(t)_i&=t_j,&s_{\varepsilon_i-\varepsilon_j}(t)_j&=t_i,\\s_{\varepsilon_i+\varepsilon_j}(t)_i&=-t_j,&s_{\varepsilon_i+\varepsilon_j}(t)_j&=-t_i.
\end{aligned}}
$$

Every other coordinate is unchanged, and $s_{-\alpha}=s_\alpha$, so these formulas cover every [root](../../../../../../root-of-a-root-system.md). The complete diagonal matrix is reconstructed with its last $n$ entries the reversed negatives of the first $n$ entries.

The [Weyl group of Dn](../../../../../../weyl-group-of-dn.md) consists of all permutations of the $n$ coordinates together with an [even number](../../../../../../even-number.md) of coordinate sign changes. Equivalently,

$$
\boxed{W(D_n)=\{t\mapsto(\delta_i t_{\sigma(i)})_{i=1}^n:\sigma\in S_n,\ \delta_i\in\{\pm1\},\ \prod_i\delta_i=1\}\cong(\mathbb Z/2\mathbb Z)^{n-1}\rtimes S_n.}
$$

Its order is $2^{n-1}n!$. The difference-root reflections give ordinary transpositions; composing a sum-root reflection with the corresponding difference-root reflection negates precisely the two selected coordinates. These describe the generators of all even signed permutations. For $n=2$ the group has four elements; for the toral case $n=1$ it is trivial.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
