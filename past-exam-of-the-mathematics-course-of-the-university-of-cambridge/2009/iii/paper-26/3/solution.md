<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Here a [formal group law](../../../../../formal-group-law.md) means a one-dimensional commutative law $F(X,Y)\in R[[X,Y]]$ with $F(X,0)=X$, $F(0,Y)=Y$, $F(X,Y)=F(Y,X)$ and $F(F(X,Y),Z)=F(X,F(Y,Z))$. It has leading part $X+Y$ and a recursively determined [formal inverse](../../../../../formal-inverse.md) $i_F(T)=-T+O(T^2)$. A homomorphism $h(T)\in TR[[T]]$ satisfies $h(F(X,Y))=G(h(X),h(Y))$. It is an isomorphism precisely when its linear coefficient is a unit of $R$: necessity follows by composing with an inverse, while sufficiency follows by recursive inversion of the series and then the homomorphism identity. Over a field the condition is **$\boxed{h'(0)\ne0}$**.

The characteristic-zero classification is that every such law over $K$ has a unique isomorphism to the [formal additive group](../../../../../formal-additive-group.md) with linear coefficient one. This is its [formal logarithm](../../../../../formal-logarithm.md). To prove it, put $f(T)=\partial_YF(T,0)$, whose constant term is one, and define

$$
\ell_F(T)=\int_0^T\frac{du}{f(u)}=T+O(T^2).
$$

Integration is coefficientwise, which is possible over the characteristic-zero field. Differentiate associativity with respect to $Z$ at zero to obtain

$$
f(F(X,Y))=\partial_YF(X,Y)f(Y).
$$

It follows that $\partial_Y\ell_F(F(X,Y))=1/f(Y)=\ell_F'(Y)$. The difference $\ell_F(F(X,Y))-\ell_F(Y)$ is therefore independent of $Y$; evaluating at $Y=0$ gives

$$
\boxed{\ell_F(F(X,Y))=\ell_F(X)+\ell_F(Y).}
$$

Its linear coefficient one makes it invertible as a formal series. Conversely, a homomorphism from $F$ to the additive law with derivative $c$ satisfies $h'(T)f(T)=c$, by differentiating its defining identity at the second variable zero. Thus $h=c\ell_F$. In particular the normalized logarithm is unique, and every homomorphism between two laws over $K$ is $\ell_G^{-1}(c\ell_F(T))$, with an isomorphism exactly when $c\ne0$. This is a formal classification; analytic convergence is a separate issue.

Now suppose $F$ is defined over $\mathcal O_K$. Write $v_K(\pi)=1$, $e=v_K(p)$ and let the residue field have size $q$. Since $f(T)$ and its reciprocal have integral coefficients, writing $\ell_F(T)=T+\sum_{n\geq2}c_nT^n$ gives the [valuation bound for coefficients of an integral formal logarithm](../../../../../valuation-bound-for-coefficients-of-an-integral-formal-logarithm.md)

$$
v_K(c_n)\geq-e\,v_p(n).
$$

Therefore the logarithm converges on $\pi\mathcal O_K$, as $nv_K(t)-e v_p(n)$ tends to infinity. Choose an integer $s>e/(p-1)$ and put $g(t)=\ell_F(t)-t$. For $t,u\in\pi^s\mathcal O_K$, factoring $t^n-u^n$ gives

$$
v_K(c_n(t^n-u^n))\geq v_K(t-u)+(n-1)s-e v_p(n)>v_K(t-u).
$$

The last inequality uses $v_p(n)\leq(n-1)/(p-1)$, since $n\geq p^{v_p(n)}\geq1+(p-1)v_p(n)$. It follows that $g$ maps this ball into $\pi^{s+1}\mathcal O_K$ and is strictly contracting, gaining at least one unit of valuation in differences.

For any $z\in\pi^s\mathcal O_K$, iterate $t_{j+1}=z-g(t_j)$ from $t_0=z$. The iterates remain in the ball, their differences gain valuation at each step, and completeness gives a limit solving $\ell_F(t)=z$. The same difference estimate makes this solution unique. Hence the logarithm is a [group isomorphism](../../../../../group-isomorphism.md)

$$
\boxed{F(\pi^s\mathcal O_K)\cong(\pi^s\mathcal O_K,+)\cong(\mathcal O_K,+).}
$$

The [formal logarithm](../../../../../formal-logarithm.md) identity applies analytically on this ball because the integral group law and all the convergent logarithm series may be substituted there. Finally reduction of the formal parameter modulo $\pi^s$ is a [group homomorphism](../../../../../group-homomorphism.md) from $F(\pi\mathcal O_K)$ onto the finite group on $\pi\mathcal O_K/\pi^s\mathcal O_K$, with kernel $F(\pi^s\mathcal O_K)$. Its index is $q^{s-1}$. Thus the required additive subgroup has finite index, as described by the [deep logarithm subgroup of a formal group](../../../../../deep-logarithm-subgroup-of-a-formal-group.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 26](../../paper-26-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
