<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The physical [state space](../../../../../state-space.md) is the [positively invariant set](../../../../../positively-invariant-set.md) $X,Y,Z\geq0$, $X+Y+Z=N$: adding the equations gives zero, and the vector field points inward at each coordinate boundary. At an [equilibrium point](../../../../../equilibrium-point-of-a-dynamical-system.md), either $Y=0$, giving $(X,Y,Z)=(N,0,0)$, or $\beta X=b+r$. Therefore

$$
\boxed{N_c=\frac{b+r}{\beta},\qquad X_s=N_c,\quad Y_s=\frac{b(N-N_c)}{b+r},\quad Z_s=\frac{r(N-N_c)}{b+r}.}
$$

A positive endemic equilibrium exists exactly when $N>N_c$.

For $N<N_c$, put $d=b+r-\beta N>0$. Since $X\leq N$,

$$
\dot Y\leq-dY,\quad 0\leq Y(t)\leq Y(0)e^{-dt},\qquad
Z(t)=Z(0)e^{-bt}+r\int_0^t e^{-b(t-s)}Y(s)\,ds\longrightarrow0.
$$

The last limit follows either by evaluating the exponential integral (with a $te^{-bt}$ term when $d=b$), or by splitting it into an early decaying part and a late part with uniformly small $Y$. Hence $X\to N$ for every physical initial condition. Although immune numbers need not decrease monotonically initially, both infected and immune numbers tend to zero.

At the endemic equilibrium, the [Jacobian matrix](../../../../../jacobian-matrix.md) of the $X,Y$ subsystem is

$$
J=\begin{pmatrix}-b-\beta Y_s&-\beta X_s\\ \beta Y_s&0\end{pmatrix}.
$$

A disturbance proportional to $e^{pt}$ therefore obeys

$$
\boxed{p^2+(b+\beta Y_s)p+\beta^2X_sY_s=0.}
$$

Both coefficients are positive. Real roots have negative sum and positive product; complex conjugate roots have real part $-(b+\beta Y_s)/2<0$. Thus the endemic equilibrium is [asymptotically stable](../../../../../asymptotic-stability.md) by [linear stability analysis](../../../../../linear-stability.md).

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
