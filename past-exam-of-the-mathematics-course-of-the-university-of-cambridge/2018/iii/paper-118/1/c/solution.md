<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A pure-type $d$-closed form is both $\partial$-closed and $\bar\partial$-closed, because these two derivatives have different types. Let $k=p+q$. The smooth [Poincaré lemma](../../../../../../poincare-lemma.md) on the [polydisc](../../../../../../polydisc.md) gives $\eta\in\mathcal A^{k-1}_{\mathbb C}$ with $d\eta=\alpha$. We will modify $\eta$ by exact terms without changing $d\eta$.

Write $\eta=\sum_r\eta^{r,k-1-r}$. Starting with the smallest holomorphic degree, eliminate every component with $r<p-1$. Once the lower components are zero, the $(r,k-r)$ component of $d\eta$ says $\bar\partial\eta^{r,k-1-r}=0$, since $r<p$. Its antiholomorphic degree is positive, so the [Dolbeault-Poincaré lemma](../../../../../../dolbeault-poincare-lemma.md) supplies $\nu^{r,k-2-r}$ with $\bar\partial\nu=\eta^{r,k-1-r}$. Replace $\eta$ by $\eta-d\nu$: this removes the component at $r$ and changes only the next holomorphic degree.

Next, work downwards from the largest holomorphic degree and eliminate the components with $r>p$. Once the higher components are zero, the corresponding component of $d\eta$ gives $\partial\eta^{r,k-1-r}=0$. By part (b), write this as $\partial\nu^{r-1,k-1-r}$ and again subtract $d\nu$. This affects only the next lower holomorphic degree. The two finite procedures leave

$$
\eta=u+v,\qquad u\in\mathcal A^{p-1,q},\quad v\in\mathcal A^{p,q-1}.
$$

The components of $d\eta=\alpha$ outside type $(p,q)$ now give $\bar\partial u=0$ and $\partial v=0$, while its $(p,q)$ component gives $\alpha=\partial u+\bar\partial v$.

Since $q\geq1$, the [Dolbeault-Poincaré lemma](../../../../../../dolbeault-poincare-lemma.md) gives $u=\bar\partial a$ with $a$ of type $(p-1,q-1)$. Since $p\geq1$, part (b) gives $v=\partial b$ of the same type. The anticommutation identity therefore yields

$$
\alpha=\partial\bar\partial a+\bar\partial\partial b=\partial\bar\partial(a-b).
$$

This proves the [Bott-Chern Poincaré lemma](../../../../../../bott-chern-poincare-lemma.md) using precisely the permitted primitives:

$$
\boxed{H_{BC}^{p,q}(\mathcal P^n)=0\qquad(p,q\geq1).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
