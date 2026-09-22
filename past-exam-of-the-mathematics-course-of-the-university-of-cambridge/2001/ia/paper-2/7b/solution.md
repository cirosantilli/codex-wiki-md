<h1 id="7b/solution">Solution</h1>

↑ **Parent:** [7B](../7b.md)

Write $A=aI+B$, where $B=\bigl(\begin{smallmatrix}1&-2\\1&-1\end{smallmatrix}\bigr)$ has $B^2=-I$. One eigenpair is

$$
\boxed{\ell=a+i,\qquad e=\begin{pmatrix}1+i\\1\end{pmatrix}.}
$$

Because $A$ is real, conjugating $Ae=\ell e$ gives $A\bar e=\bar\ell\bar e$. The [eigenvector](../../../../../eigenvector.md) matrix $(e,\bar e)$ has [determinant](../../../../../determinant.md) $2i\ne0$, so the [eigenvectors](../../../../../eigenvector.md) form a [basis](../../../../../basis.md). Reality of $z$ then forces conjugate coefficients, giving $z=\alpha e+\bar\alpha\bar e$.

Set $c=(1-i)/2$. The forcing has the same basis decomposition,

$$
h(t)=c e^{-it}e+\bar c e^{it}\bar e.
$$

Equating the coefficient of $e$ in the [linear system of differential equations](../../../../../linear-system-of-differential-equations.md) yields

$$
\boxed{\dot\alpha+(a+i)\alpha=c e^{-it}.}
$$

For $a>0$, an [integrating factor](../../../../../integrating-factor.md) gives $\alpha=(c/a)e^{-it}+C e^{-(a+i)t}$. The zero initial vector means $\alpha(0)=0$, so

$$
\alpha(t)=\frac c a(1-e^{-at})e^{-it}.
$$

Taking the real vector combination gives

$$
\boxed{z(t)=\frac{1-e^{-at}}a
\begin{pmatrix}2\cos t\\\cos t-\sin t\end{pmatrix},\qquad a>0.}
$$

Exact secular [resonance](../../../../../resonance.md) occurs at $a=0$: the forcing frequency matches the undamped homogeneous mode. For positive $a$, damping prevents secular growth, and the late-time periodic amplitude is proportional to $1/a$. Thus there is a resonant small-damping limit, but no unbounded resonant response at fixed $a>0$.

Since $(1-e^{-at})/a\to t$ for each fixed $t$, the requested limit gives

$$
\boxed{z(t)=t\begin{pmatrix}2\cos t\\\cos t-\sin t\end{pmatrix}\quad(a=0).}
$$

Equivalently $\alpha=c t e^{-it}$ at zero damping; its linear prefactor displays the resonance explicitly.

## ↑ Ancestors (10)

1. [7B](../7b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
