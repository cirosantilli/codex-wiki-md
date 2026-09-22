# Implicit midpoint Lipschitz estimate

↑ **Parent:** [Implicit midpoint rule](implicit-midpoint-rule.md)

For a uniformly [Lipschitz continuous](lipschitz-continuity.md) state field $f$ with constant $L$, an [implicit midpoint rule](implicit-midpoint-rule.md) step is uniquely solvable when $hL/2<1$, by the [contraction mapping theorem](contraction-mapping-theorem.md). Write its step map as $\Psi_h(u)=u+h\Phi_h(u)$, where $\Phi_h(u)=f(t+h/2,u+h\Phi_h(u)/2)$. Subtracting the increment equations gives

$$
(1-hL/2)\|\Phi_h(u)-\Phi_h(v)\|\leq L\|u-v\|.
$$

Therefore $\operatorname{Lip}(\Phi_h)\leq L/(1-hL/2)$, and the [triangle inequality](triangle-inequality.md) gives the bound for $\Psi_h$. Combining it with the [implicit midpoint consistency bound](implicit-midpoint-consistency-bound.md) yields

$$
\|e_n\|\leq R_h^n\|e_0\|+\frac{Kh^2}{L}(R_h^n-1),
\qquad R_h=\frac{1+hL/2}{1-hL/2}
$$

for $L>0$. This follows by summing the geometric error recurrence with forcing $Kh^3/(1-hL/2)$. For $hL\leq1$ and $nh\leq T$, $R_h^n\leq e^{2LT}$, proving second-order [global error](global-discretization-error.md) with exact starting data. If $L=0$, the direct bound is $\|e_n\|\leq\|e_0\|+KTh^2$.

## ↑ Ancestors (9)

1. [Implicit midpoint rule](implicit-midpoint-rule.md)
2. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
3. [Runge-Kutta method](runge-kutta-method-split.md)
4. [One-step method](one-step-method.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-analysis-course-of-the-university-of-oxford/2023/3/c/solution.md)
