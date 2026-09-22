<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

Divide the differential equation by $\sqrt{1-x^2}$. Its [Sturm-Liouville form](../../../../../sturm-liouville-form.md) is

$$
\boxed{\frac d{dx}\left(\sqrt{1-x^2}\,y'\right)
+\frac{n^2}{\sqrt{1-x^2}}y=0.}
$$

Here $p(x)=\sqrt{1-x^2}$ and weight $w(x)=(1-x^2)^{-1/2}$. Multiply the equations for $T_n,T_m$ by the other polynomial and subtract. [Integration by parts](../../../../../integration-by-parts.md) gives a boundary term $p(T_mT_n'-T_nT_m')$, which vanishes at both endpoints because polynomial derivatives are finite and $p\to0$. Hence

$$
(n^2-m^2)\int_{-1}^1\frac{T_nT_m}{\sqrt{1-x^2}}dx=0.
$$

With the standard nonnegative degree indices $n,m$, this proves **orthogonality for $n\ne m$**. If signed integer indices are used literally, the condition is $|n|\ne|m|$: $T_{-n}=T_n$, so merely $n\ne m$ would not suffice.

Set $x=\cos\theta$ and $Y(\theta)=y(\cos\theta)$. The chain rule gives $(1-x^2)y''-xy'=Y''$, so $Y''+n^2Y=0$. For $n>0$, $Y=A\cos(n\theta)+B\sin(n\theta)$. A polynomial $y$ has $Y'(0)=0$, forcing $B=0$. At $n=0$, $Y=A+B\theta$ and the same endpoint condition gives $B=0$. Therefore every polynomial solution is proportional to

$$
\boxed{T_n(x)=\cos(n\arccos x).}
$$

The cosine recurrence yields $T_{n+1}=2xT_n-T_{n-1}$, $T_0=1,T_1=x$, confirming that these functions are polynomials. In this normalization the [Chebyshev polynomial](../../../../../chebyshev-polynomial.md) weight identity is

$$
\int_{-1}^1\frac{T_nT_m}{\sqrt{1-x^2}}dx=
\begin{cases}0,&n\ne m,\\\pi,&n=m=0,\\\pi/2,&n=m>0.\end{cases}
$$

It is simply cosine orthogonality after $x=\cos\theta$.

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
