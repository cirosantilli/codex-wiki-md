<h1 id="39a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $K_N=\{k\in\mathbb Z^2:|k_1|,|k_2|\le N\}$, use $u_N=\sum_{k\in K_N}u_ke^{i\pi k\cdot x}$ and impose $u_0=0$. The coefficient has $a_0=3$ and $a_{\pm e_1}=a_{\pm e_2}=1/2$, with all other coefficients zero. Fourier differentiation and convolution give

$$
[\nabla\cdot(a\nabla u_N)]_k=-\pi^2\sum_{\ell\in K_N}(k\cdot\ell)a_{k-\ell}u_\ell.
$$

Consequently the explicit Galerkin system for each $k\in K_N\setminus\{0\}$ is

$$
\boxed{-3\pi^2|k|^2u_k-\frac{\pi^2}{2}\sum_{e\in\{\pm e_1,\pm e_2\}}k\cdot(k-e)\,u_{k-e}=f_k,}
$$

where coefficients outside $K_N$ and $u_0$ are zero. The forcing is $f_{e_1}=f_{e_2}=1/(2i)$, $f_{-e_1}=f_{-e_2}=-1/(2i)$ and zero elsewhere. The $k=0$ equation is $0=0$ and is replaced by normalization. For a real solution $u_{-k}=\overline{u_k}$, so the system can equivalently be written in real sine/cosine coordinates.

Since $a\ge1$, the negative of this operator has [quadratic form](../../../../../../quadratic-form.md) $\int a|\nabla u_N|^2$, strictly positive on nonzero zero-mean trigonometric polynomials. Thus the finite [linear system](../../../../../../system-of-linear-equations.md) is invertible. This construction multiplies the coefficient and derivative before projecting; it retains the explicit nearest-neighbour mode coupling rather than dividing the forcing by $a$ pointwise.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [39A](../../39a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
