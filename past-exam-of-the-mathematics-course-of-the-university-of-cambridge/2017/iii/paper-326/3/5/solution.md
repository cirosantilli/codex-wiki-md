<h1 id="3/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

First use the usual [Hilbert space](../../../../../../hilbert-space-split.md) convention for the [proximal operator](../../../../../../proximal-operator.md), identifying the dual element $z$ with its representing vector. For $c\ne0$, completing the square gives

$$
\frac12\|x-q\|^2+\langle x,z\rangle=\frac12\|x-(q-z)\|^2+\text{constant}.
$$

Set $v=cx-y$ and multiply the objective by $c^2$. Its variable part becomes $\|v-[c(q-z)-y]\|^2/2+\alpha c^2J(v)$. Thus the [proximal operator under affine rescaling](../../../../../../proximal-operator-under-affine-rescaling.md) is

$$
\boxed{\operatorname{prox}_E(q)=\frac{y+\operatorname{prox}_{\alpha c^2J}(c(q-z)-y)}c\qquad(c\ne0).}
$$

Negative $c$ is allowed. If $c=0$ and $J(-y)<\infty$, the penalty is constant and the answer is $q-z$. If $c=0$ and $J(-y)=\infty$, $E$ is identically infinite, so there is no proper proximal problem.

The PDF actually assumes an arbitrary [Banach space](../../../../../../banach-space-split.md), so the Hilbert input shift cannot be asserted literally under its hypotheses. Define $\operatorname{Prox}_F(s)=\arg\min_v\{F(v)+\|v-s\|^2/2\}$ as a possibly empty or set-valued minimizer set. Absolute homogeneity of the [norm](../../../../../../norm.md) still gives the valid change of variables

$$
\boxed{\operatorname{Prox}_E(q)=\frac{y+\operatorname{Prox}_{\alpha c^2J+c\langle\cdot,z\rangle}(cq-y)}c\qquad(c\ne0).}
$$

This retains the linear term, rather than shifting by a dual vector. Equivalently its optimality condition uses the [duality mapping](../../../../../../duality-mapping.md) $\mathcal J=\partial(\|\cdot\|^2/2)$:

$$
0\in\mathcal J(x-q)+\alpha c\,\partial J(cx-y)+z.
$$

For a concrete failure of the Hilbert shortcut, take $(\mathbb R^2,\|\cdot\|_1)$, $J=0$, $q=y=0$, $c=1$ and $z=(1,1)$. Every $x_1,x_2\leq0$ with $x_1+x_2=-1$ minimizes $\|x\|_1^2/2+x_1+x_2$ with value $-1/2$. The naive shifted answer $(-1,-1)$ has value zero and is not a minimizer. Hence **the simple shifted formula requires Hilbert geometry; general Banach proximal minimizers need not be unique**. For $c=0$ with finite constant penalty the Banach condition is $-z\in\mathcal J(x-q)$, not generally $x=q-z$.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
