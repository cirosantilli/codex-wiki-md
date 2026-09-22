<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $X=\sum_s a_s^\dagger b_s$ and $Y=X^\dagger$, and take real hopping amplitude $t$ and real $\mathcal E$. Write the [anti-Hermitian](../../../../../skew-hermitian-matrix.md) ansatz with its ordering visible:

$$
S=f(\Delta)X-Yf(\Delta).
$$

Using $Yf(\Delta)=f(\Delta+2)Y$, its [commutator](../../../../../commutator.md) with $\mathcal E$ is

$$
[S,\mathcal E]
=f(\Delta)[\mathcal E(\Delta-2)-\mathcal E(\Delta)]X
-f(\Delta+2)[\mathcal E(\Delta+2)-\mathcal E(\Delta)]Y.
$$

Both terms equal their required hopping coefficients $-t$ if

$$
\boxed{f(\Delta)=\frac{t}{\mathcal E(\Delta)-\mathcal E(\Delta-2)}.}
$$

The shifted expression is then $f(\Delta+2)=t/[\mathcal E(\Delta+2)-\mathcal E(\Delta)]$. For a transition from difference $d$ to $d+2$, the left-ordered factor evaluates as $f(d+2)=t/[\mathcal E(d+2)-\mathcal E(d)]$, the final-minus-initial energy denominator.

The formula describes [occupation-dependent virtual hopping](../../../../../occupation-dependent-virtual-hopping.md) on actual transitions with nonzero energy gaps. [Perturbation theory](../../../../../perturbation-theory.md) also requires the hopping [matrix](../../../../../matrix.md) element, including its bosonic occupation factors, to be small compared with that gap. The [resonance obstruction to perturbative elimination](../../../../../resonance-obstruction-to-perturbative-elimination.md) at a zero denominator on a nonzero hop requires [degenerate perturbation theory](../../../../../degenerate-perturbation-theory.md). Values on unreachable states whose hopping amplitude vanishes need not determine the generator.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
