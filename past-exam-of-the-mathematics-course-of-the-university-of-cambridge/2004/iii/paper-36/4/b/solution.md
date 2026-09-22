<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the first endowment as $(a,t)$. The [budget constraint](../../../../../../budget-constraint.md) at normalized prices is $px+y\leq pa+t$. Because the [quasilinear utility](../../../../../../quasilinear-utility.md) is increasing in $y$, the budget binds, and its maximization reduces to maximizing $\log x-px+pa+t$ over $x>0$. Its derivative is $1/x-p$ and its second derivative is $-1/x^2<0$, giving the unique [demand correspondence](../../../../../../demand-correspondence.md)

$$
x_1(p,t)=\frac1p,\qquad y_1(p,t)=pa+t-1.
$$

The first-good demand has no wealth effect. Since the second consumer's endowment and [preference relation](../../../../../../preference-relation.md) are fixed, $Z_t=0$ everywhere. Thus the joint condition of part (a) becomes $Z_p\ne0$ at equilibrium; **it is not automatically satisfied**.

Here is a complete smooth counterexample, with the second consumer's consumption set specified explicitly. The question does not impose the first consumer's consumption set on the second consumer. Take endowments $(a,t)=(1/10,t)$ and $(b,c)=(2,1)$. Give the second consumer consumption set $X_2=(-\infty,A)\times\mathbb R$, where $A=43/20$, and put $B=31/20$. Its [utility function](../../../../../../utility-function-split.md) is

$$
U_2(x,y)=\begin{cases}\displaystyle\exp\!\left(-\frac{(A-x+y-B)^2}{4(y-B)}\right),&y>B,\\[1ex]0,&y\leq B.\end{cases}
$$

This defines complete, transitive, continuous [preference relations](../../../../../../preference-relation.md). It is in fact smooth on $X_2$: writing $r=A-x>0$ and $s=y-B>0$, the positive branch is $\exp(-r^2/(4s)-r/2-s/4)$; at $s=0$ all derivatives tend to zero locally uniformly where $r>0$. The endowment belongs to $X_2$. Allowing negative holdings is explicit here, just as the first consumer's second coordinate is unrestricted in the printed question.

We now derive, rather than posit, the second consumer's [demand correspondence](../../../../../../demand-correspondence.md). For $v>0$, the upper contour $U_2\geq e^{-v}$ is described by $(r+s)^2\leq4vs$, with $r,s>0$. At a fixed $s$, its cheapest first coordinate uses $r=2\sqrt{vs}-s$. Minimizing total expenditure over $s$ therefore means minimizing

$$
pA+B+(1+p)s-2p\sqrt{vs}.
$$

The unique minimum occurs at $\sqrt{s}=p\sqrt v/(1+p)$, with $r=vp(p+2)/(1+p)^2>0$. The expenditure necessary to reach this contour is consequently

$$
e(p,v)=pA+B-\frac{vp^2}{1+p}.
$$

Set $\delta=A-b=3/20$ and $\varepsilon=B-c=11/20$. Wealth is $pb+c$, so the best affordable contour has

$$
v_*=(\delta p+\varepsilon)\frac{1+p}{p^2}>0.
$$

All affordable positive-utility bundles have $v\geq v_*$, and the minimum-expenditure bundle on that contour is unique and spends precisely the budget. Zero-utility bundles cannot be optimal because this positive-utility bundle is available. Substitution yields globally smooth unique demands for every $p>0$:

$$
x_2(p)=A-\frac{(\delta p+\varepsilon)(p+2)}{p(p+1)},\qquad y_2(p)=B+\frac{\delta p+\varepsilon}{p+1}.
$$

The [aggregate excess demand](../../../../../../aggregate-excess-demand.md) is now

$$
\boxed{Z(p,t)=\frac1p+x_2(p)-(a+b)=-\frac{(p-1)^2}{10p(p+1)}.}
$$

For every $t>0$, the unique equilibrium price is $p=1$, and $Z_p(1,t)=Z_t(1,t)=0$. At this price the allocations are $(1,t-9/10)$ and $(11/10,19/10)$, whose sum equals the aggregate endowment $(21/10,t+1)$. Second-good excess demand is $-pZ$, so it too is smooth and clears. Hence **every economy in this smooth parameterized family is singular**. This demonstrates why the first consumer's missing wealth effect alone gives no transversality guarantee; the stronger conclusion in part (c) comes from the second consumer's additional demand restriction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
