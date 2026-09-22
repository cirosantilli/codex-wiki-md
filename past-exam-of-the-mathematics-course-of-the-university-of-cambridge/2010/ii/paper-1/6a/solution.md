<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

The positive [steady state](../../../../../steady-state.md) satisfies $1+b(N^*)^2=r$, so

$$
\boxed{N^*=\sqrt{(r-1)/b}.}
$$

With $N_t=N^*+\eta_t$, the [linearization](../../../../../linearization.md) is

$$
\eta_{t+1}=\eta_t-\frac{2(r-1)}r\eta_{t-1}.
$$

Its [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\lambda^2-\lambda+d$, where $d=2(r-1)/r$. The roots are inside the unit disk precisely when $0<d<1$: when they are real they are positive with sum one, and when complex conjugate their common modulus is $\sqrt d$. Therefore the [fixed point](../../../../../fixed-point.md) is **linearly asymptotically stable for $1<r<2$ and unstable for $r>2$**. At $r=2$,

$$
\boxed{\lambda_\pm=e^{\pm i\pi/3},\qquad\eta_{t+6}=\eta_t.}
$$

This proves period six for the neutral linearized oscillations. The stronger printed claim of a nonlinear period-six branch is not valid for the stated recurrence. It is important to distinguish these two assertions.

Here is a local obstruction, which also checks that the qualification is not merely absence of a proof. Normalize by the moving [fixed point](../../../../../fixed-point.md), let $x=N_{t-1}/N^*(r)-1$, $y=N_t/N^*(r)-1$, and define

$$
F_r(x,y)=\left(y,\frac{r(1+y)}{1+(r-1)(1+x)^2}-1\right).
$$

Put $v=(x,y)^T$, $\delta=r-2$, and $Q=x^2-xy+y^2>0$ for $v\ne0$. The quadratic and cubic terms of $F_2$'s second component are $x^2/2-xy+x^2y/2$. Composing six times gives

$$
F_r^6(v)-v=\delta Bv+QD v+
O\bigl(|v|^4+|\delta||v|^2+\delta^2|v|\bigr),
\quad
B=\begin{pmatrix}1&1\\-1&2\end{pmatrix},\quad
D=\begin{pmatrix}-1/2&-1\\1&-3/2\end{pmatrix}.
$$

In particular the quadratic terms cancel, while the cubic components are $-(x+2y)Q/2$ and $(2x-3y)Q/2$. If a small nonzero $v$ were a period-six point, invertibility of $B$ and the norm of this equation would imply $|\delta|=O(|v|^2)$. Taking its [determinant](../../../../../determinant.md) with $Bv$ then gives

$$
0=\det(Bv,QDv)+O(|v|^5)=\frac{Q^2}{2}+O(|v|^5).
$$

Since $Q\geq|v|^2/2$, this is impossible for sufficiently small nonzero $v$. Thus **no nontrivial nonlinear six-cycle bifurcates locally at $r=2$**. At the threshold the same expansion gives $Q(F_2^6(v))=Q(v)-2Q(v)^2+O(|v|^5)$, so the [fixed point](../../../../../fixed-point.md) is actually locally asymptotically stable nonlinearly, with slow decay. The valid intended linear-stability conclusion is the period-six neutral oscillation above; a literal nonlinear assertion requires a changed model or wording. This is an example of the [distinction between linear resonance and nonlinear periodic bifurcation](../../../../../distinction-between-linear-resonance-and-nonlinear-periodic-bifurcation.md).

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
