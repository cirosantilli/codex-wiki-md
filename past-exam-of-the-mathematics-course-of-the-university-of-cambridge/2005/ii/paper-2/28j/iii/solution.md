<h1 id="28j/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The equalities are valid at a differentiable interior optimum under the intended concave formulation, but not under the printed assumptions alone. To derive the intended result, differentiate the finite conditional sum in the Bellman objective. For an interior [portfolio](../../../../../../investment-portfolio.md) fraction with positive invested wealth, its derivative gives

$$
0=E_n[V_{n+1}'(w_{n+1}^*)(X_{n+1}-r)].
$$

The [consumption](../../../../../../consumption.md) derivative gives $U'(c_n^*)=E_n[V_{n+1}'(w_{n+1}^*)G_{\theta_n^*}]$. Since $G_\theta=r+\theta(X-r)$, the first equality cancels its risky part and yields the second requested equality. The envelope derivative with respect to wealth gives $V_n'(w_n^*)=E_n[V_{n+1}'(w_{n+1}^*)G_{\theta_n^*}]$, giving the third. Thus, under these added hypotheses,

$$
\boxed{E_n[V_{n+1}'(w_{n+1}^*)(X_{n+1}-r)]=0,
\qquad U'(c_n^*)=rE_n[V_{n+1}'(w_{n+1}^*)]=V_n'(w_n^*).}
$$

The first prices the excess stock payoff using future marginal utility; the second equates marginal utility from consuming now to that from saving in the bank; the third identifies the marginal value of wealth with that common quantity. At [portfolio](../../../../../../investment-portfolio.md) or [consumption](../../../../../../consumption.md) boundaries these are replaced by one-sided optimality inequalities. Finiteness of the sample space justifies differentiating a finite sum; it does not ensure differentiability of a [supremum](../../../../../../supremum.md) or an interior optimum.

A concrete counterexample satisfies the printed convex assumptions and attains every [supremum](../../../../../../supremum.md). Take one remaining decision, a one-point sample space, a deterministic stock return $X=x>r>1$, $U(c)=c^2$, and controls in $[0,w]\times[0,1]$. The optimum is $c^*=0,\theta^*=1$, since the objective $c^2+x^2(w-c)^2$ is convex in $c$ and its larger endpoint value is $x^2w^2$. Then $w_{n+1}^*=xw$ and $V_{n+1}'=2xw$. The first claimed [expectation](../../../../../../expected-value.md) is $2xw(x-r)>0$; the second compares $2rxw>0$ to $U'(0)=0$; the third compares $2rxw$ to $V_n'(w)=2x^2w$. All three fail. Consequently **the requested equalities cannot be proved as printed**; the derivation above supplies their precise intended interior version.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [28J](../../28j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
