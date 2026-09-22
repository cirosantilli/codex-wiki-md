<h1 id="8f/solution">Solution</h1>

↑ **Parent:** [8F](../8f.md)

Use the convention that a [sesquilinear form](../../../../../sesquilinear-form.md) is linear in its first argument and conjugate-linear in its second: for complex scalars $a,b$,

$$
\phi(av_1+bv_2,w)=a\phi(v_1,w)+b\phi(v_2,w),\qquad \phi(v,aw_1+bw_2)=\bar a\phi(v,w_1)+\bar b\phi(v,w_2).
$$

No symmetry or positivity is assumed. Put $\chi=\phi-\psi$. Its diagonal vanishes. Expansion at $v+w$ gives

$$
\chi(v,w)+\chi(w,v)=0,
$$

while expansion at $v+iw$ gives

$$
-i\chi(v,w)+i\chi(w,v)=0.
$$

These two equations force $\chi(v,w)=\chi(w,v)=0$. This is the [polarization argument for a vanishing quadratic form](../../../../../polarization-argument-for-a-vanishing-quadratic-form.md), and proves **$\phi=\psi$ on every pair of vectors**.

For the final deduction, the [linear map](../../../../../linear-map.md) $\alpha$ makes $\psi(v,w)=\phi(\alpha v,\alpha w)$ another [sesquilinear form](../../../../../sesquilinear-form.md). Its diagonal agrees with that of $\phi$, so the result just proved gives

$$
\boxed{\phi(\alpha v,\alpha w)=\phi(v,w)\quad\text{for all }v,w\in V}.
$$

## ↑ Ancestors (10)

1. [8F](../8f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
