<h1 id="5c/solution">Solution</h1>

↑ **Parent:** [5C](../5c.md)

Using [Einstein notation](../../../../../einstein-notation.md) and

$$
\epsilon_{ijk}\epsilon_{klm}
=\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl},
$$

we obtain

$$
\begin{aligned}
[a\times(b\times c)]_i
&=\epsilon_{ijk}a_j\epsilon_{klm}b_lc_m\\
&=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})
a_jb_lc_m\\
&=(a\cdot c)b_i-(a\cdot b)c_i.
\end{aligned}
$$

Thus

$$
\boxed{a\times(b\times c)=(a\cdot c)b-(a\cdot b)c}.
$$

The [scalar triple product](../../../../../scalar-triple-product.md) is

$$
[a,b,c]=a\cdot(b\times c).
$$

Put $\Delta=[a,b,c]$. When $\Delta\ne0$, the three vectors

$$
e'_1=\frac{b\times c}{\Delta},
\qquad
e'_2=\frac{c\times a}{\Delta},
\qquad
e'_3=\frac{a\times b}{\Delta}
$$

form the [reciprocal basis](../../../../../reciprocal-basis.md) to $a,b,c$, so $e'_i\cdot e_j=\delta_{ij}$. Their scalar triple product is $1/\Delta$. Therefore

$$
[a\times b,b\times c,c\times a]
=\Delta^3[e'_3,e'_1,e'_2]
=\boxed{\Delta^2},
$$

since the cyclic permutation preserves orientation. The identity also holds when $\Delta=0$, either by continuity or directly because the cross products are then linearly dependent.

For the given basis $e_1,e_2,e_3$, the same identities give

$$
e'_i\cdot e_j=\delta_{ij}.
$$

If $\sum_i\alpha_ie'_i=0$, dotting with $e_j$ gives $\alpha_j=0$, so the $e'_i$ are linearly independent and hence form a basis. Moreover, $e_i\cdot e'_j=\delta_{ij}$, so the original basis is reciprocal to the primed basis. Uniqueness of a reciprocal basis gives

$$
\boxed{e''_i=e_i\qquad(i=1,2,3)}.
$$

Every vector $K$ has a unique expansion $K=\sum_i\kappa_ie'_i$, and then

$$
K\cdot R
=\sum_{i,j}\kappa_i n_j e'_i\cdot e_j
=\sum_i\kappa_i n_i.
$$

This is an integer for every integer triple $(n_1,n_2,n_3)$ exactly when every $\kappa_i$ is an integer. Hence all such points are

$$
\boxed{K=m_1e'_1+m_2e'_2+m_3e'_3,
\qquad m_1,m_2,m_3\in\mathbb Z}.
$$

They form the reciprocal lattice in the convention without a factor of $2\pi$.

## ↑ Ancestors (10)

1. [5C](../5c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
