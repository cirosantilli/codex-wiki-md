<h1 id="23h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By part (a), $B$ is a [bounded bilinear form](../../../../../../bounded-bilinear-form.md): $|B(u,v)|\leq M\lVert u\rVert\lVert v\rVert$. For each fixed $v$, the map $u\mapsto B(u,v)$ is consequently a [bounded linear functional](../../../../../../continuous-linear-functional.md). The [Riesz representation theorem](../../../../../../riesz-representation-theorem.md) supplies a unique vector $Lv$ such that

$$
B(u,v)=\langle u,Lv\rangle
\qquad(u\in\mathcal H).
$$

Uniqueness of the representing vector makes $L$ [linear](../../../../../../linearity.md), and $\lVert Lv\rVert\leq M\lVert v\rVert$ makes it a [bounded linear operator](../../../../../../continuous-linear-operator.md).

The [coercivity](../../../../../../coercive-bilinear-form.md) assumption implies

$$
C\lVert v\rVert^2\leq B(v,v)=\langle v,Lv\rangle
\leq\lVert v\rVert\lVert Lv\rVert,
$$

hence $\lVert Lv\rVert\geq C\lVert v\rVert$. Moreover, using the [adjoint operator](../../../../../../adjoint-operator.md),

$$
\langle v,L^*v\rangle=\langle Lv,v\rangle=B(v,v),
$$

so the same argument gives $\lVert L^*v\rVert\geq C\lVert v\rVert$. The [invertibility from lower bounds on an operator and its adjoint](../../../../../../invertibility-from-lower-bounds-on-an-operator-and-its-adjoint.md) therefore shows that $L$ is invertible and $L^{-1}$ is bounded.

Set $v_f=L^{-1}f$. Then $B(u,v_f)=\langle u,Lv_f\rangle=\langle u,f\rangle$ for every $u$. If another $v$ has this property, then $L(v-v_f)=0$, and the injectivity of $L$ gives $v=v_f$. Thus **the unique vector is $v_f=L^{-1}f$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [23H](../../23h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
