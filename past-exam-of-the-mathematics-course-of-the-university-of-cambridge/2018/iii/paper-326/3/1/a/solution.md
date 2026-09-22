<h1 id="3/1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

First interpret the stated well-definedness as including uniqueness of the [global minimizer](../../../../../../../global-minimizer.md) for each positive parameter. Under that assumption, the [parameter continuity of variational regularization](../../../../../../../parameter-continuity-of-variational-regularization.md) follows from the [direct method in the calculus of variations](../../../../../../../direct-method-in-the-calculus-of-variations.md) argument below.

Let $M=D(0)=\|f\|^2/2$. For large $n$, $\alpha_n\geq\beta:=\alpha/2$. Comparison with zero, using $J(0)=0$, gives

$$
\Phi_{\beta,f}(u_{\alpha_n})\leq\Phi_{\alpha_n,f}(u_{\alpha_n})\leq M,
\qquad J(u_{\alpha_n})\leq M/\beta.
$$

[Coercivity](../../../../../../../coercive-function.md) of $\Phi_{\beta,f}$ therefore bounds the sequence. Take a $\tau$-[convergent subsequence](../../../../../../../convergent-subsequence.md) with limit $\bar u$. For any $v\in\operatorname{dom}J$, optimality gives

$$
\Phi_{\alpha,f}(u_{\alpha_n})
\leq\Phi_{\alpha,f}(v)
+(\alpha_n-\alpha)J(v)+(\alpha-\alpha_n)J(u_{\alpha_n}).
$$

The last two terms vanish. [Sequential lower semicontinuity](../../../../../../../sequential-lower-semicontinuity.md) at the fixed parameter $\alpha$ implies $\Phi_{\alpha,f}(\bar u)\leq\Phi_{\alpha,f}(v)$. Thus every cluster point is a [global minimizer](../../../../../../../global-minimizer.md) at $\alpha$. Uniqueness makes it $u_\alpha$, and the subsequence property proves

$$
\boxed{u_{\alpha_n}\xrightarrow{\tau}u_\alpha.}
$$

Indeed, a subsequence staying outside a neighborhood of $u_\alpha$ would have a further convergent subsequence, whose limit must be $u_\alpha$, a contradiction.

**The listed existence hypotheses alone do not imply uniqueness or convergence of an arbitrary selection.** For example, on $\mathbb R^2$, set $K(x,y)=x$, $f=1$, and

$$
J(x,y)=x^2+\bigl(\max\{|y|-1,0\}\bigr)^2.
$$

This is nonnegative, [convex](../../../../../../../convex-function.md), [continuous](../../../../../../../continuous-function.md) and has $J(0)=0$; every $\Phi_{\alpha,f}$ has [coercivity](../../../../../../../coercive-function.md). Its minimizers are $(1/(1+2\alpha),y)$ for all $|y|\leq1$. Along $\alpha_n=\alpha+1/n$, selecting $y_n=(-1)^n$ prevents convergence. Without uniqueness, the valid conclusion is that every cluster point minimizes the limiting objective.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [3](../../../3.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
