<h1 id="a/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $\operatorname{Re}s>1$, logarithmic differentiation of the [absolutely convergent](../../../../absolute-convergence.md) [Euler product](../../../../euler-product.md) gives $-\zeta'(s)/\zeta(s)=\sum_{n\ge1}\Lambda(n)n^{-s}$, where $\Lambda(p^k)=\log p$ and it is zero otherwise. On the line $\operatorname{Re}s=c>1$, this series is absolutely bounded by $\sum_n(\log n)n^{-c}<\infty$, and $1/[s(s+1)]$ is integrable in the vertical variable. Hence [absolute convergence](../../../../absolute-convergence.md) justifies interchanging sum and [contour integral](../../../../contour-integral.md). The given first Mellin kernel, with $y=x/n$, contributes $x(1-n/x)=x-n$ if $n\le x$ and zero otherwise. Thus

$$
\boxed{\psi_1(x)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}-\frac{\zeta'(s)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds.}
$$

Splitting off $1/(s-1)$ gives the desired decomposition with $f$ for $x\ge1$. There is a range misprint in the second supplied kernel: for $0<y<1$ its integral is zero, not $(y-1)^2/2$. The globally correct value is $(y-1)_+^2/2$. For $y\ge1$ it is exactly the expression used here, so the subsequent large-$x$ argument is unchanged.

Near one, write $h=s-1$ and $\zeta(s)=h^{-1}+\gamma+O(h)$. Then $-\zeta'/\zeta=h^{-1}-\gamma+O(h)$, so subtraction cancels the [pole](../../../../pole.md) and $f$ has the removable value $\boxed{f(1)=-\gamma/2}$.

For a continuously differentiable $F$ with the given decay, both $F$ and $F'$ are integrable and $F(t)\to0$ at either end. [Integration by parts](../../../../integration-by-parts.md) on finite intervals and passage to the limit gives, for $x>1$,

$$
\int_{-\infty}^\infty F(t)x^{it}\,dt=-\frac1{i\log x}\int_{-\infty}^\infty F'(t)x^{it}\,dt.
$$

Its absolute value is at most $\|F'\|_1/\log x$, proving the estimate.

We also need uniform control of $f(c+it)$ on bounded $t$ as $c\downarrow1$. Here is the [three-four-one zero-free-region argument](../../../../three-four-one-zero-free-region-argument.md) supplying it. For $\sigma>1$, the [Euler product](../../../../euler-product.md) and $3+4\cos u+\cos2u=2(1+\cos u)^2\ge0$ imply

$$
\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1.
$$

If $\zeta(1+it)$ vanished for a nonzero real $t$, holomorphy from (3) would make the left side $O((\sigma-1)^{-3+4})\to0$, since $\zeta(\sigma+2it)$ remains bounded, a contradiction. Thus there are no zeros on that line, and there are none to its right by the [Euler product](../../../../euler-product.md). After removal of the singularity at one, $f$ and $f'$ are bounded on the compact rectangle $1\le\operatorname{Re}s\le2$, $|\operatorname{Im}s|\le3$.

For $|t|\ge3$, put $H=-\zeta'/\zeta-1/(s-1)$. The supplied estimates give $H=O((\log|t|)^9)$ and

$$
H'=-\frac{\zeta''}{\zeta}+\left(\frac{\zeta'}{\zeta}\right)^2+\frac1{(s-1)^2}=O((\log|t|)^{18}),
$$

uniformly in $1<c<2$. Since $f=H/[s(s+1)]$, it follows that $f=O(t^{-2}(\log|t|)^9)$ and $f'=O(t^{-2}(\log|t|)^{18})$, both $O(|t|^{-3/2})$. Also $d f(c+it)/dt=if'(c+it)$. Together with the compact bound this proves both required decay bounds with constants independent of $c$.

Parametrizing the contour, the remainder in the decomposition is $x^{c+1}/(2\pi)$ times the [oscillatory integral](../../../../oscillatory-integral.md) just bounded. Choose $c=1+1/\log x$ for $x>e$, so $x^{c+1}=ex^2$. Hence the remainder is $O(x^2/\log x)$. Finally $(x-1)^2/2=x^2/2+O(x)$, and $O(x)$ is absorbed, proving

$$
\boxed{\psi_1(x)=\frac{x^2}2+O\left(\frac{x^2}{\log x}\right).}
$$

## ↑ Ancestors (12)

1. [4](../4.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../split.md)
5. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
