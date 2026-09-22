<h1 id="b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [character of an algebra](../../../../character-of-an-algebra.md) is a nonzero [multiplicative](../../../../multiplicative-function.md) complex-[linear map](../../../../linear-map.md) $\chi:A\to\mathbb C$. A maximal proper ideal is a proper ideal contained in no larger proper ideal. For a character, $\chi(1)=1$ and $\chi(a)\in\sigma(a)$: otherwise $a-\chi(a)1$ would be invertible although its character value is zero. The spectral bound gives $|\chi(a)|\leq\|a\|$, so the character is continuous. It is onto, and its kernel is a closed [maximal ideal](../../../../maximal-ideal.md) because $A/\ker\chi\cong\mathbb C$.

Conversely let $M$ be maximal. Its closure is an ideal and remains proper: otherwise an element of $M$ would lie within distance one of the unit, hence would be invertible by the [Neumann series](../../../../neumann-series.md), forcing $1\in M$. Maximality then gives $\overline M=M$. The [Banach algebra](../../../../banach-algebra-split.md) $A/M$ is a field. For any $b$ in this quotient choose $\lambda\in\sigma(b)$, using nonemptiness of the complex spectrum. In a field only zero is noninvertible, so $b-\lambda1=0$. Hence every quotient element is a scalar multiple of the unit. The [quotient map](../../../../quotient-map.md) therefore determines a character $\chi_M$, uniquely normalized by $\chi_M(1)=1$. These constructions are inverse:

$$
\boxed{\Delta(A)\longleftrightarrow M(A),\qquad\chi\longmapsto\ker\chi.}
$$

For the convolution algebra, write $e_j$ for the sequence supported at $j$ with value one. Then $e_j e_k=e_{j+k}$, $e_0=1$, and $e_1e_{-1}=1$. If $z=\chi(e_1)$, continuity and $\|e_{\pm1}\|_1=1$ imply $|z|\leq1$ and $|z^{-1}|\leq1$. Thus $|z|=1$, so uniquely $z=e^{it}$ for $0\leq t<2\pi$, and $\chi(e_j)=e^{ijt}$ for every integer $j$. [Absolute convergence](../../../../absolute-convergence.md) in $\ell^1$ now gives

$$
\boxed{\chi_t(\alpha)=\sum_{j\in\mathbb Z}\alpha_je^{ijt}.}
$$

Conversely each displayed map is bounded, nonzero, and [multiplicative](../../../../multiplicative-function.md), since the absolutely convergent double sum can be rearranged along $k+l=j$. Thus these are all characters, and all maximal proper ideals are

$$
\boxed{M_t=\left\{\alpha\in\ell^1(\mathbb Z):\sum_j\alpha_je^{ijt}=0\right\},\qquad0\leq t<2\pi.}
$$

They are distinct because the character is uniquely recovered from its kernel and its value on the unit.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [B](../../b.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../split.md)
5. [Functional Analysis and Banach and C\*-Algebras course of the University of Oxford](../../../../functional-analysis-and-banach-and-c-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
