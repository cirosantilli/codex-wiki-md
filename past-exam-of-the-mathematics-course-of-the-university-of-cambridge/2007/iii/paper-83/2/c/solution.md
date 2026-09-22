<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $c_0=\sqrt{g'h_0/2}$, as printed in the PDF. The converted TeX misrenders this expression. The undisturbed reservoir has $u=0$, $c=c_0$. The expansion fan moving into it is a simple wave with $R_+=u+4c=4c_0$ constant. On the other characteristic family, a self-similar fan satisfies

$$
\xi=\frac xt=u-c.
$$

Solving these two equations gives

$$
\boxed{c(\xi)=\frac{4c_0-\xi}{5},\qquad
u(\xi)=\frac45(c_0+\xi),\qquad
h(\xi)=\frac2{g'}\left(\frac{4c_0-\xi}{5}\right)^2.}
$$

The fan begins at $\xi=-c_0$, where it matches the initially resting reservoir.

At the front, write $k_F=\sqrt2F$. The nose closure is $u_f=k_Fc_f$ and the invariant gives $u_f+4c_f=4c_0$. Therefore

$$
\boxed{c_f=\frac{4c_0}{4+k_F},\qquad
u_f=\frac{4k_Fc_0}{4+k_F},\qquad
h_f=\frac{16h_0}{(4+k_F)^2}.}
$$

A uniform region of this state connects the right edge of the fan, $\xi_n=u_f-c_f$, to the advancing front $x_f=u_ft$. Its width is $c_ft>0$. The complete lower-layer solution for $t>0$ is

$$
\boxed{u(x,t)=\begin{cases}
0,&\xi\leq-c_0,\\
\frac45(c_0+\xi),&-c_0\leq\xi\leq\xi_n,\\
u_f,&\xi_n\leq\xi<u_f,
\end{cases}}
$$

and

$$
\boxed{h(x,t)=\begin{cases}
h_0,&\xi\leq-c_0,\\
\frac2{g'}\left(\frac{4c_0-\xi}{5}\right)^2,&-c_0\leq\xi\leq\xi_n,\\
h_f,&\xi_n\leq\xi<u_f,\\
0,&\xi>u_f.
\end{cases}}
$$

Ahead of the front there is no lower-layer current, so its [velocity](../../../../../../velocity.md) is not a physical variable there. Both transitions inside the current are continuous; the finite-height nose is closed by the ambient-front condition, not by an unsupported vacuum jump. These formulas give the [front-regularized triangular-channel dam break](../../../../../../front-regularized-triangular-channel-dam-break.md) for any specified positive constant $F$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
