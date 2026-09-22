<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The complex [Special orthogonal Lie algebra](../../../../../../special-orthogonal-lie-algebra.md) $\mathfrak{so}_5$ consists of endomorphisms preserving a nondegenerate symmetric [bilinear form](../../../../../../bilinear-form.md) infinitesimally:

$$
\mathfrak{so}(V,B)=\{X:B(Xu,v)+B(u,Xv)=0\}.
$$

In an orthonormal basis this is $\{X\in M_5(\mathbb C):X^T+X=0\}$, with the [commutator](../../../../../../commutator.md) bracket and dimension $\binom52=10$. Its compact real form is obtained by taking real skew-symmetric matrices. For diagonal root calculations it is more convenient to use an isotropic basis $v_1,v_2,v_0,v_{-2},v_{-1}$ with $B(v_i,v_j)=\delta_{i,-j}$, including $B(v_0,v_0)=1$.

A [maximal torus](../../../../../../maximal-torus.md) of the complex [special orthogonal group](../../../../../../special-orthogonal-group.md) is

$$
T=\{\operatorname{diag}(t_1,t_2,1,t_2^{-1},t_1^{-1}):t_1,t_2\in\mathbb C^\times\}.
$$

Its Lie algebra is the [Cartan subalgebra](../../../../../../cartan-subalgebra.md)

$$
\mathfrak h=\{H(h_1,h_2)=\operatorname{diag}(h_1,h_2,0,-h_2,-h_1)\}.
$$

In the compact real form the corresponding torus consists of independent rotations in two orthogonal coordinate planes, fixing the remaining direction. Define $\varepsilon_i(H)=h_i$ for $i=1,2$, and $\varepsilon_{-i}=-\varepsilon_i$, $\varepsilon_0=0$.

Writing $E_{ij}$ for the matrix unit in the isotropic basis, $F_{ij}=E_{ij}-E_{-j,-i}$ lies in $\mathfrak{so}_5$ and satisfies

$$
[H,F_{ij}]=(\varepsilon_i-\varepsilon_j)(H)F_{ij}.
$$

Thus the nonzero [root spaces](../../../../../../root-space.md) are one-dimensional and the [root-space decomposition](../../../../../../root-space-decomposition.md) is

$$
\boxed{\mathfrak{so}_5=\mathfrak h\oplus\bigoplus_{\alpha\in R}\mathfrak g_\alpha,
\qquad R=\{\pm\varepsilon_1,\pm\varepsilon_2,\pm\varepsilon_1\pm\varepsilon_2\}.}
$$

Explicit generators for four positive root spaces are

$$
\begin{array}{c|c}
\alpha&X_\alpha\\\hline
\varepsilon_1-\varepsilon_2&E_{12}-E_{-2,-1}\\
\varepsilon_1+\varepsilon_2&E_{1,-2}-E_{2,-1}\\
\varepsilon_1&E_{10}-E_{0,-1}\\
\varepsilon_2&E_{20}-E_{0,-2}
\end{array}
$$

The transposes of these matrices generate the negative root spaces. Each transpose still satisfies the bilinear-form condition and reverses the displayed diagonal weight. These eight root vectors and the two independent Cartan matrices exhaust the dimension ten; a matrix commuting with every $H$ is diagonal and the form condition makes it lie in $\mathfrak h$. This also proves that the torus has maximal dimension.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
