<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let

$$
c=\frac{3-\sqrt5}{2}=1-\frac1\varphi,
$$

where $\varphi$ is the [golden ratio](../../../../../../golden-ratio.md). If the [union-closed family](../../../../../../union-closed-family.md) consists of one nonempty set, any element of that set has frequency one, so assume its cardinality exceeds one. Choose independent uniform members $A,B$ and let $X,Y\in\{0,1\}^n$ be their [characteristic vectors of sets](../../../../../../characteristic-vector-of-a-set.md). Then $H(X)=H(Y)=\log|\mathcal A|>0$.

Suppose for a contradiction that every element has frequency $p_i<c$. Put $q_i=1-p_i>1/\varphi$, and let $Z=X\mathbin{\mathrm{OR}}Y$, the [characteristic vector of a set](../../../../../../characteristic-vector-of-a-set.md) of $A\cup B$. The [chain rule for information entropy](../../../../../../chain-rule-for-information-entropy.md) and [conditioning reduces entropy](../../../../../../conditioning-reduces-entropy.md) give

$$
H(Z)=\sum_iH(Z_i\mid Z_{<i})
\geq\sum_iH(Z_i\mid X_{<i},Y_{<i}),
$$

because $Z_{<i}$ is a [function](../../../../../../function-split.md) of $(X_{<i},Y_{<i})$.

Fix the two prefixes and set

$$
x=\mathbb P(X_i=0\mid X_{<i}),
\qquad
y=\mathbb P(Y_i=0\mid Y_{<i}).
$$

The two conditioned bits are [independent random variables](../../../../../../independent-random-variables.md), and $Z_i=0$ exactly when both are zero. The supplied [binary entropy product inequality](../../../../../../binary-entropy-product-inequality.md) therefore gives

$$
H(Z_i\mid X_{<i},Y_{<i})
=h_2(xy)
\geq\frac\varphi2\bigl(xh_2(y)+yh_2(x)\bigr).
$$

Averaging over the independent prefixes yields

$$
\begin{aligned}
H(Z_i\mid X_{<i},Y_{<i})
&\geq\frac\varphi2\bigl(q_iH(Y_i\mid Y_{<i})+q_iH(X_i\mid X_{<i})\bigr)\\
&>\frac12\bigl(H(Y_i\mid Y_{<i})+H(X_i\mid X_{<i})\bigr)
\end{aligned}
$$

whenever either conditional entropy is positive. Summing and using $H(X)>0$ gives $H(Z)>H(X)$.

But [set union](../../../../../../set-union.md) keeps $A\cup B$ inside the [union-closed family](../../../../../../union-closed-family.md), so $Z$ is supported on $\mathcal A$. The [maximum entropy distribution on a finite set](../../../../../../maximum-entropy-distribution-on-a-finite-set.md) gives $H(Z)\leq\log|\mathcal A|=H(X)$, a contradiction. Some element must therefore occur in at least $c|\mathcal A|$ members, proving the [entropy bound for a union-closed family](../../../../../../entropy-bound-for-a-union-closed-family.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 164](../../../paper-164-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
