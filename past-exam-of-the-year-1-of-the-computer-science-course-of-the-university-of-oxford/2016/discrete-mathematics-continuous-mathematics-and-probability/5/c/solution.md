<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply [separation of variables](../../../../../separation-of-variables.md) to each mode of the [damped wave equation](../../../../../damped-wave-equation.md) $u_{tt}+2k^2u_t=c^2u_{xx}$, assuming $L,c>0$. The spatial [ordinary differential equation](../../../../../ordinary-differential-equation.md) is $X_n''+(\lambda_n/c)^2X_n=0$. Its general solution is $C\sin(\lambda_n x/c)+D\cos(\lambda_n x/c)$. The boundary condition at $0$ gives $D=0$; a nonzero mode at $L$ requires

$$
\boxed{\lambda_n=\frac{n\pi c}L,\quad n=1,2,\ldots,\qquad X_n(x)=\sin\frac{n\pi x}L.}
$$

Only odd $n=2m+1$ occur in the initial [Fourier sine series](../../../../../fourier-sine-series.md). Put $\omega_m=(2m+1)\pi c/L$ and $d_m=\sqrt{k^4-\omega_m^2}$. The temporal equation $T_m''+2k^2T_m'+\omega_m^2T_m=0$ has roots $-k^2\pm d_m$. Define

$$
\boxed{\alpha_m=k^2-d_m,\qquad\beta_m=k^2+d_m.}
$$

For distinct roots, let the full amplitude be $q_m(t)=A_me^{-\alpha_mt}+B_me^{-\beta_mt}$. The initial displacement and zero initial velocity impose $A_m+B_m=F_m$ and $\alpha_mA_m+\beta_mB_m=0$. Solving gives

$$
\boxed{A_m=\frac{\beta_mF_m}{\beta_m-\alpha_m},\qquad
B_m=-\frac{\alpha_mF_m}{\beta_m-\alpha_m}.}
$$

Thus the physically consistent superposition is

$$
\boxed{u(x,t)=\sum_{m=0}^\infty q_m(t)\sin\frac{(2m+1)\pi x}L.}
$$

For $\omega_m<k^2$ there is [overdamping](../../../../../overdamping.md), with two real decaying exponentials. For $\omega_m>k^2$ there is [underdamping](../../../../../underdamping.md); set $\nu_m=\sqrt{\omega_m^2-k^4}$; the equivalent real expression is

$$
q_m(t)=F_me^{-k^2t}\left(\cos(\nu_mt)+\frac{k^2}{\nu_m}\sin(\nu_mt)\right).
$$

At [critical damping](../../../../../critical-damping.md), the repeated-root case $\omega_m=k^2$, take the limit, giving $q_m(t)=F_m(1+k^2t)e^{-k^2t}$. These formulas all satisfy $q_m(0)=F_m$ and $q_m'(0)=0$.

Three source qualifications matter. First, the sum must start at $m=0$, for the same reason as in (b). Second, the printed $X(x)=u_0(x)$ cannot hold for a single separated mode: the tent has $X''=0$ on each open linear segment but $X\ne0$, contradicting $X''=-(\lambda_n/c)^2X$ for positive $\lambda_n$, and its peak is not twice differentiable. Separation applies mode by mode, with the initial tent recovered by superposition. Third, no finite “large” $k$ makes every mode overdamped, because $\omega_m\to\infty$. The two-exponential expression permits complex conjugate roots, while a repeated root requires its displayed limiting form. The tent initial data are naturally interpreted through the convergent modal solution, rather than as a single smooth separated product.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
