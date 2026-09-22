<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [finite-rank operator](../../../../../../finite-rank-operator.md) $T$, define $|T|=(T^*T)^{1/2}$ and its [trace norm](../../../../../../trace-norm.md) by

$$
\boxed{\|T\|_1=\operatorname{Tr}|T|=\sum_{j=1}^r s_j,}
$$

where $s_j>0$ are its nonzero [singular values](../../../../../../singular-value.md), counted with multiplicity. The finite-rank spectral theorem gives orthonormal systems $(u_j),(v_j)$ with $T=\sum_js_jR_{u_j,v_j}$, where $R_{x,y}z=\langle z,y\rangle x$.

For every [bounded operator](../../../../../../continuous-linear-operator.md) $B$,

$$
\operatorname{Tr}(BT)=\sum_js_j\langle Bu_j,v_j\rangle,
\qquad |\operatorname{Tr}(BT)|\leq\|B\|\sum_js_j.
$$

Choose the contraction $B$ taking $u_j$ to $v_j$ and vanishing on their [orthogonal complement](../../../../../../orthogonal-complement.md). It attains equality, so

$$
\boxed{\|T\|_1=\sup_{\|B\|\leq1}|\operatorname{Tr}(BT)|.}
$$

This formula proves the [triangle inequality](../../../../../../triangle-inequality.md) and absolute homogeneity. Also $\|T\|\leq\|T\|_1$, so vanishing of the [trace norm](../../../../../../trace-norm.md) forces $T=0$. Thus it is a [norm](../../../../../../norm.md) on the [vector](../../../../../../vector.md) space of [finite-rank operators](../../../../../../finite-rank-operator.md).

The map $B\mapsto F_B$, where $F_B(T)=\operatorname{Tr}(BT)$, is a bounded linear map into the dual of this normed space. Its [norm](../../../../../../norm.md) is at most $\|B\|$. Rank-one tests give the reverse inequality: $\|R_{x,y}\|_1=\|x\|\|y\|$ and $F_B(R_{x,y})=\langle Bx,y\rangle$, so taking unit [vectors](../../../../../../vector.md) $x,y$ gives $\|F_B\|=\|B\|$.

Conversely, let $F$ be a [bounded linear functional](../../../../../../continuous-linear-functional.md) for the [trace norm](../../../../../../trace-norm.md). The [sesquilinear form](../../../../../../sesquilinear-form.md) $\beta(x,y)=F(R_{x,y})$ satisfies

$$
|\beta(x,y)|\leq\|F\|\|x\|\|y\|.
$$

The [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) gives a unique [bounded operator](../../../../../../continuous-linear-operator.md) $B$ with $\beta(x,y)=\langle Bx,y\rangle$, and $\|B\|\leq\|F\|$. Since every [finite-rank operator](../../../../../../finite-rank-operator.md) is a finite sum of [rank-one operators](../../../../../../rank-one-operator.md), [linearity](../../../../../../linearity.md) implies $F(T)=\operatorname{Tr}(BT)$ for every $T$. Hence

$$
\boxed{(\mathcal F(H),\|\cdot\|_1)^*\cong B(H)\text{ isometrically}.}
$$

The same identification extends to the completion, the [trace-class operators](../../../../../../trace-class-operator.md). This is [trace-class duality](../../../../../../trace-class-duality.md); completeness of the original finite-rank space is not required to identify its bounded dual.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
