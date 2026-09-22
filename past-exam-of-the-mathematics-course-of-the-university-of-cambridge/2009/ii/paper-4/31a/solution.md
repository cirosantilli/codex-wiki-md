<h1 id="31a/solution">Solution</h1>

↑ **Parent:** [31A](../31a.md)

The lowest [Liouville–Green approximation](../../../../../wkb-approximation.md) comes from $f=e^S$, for which $S''+(S')^2=Q$. First take $S'=\pm\sqrt Q$; the next transport term is $-Q'/(4Q)$. Integrating gives

$$
\boxed{f_\pm(x)=Q(x)^{-1/4}\exp\left(\pm\int^x\sqrt{Q(t)}\,dt\right).}
$$

Multiplicative constants and the lower limit are arbitrary. The negative sign selects the recessive approximation in the usual [WKB approximation](../../../../../wkb-approximation.md) regime, where the exponent dominates the amplitude and the derivative corrections are small. Positivity of $Q$ by itself does not prove that $f_-$ tends to zero or that the approximation is valid: for example $Q=e^{-x}$ makes this expression grow like $e^{x/4}$ with a bounded integral in its exponent. For $Q=x$, all the required large-$x$ conditions hold and $f_-=x^{-1/4}e^{-2x^{3/2}/3}\to0$.

Put $a=f_-$. Direct differentiation gives

$$
\frac{a'}a=-\sqrt x-\frac1{4x},\qquad\frac{a''}a=x+\frac5{16x^2}.
$$

Substituting $\operatorname{Ai}=wa$ into the [Airy ordinary differential equation](../../../../../airy-ordinary-differential-equation.md) $\operatorname{Ai}''=x\operatorname{Ai}$ and dividing by $a$ gives $w''+2(a'/a)w'+5w/(16x^2)=0$. Multiplication by $x^2$ proves

$$
\boxed{x^2w''-\left(2x^{5/2}+\frac x2\right)w'+\frac5{16}w=0.}
$$

The recessive branch has a constant leading amplitude $c$. To find its first correction write $w=c(1+b x^{-\delta}+\cdots)$. Balancing $-2x^{5/2}w'$ against the constant term $5c/16$ forces $3/2-\delta=0$, so $\delta=3/2$. The constant coefficients then give $3b+5/16=0$. The remaining terms are of order $x^{-3/2}$ and are cancelled by a next term of order $x^{-3}$. Thus

$$
\boxed{w(x)\sim c\left(1-\frac5{48}x^{-3/2}+\cdots\right).}
$$

The multiplicative constant depends on the chosen normalization of the [Airy function](../../../../../airy-function.md) and of $f_-$. The calculation selects the recessive solution; a growing Airy solution would not have this constant-amplitude expansion.

## ↑ Ancestors (10)

1. [31A](../31a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
