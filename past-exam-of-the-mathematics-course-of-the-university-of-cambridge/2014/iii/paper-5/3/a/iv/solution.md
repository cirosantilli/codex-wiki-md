<h1 id="3/a/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Work in the [mean-zero Sobolev space](../../../../../../../mean-zero-sobolev-space.md)

$$
H=\left\{v\in H^1(U):\int_Uv=0\right\},\qquad a(u,v)=\int_U\nabla u\cdot\nabla v.
$$

The integral is a continuous functional on $H^1(U)$, so $H$ is closed. The [Neumann-Poincare inequality](../../../../../../../poincare-wirtinger-inequality.md) shows that $\|v\|_a=\|\nabla v\|_2$ is equivalent to the usual $H^1$ [norm](../../../../../../../norm.md) on $H$, making $a$ a complete [inner product](../../../../../../../inner-product.md) there.

For $f\in L^2(U)$ the functional $L(v)=\int_Ufv$ satisfies

$$
|L(v)|\leq\|f\|_2\|v\|_2\leq\sqrt{C_P}\|f\|_2\|v\|_a.
$$

The [Riesz representation theorem](../../../../../../../riesz-representation-theorem.md), or the [Lax-Milgram theorem](../../../../../../../lax-milgram-theorem.md), gives a unique $u\in H$ with $a(u,v)=L(v)$ for all $v\in H$. To recover every $H^1(U)$ test, write $v=(v-v_U)+v_U$. The constant contributes zero to $a$ and contributes $v_U\int_Uf=0$ to $L$. Thus the same equality holds for all $v\in H^1(U)$.

**A [weak solution](../../../../../../../weak-solution.md) exists whenever $\int_Uf=0$; fixing its average to zero makes it unique.** Moreover $\|\nabla u\|_2\leq\sqrt{C_P}\|f\|_2$ and the [Neumann-Poincare inequality](../../../../../../../poincare-wirtinger-inequality.md) also controls $\|u\|_2$.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 5](../../../../paper-5-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
