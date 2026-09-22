<h1 id="4/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $g(y)=f_y(y)f(y)$. The [chain rule](../../../../../../chain-rule.md) gives $y''=g(y)$ along a smooth solution. Expanding every term about $t_n$, the unscaled exact-solution residual of this [multiderivative multistep method](../../../../../../multiderivative-multistep-method.md) is

$$
R_h=\frac{5a-11}{6}h^3y'''(t_n)
+\frac{23a-57}{24}h^4y^{(4)}(t_n)+O(h^5).
$$

For example, at derivative degree $q\geq2$ its coefficient is

$$
\frac{2^q-(1+a)}{q!}
-\frac{3-a}{2}\frac{2^{q-2}}{(q-2)!};
$$

the coefficients at degrees zero, one and two vanish. Thus the formal [order of a numerical method](../../../../../../order-of-a-numerical-method.md) is **two for $a\ne11/5$**, and **three for $a=11/5$**, where the fourth-degree coefficient is $-4/15$. This order statement describes the exact-solution defect; convergence also needs [zero-stability](../../../../../../zero-stability.md).

At $h=0$ the characteristic polynomial is

$$
\rho(\zeta)=\zeta^2-(1+a)\zeta+a=(\zeta-1)(\zeta-a).
$$

The [root condition for a multistep method](../../../../../../root-condition-for-a-multistep-method.md) holds exactly when $|a|\leq1$ and $a\ne1$. In particular $a=-1$ has two distinct unit roots and is admissible, whereas $a=1$ has a repeated unit root. Applying the permitted [Dahlquist equivalence theorem](../../../../../../dahlquist-equivalence-theorem.md) for this multiderivative setting, with smooth $f$, the nearby implicit solution branch and convergent starting values, yields

$$
\boxed{\text{convergent exactly for }-1\leq a<1.}
$$

All those methods have **global order two**, provided the starting errors are $O(h^2)$. The formally third-order choice $a=11/5$ is not zero-stable and therefore is not convergent as a method for general initial-value problems.

One can see the failure without any nonlinear difficulty. For $y'=0$, an error mode $e_n=a^n e_0$ grows exponentially if $|a|>1$. At $a=1$, $e_n=C+Dn$; choosing $e_0=0$, $e_1=h$ gives vanishing starting errors but $e_{T/h}=T$. This also explains why a small residual alone does not rescue that degenerate choice: at $a=1$ the first-derivative term disappears and the formula has no zero-stable first-order evolution interpretation.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
