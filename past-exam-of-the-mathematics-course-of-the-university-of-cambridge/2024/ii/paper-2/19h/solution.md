<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

The character of $(\rho,V)$ is

$$
\chi_V(g)=\operatorname{tr}\rho(g).
$$

The stated action is a representation because successive action by $(g_2,h_2)$ and $(g_1,h_1)$ gives

$$
\sigma(h_1h_2)\,\alpha\,\rho(g_2^{-1}g_1^{-1})
=\sigma(h_1h_2)\,\alpha\,\rho((g_1g_2)^{-1}).
$$

Identifying $\operatorname{Hom}_{\mathbb C}(V,W)$ with $V^*\otimes W$ gives the [character of a Hom representation](../../../../../character-of-a-hom-representation.md)

$$
\boxed{\chi_{\operatorname{Hom}(V,W)}(g,h)
=\chi_V(g^{-1})\chi_W(h)
=\overline{\chi_V(g)}\,\chi_W(h)}.
$$

Here the final equality follows after unitarizing the finite-group representation.

The permutation character of $\mathbb CG$ counts fixed points:

$$
\chi_{\mathbb CG}(g,h)
=\#\{x\in G:gxh^{-1}=x\}
=\#\{x:x^{-1}gx=h\}.
$$

Thus

$$
\chi_{\mathbb CG}(g,h)=
\begin{cases}
|C_G(g)|,&g\text{ and }h\text{ are conjugate},\\
0,&\text{otherwise}.
\end{cases}
$$

On the other hand, the character of  
$\bigoplus_i\operatorname{Hom}(V_i,V_i)$ is

$$
\sum_i\overline{\chi_i(g)}\chi_i(h).
$$

The column form of [character orthogonality](../../../../../character-orthogonality.md) says that this has exactly the same two values above. Complex representations of a finite [group](../../../../../group-split.md) are semisimple, and semisimple representations with the same character are isomorphic. Hence the [two-sided regular representation decomposition](../../../../../two-sided-regular-representation-decomposition.md) is

$$
\boxed{\mathbb CG\cong
\bigoplus_{i=1}^r\operatorname{Hom}_{\mathbb C}(V_i,V_i)}
$$

as a $G\times G$ representation.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
