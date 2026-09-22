<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The three [distinguished limits](../../../../../distinguished-limit.md) are the [outer expansion](../../../../../outer-expansion.md) at $x=O(1)$, an [intermediate asymptotic region](../../../../../intermediate-asymptotic-region.md) at $x=O(\epsilon)$, and an [inner expansion](../../../../../inner-expansion.md) at $x=O(\epsilon^2)$. The middle scale resolves the coefficient change from $x$ to $x+\epsilon$; the narrower scale resolves the unmet left [boundary condition](../../../../../boundary-condition.md). The original equation is understood on $x>0$ with a continuous extension to the boundary. As explained below, imposing a classical second [derivative](../../../../../derivative.md) at $x=0$ would be too strong for this [degenerate ordinary differential equation](../../../../../degenerate-ordinary-differential-equation.md).

In the [outer expansion](../../../../../outer-expansion.md), set $y=y_0+\epsilon y_1+\cdots$. The leading equation is $x(x+1)y_0'-xy_0=0$. Enforcing the right [boundary condition](../../../../../boundary-condition.md) gives $y_0=x+1$. Because $y_0''=0$, the next equation is particularly simple:

$$
x(x+1)y_1'-xy_1=-(x+1),\qquad y_1(1)=0.
$$

An [integrating factor](../../../../../integrating-factor.md), or the substitution $y_1=(x+1)u$, gives $u'=-1/[x(x+1)]$. Thus

$$
\boxed{y_{\rm out}(x)=(1+x)\left[1+\epsilon\log\frac{1+x}{2x}\right]+O(\epsilon^2),\qquad x=O(1).}
$$

The error statement is for $x$ bounded away from zero. The left limiting form is $1+x-\epsilon\log(2x)$ through the terms needed for matching. A [logarithm](../../../../../logarithm.md) in the correction makes a pure integer-power inner ansatz inadequate.

For the [intermediate asymptotic region](../../../../../intermediate-asymptotic-region.md), put $x=\epsilon s$ and $y=V(s)$. The transformed equation is

$$
\sqrt\epsilon\sqrt s(s+1)\frac{\sin[\epsilon(s+1)]}{\epsilon(s+1)}V''+(s+1)(1+\epsilon s)V'-\epsilon(s+\epsilon)V=0.
$$

The leading $V_0$ is a constant fixed to $1$ by matching. There is no order-$\sqrt\epsilon$ forcing, so that homogeneous constant is zero after matching. At order $\epsilon$, $(s+1)V_1'=s$, giving $V_1=s-\log(1+s)+C(\epsilon)$. Matching for $1\ll s\ll1/\epsilon$ with the [outer expansion](../../../../../outer-expansion.md) fixes $C=-\log(2\epsilon)$. Hence

$$
\boxed{y_{\rm mid}(\epsilon s)=1+\epsilon\left[s-\log(1+s)-\log(2\epsilon)\right]+o(\epsilon),\qquad s=O(1),\ s>0.}
$$

The [switchback term](../../../../../switchback-term.md) $-\epsilon\log\epsilon$ is larger than an ordinary $O(\epsilon)$ constant correction and must be retained. The highest [derivative](../../../../../derivative.md) term first changes this middle solution at order $\epsilon^{3/2}$, so it does not alter the displayed result.

To locate the [inner expansion](../../../../../inner-expansion.md), compare the [derivative](../../../../../derivative.md) terms for $x\ll\epsilon$. Their ratio at a layer width $\delta$ is $\epsilon/\sqrt\delta$, so the [square-root-degenerate endpoint layer](../../../../../square-root-degenerate-endpoint-layer.md) has $\delta=\epsilon^2$. Put $x=\epsilon^2X$ and $y=U(X)$. After dividing by the common leading factor, the equation through order $\epsilon$ is

$$
\sqrt X(1+\epsilon X)U''+(1+\epsilon X)U'+O(\epsilon^2)=0.
$$

Both orders therefore have the same homogeneous operator $\sqrt X\,d^2/dX^2+d/dX$. Its [derivative](../../../../../derivative.md) mode is proportional to $e^{-2\sqrt X}$. Using $U(0)=0$ and the supplied elementary [integral](../../../../../integral.md), define

$$
H(X)=2\int_0^X e^{-2\sqrt q}\,dq=1-(1+2\sqrt X)e^{-2\sqrt X}.
$$

The [intermediate asymptotic region](../../../../../intermediate-asymptotic-region.md) gives the overlap value $1-\epsilon\log(2\epsilon)$ as $s\to0$. Therefore

$$
\boxed{y_{\rm in}(\epsilon^2X)=\left[1-\epsilon\log(2\epsilon)\right]\left[1-(1+2\sqrt X)e^{-2\sqrt X}\right]+o(\epsilon),\qquad X=O(1).}
$$

It satisfies the left [boundary condition](../../../../../boundary-condition.md) exactly to the retained orders, and its large-$X$ limit matches the middle result in $1\ll X\ll1/\epsilon$. The outer and middle limits match with $\epsilon\ll x\ll1$. These three formulae include all terms through $O(\epsilon)$, including the logarithmic switchback; the omitted terms in the middle and inner regions need not be $O(\epsilon^2)$.

For a check on that last point, continue the middle equation by one order. Its $\epsilon^{3/2}$ term obeys

$$
V_{3/2}'=-\frac{\sqrt s}{(1+s)^2},\qquad
V_{3/2}(s)=\int_s^\infty\frac{\sqrt r}{(1+r)^2}\,dr=\frac\pi2-\arctan\sqrt s+\frac{\sqrt s}{1+s}.
$$

The integration constant is selected by the outer limit. Its value at $s=0$ is $\pi/2$, so the inner matching amplitude has a next correction $\pi\epsilon^{3/2}/2$. This independently explains why an $o(\epsilon)$ remainder is appropriate.

If a single [additive composite expansion](../../../../../additive-composite-expansion.md) is useful, combine the three formulae and subtract their two common overlaps. Writing $A=1-\epsilon\log(2\epsilon)$ and interpreting $x\log x=0$ at zero gives

$$
y_{\rm comp}=1+x+\epsilon\left[(1+x)\log\frac{1+x}{2}-x\log x-\log(x+\epsilon)\right]-A\left(1+\frac{2\sqrt x}{\epsilon}\right)e^{-2\sqrt x/\epsilon}.
$$

It is zero at $x=0$, gives $2+O(\epsilon^2)$ at $x=1$, and reproduces all three retained expansions. It does not assert an $O(\epsilon^2)$ error uniformly through the nested regions.

Finally, near zero $H(X)=2X-\tfrac83X^{3/2}+O(X^2)$. Thus the solution has a finite nonzero first [derivative](../../../../../derivative.md) but generally a second [derivative](../../../../../derivative.md) diverging like $x^{-1/2}$. This is compatible with the equation for $x>0$: the vanishing coefficient of $y''$ multiplies that singular [derivative](../../../../../derivative.md) to give a finite limit. If one instead required $y\in C^2[0,1]$ and the differential equation pointwise at $0$, the left condition would force $y'(0)=0$. The normalized equation's other coefficients have only integrable $x^{-1/2}$ singularities, so uniqueness for the [initial value problem](../../../../../initial-value-problem.md) with $y(0)=y'(0)=0$ would give the zero solution, contradicting the right condition. Explicitly, write the normalized equation as a first-order system for $(y,y')$ with an integrable coefficient matrix; its integral equation and the [Gronwall inequality](../../../../../gronwall-inequality.md) force a solution with zero initial vector to vanish. The continuous-endpoint interpretation is therefore essential.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 336](../../paper-336-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
