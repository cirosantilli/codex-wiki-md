<h1 id="3d/solution">Solution</h1>

↑ **Parent:** [3D](../3d.md)

The definition of a [convergent sequence](../../../../../convergent-sequence.md) is

$$
\boxed{\forall\epsilon>0\ \exists N\ \forall n\ge N:\ |u_n-l|<\epsilon.}
$$

To prove the product rule, convergence first gives an eventual bound $|u_n|\le |l|+1=:M$. Then

$$
|u_nv_n-lk|=|u_n(v_n-k)+k(u_n-l)|\le M|v_n-k|+|k||u_n-l|.
$$

Choose $n$ sufficiently large that $|v_n-k|<\epsilon/(2M)$ and $|u_n-l|<\epsilon/[2(|k|+1)]$, as well as the bound on $u_n$. The right side is less than $\epsilon$, proving **$u_nv_n\to lk$** directly from the [limit of a sequence](../../../../../limit-of-a-sequence.md) definition.

If $l\ne0$, eventually $|u_n-l|<|l|/2$, so the [reverse triangle inequality](../../../../../reverse-triangle-inequality.md) gives $|u_n|>|l|/2$. Consequently

$$
\left|\frac1{u_n}-\frac1l\right|=\frac{|u_n-l|}{|u_n||l|}\le\frac{2|u_n-l|}{|l|^2}\longrightarrow0.
$$

Thus **$1/u_n\to1/l$**. The condition $u_n\ne0$ ensures the reciprocal sequence is defined at every index; the nonzero limit supplies the eventual uniform bound away from zero. Finally $\boxed{u_n=1/(n+1)\to0}$ has every term nonzero, showing that this termwise property alone does not prevent a zero limit.

## ↑ Ancestors (10)

1. [3D](../3d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
