<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The [eddy viscosity](../../../../../../eddy-viscosity.md) in the prescribed [mixing length](../../../../../../mixing-length.md) model is

$$
\boxed{\nu_T=l^2|U_y|=C_1^2M_0^{1/2}x^{1/2}\eta^2|f''(\eta)|.}
$$

Thus at a fixed similarity coordinate $\eta$, every nonzero value grows as $x^{1/2}$. Its maximum occurs at a fixed coordinate maximizing $\eta^2|f''|$, so the maximum itself has the same downstream scaling.

The formal argument intended by the edge assumption is also clear. If one independently stipulates $|f''(\eta)|\leq|f''(\eta_w)|$ for $|\eta|\leq\eta_w$, then $\eta^2|f''(\eta)|\leq\eta_w^2|f''(\eta_w)|$. This would put the maximum [eddy viscosity](../../../../../../eddy-viscosity.md) at the edge and give

$$
\frac{U(x,0)y_w}{\nu_T(x,y_w)}=\frac{f'(0)}{C_1^2\eta_w|f''(\eta_w)|},
$$

independent of $x$, provided $f''(\eta_w)\ne0$. That is a conditional scaling calculation, not an admissible solution of the full momentum problem.

The printed edge claim fails for the reason established in part (e): $f'(\eta_w)=0$ forces $f''(\eta_w)=0$, and therefore

$$
\boxed{\nu_T(x,\pm y_w)=0.}
$$

A nontrivial profile has positive [eddy viscosity](../../../../../../eddy-viscosity.md) in the interior; hence its maximum cannot occur at that finite free edge. Moreover $U(x,0)y_w/\nu_T(x,\pm y_w)$ has a zero denominator, so it is **not a finite effective Reynolds number** under the literal assumptions.

The intended downstream cancellation is valid if one uses a consistent interior reference point $\eta_*\in(0,\eta_w)$ with $f''(\eta_*)\ne0$, for example the maximum of $\nu_T$. Since $U(x,0)=M_0^{1/2}x^{-1/2}f'(0)$ and $y_w=\eta_wx$,

$$
\boxed{\frac{U(x,0)y_w}{\nu_T(x,\eta_*x)}
=\frac{f'(0)\eta_w}{C_1^2\eta_*^2|f''(\eta_*)|},}
$$

which is independent of $x$. This is a qualified correction of the reference point, not a proof of the false edge maximum.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
