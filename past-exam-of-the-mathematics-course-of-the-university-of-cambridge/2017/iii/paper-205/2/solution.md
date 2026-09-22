<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the normalization

$$
\widehat\beta\in\operatorname*{argmin}_{\beta\in\mathbb R^p}\left\{\frac{\|Y-X\beta\|_2^2}{2n}+\lambda\|\beta\|_1\right\}
$$

for the [Lasso](../../../../../lasso.md). A centered [sub-Gaussian random variable](../../../../../sub-gaussian-distribution.md) with parameter $\sigma$ satisfies $\mathbb E e^{tW}\le e^{\sigma^2t^2/2}$ for all $t\in\mathbb R$; for a noncentered variable apply this definition to $W-\mathbb EW$. With fixed $X$, [independence](../../../../../independent-random-variables.md) of the errors gives

$$
\mathbb E\exp\left(t\frac{X_j^T\varepsilon}{n}\right)\le\exp\left(\frac{\sigma^2t^2\|X_j\|_2^2}{2n^2}\right)=\exp\left(\frac{\sigma^2t^2}{2n}\right).
$$

The [exponential Markov bound](../../../../../exponential-markov-bound.md), optimized over $t$ separately for the two signs, gives $\Pr(|X_j^T\varepsilon|/n>u)\le2e^{-nu^2/(2\sigma^2)}$. Take $u=\lambda/2=\sigma A\sqrt{\log p/n}$ and apply the [union bound](../../../../../boole-s-inequality.md) over columns:

$$
\boxed{\Pr(\Omega)\ge1-2p\exp(-A^2\log p/2)=1-2p^{-(A^2/2-1)}.}
$$

The specified positive tuning parameter requires $p\ge2$; at $p=1$ its formula is zero. For small $A$ the [probability](../../../../../probability.md) lower bound can be negative and hence uninformative. Although centering makes the centered errors dependent, $X^T\mathbf1=0$ means $X^T(\varepsilon-\bar\varepsilon\mathbf1)=X^T\varepsilon$, so the preceding proof uses the original independent errors, not independence after centering.

The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md), using the [subdifferential of the L1 norm](../../../../../subdifferential-of-the-l1-norm.md), are

$$
\frac{X^T(Y-X\widehat\beta)}n=\lambda z,\qquad
z_j=\operatorname{sgn}(\widehat\beta_j)\ (\widehat\beta_j\ne0),\quad |z_j|\le1\ (\widehat\beta_j=0).
$$

Consequently, for nonempty $B\subseteq\widehat S$, on $\Omega$,

$$
\begin{aligned}
\frac{\operatorname{sgn}(\widehat\beta_B)^TX_B^TX(\beta^0-\widehat\beta)}n
&=\lambda|B|-\frac{\operatorname{sgn}(\widehat\beta_B)^TX_B^T\varepsilon}n\\
&\ge\lambda|B|-|B|\frac{\|X^T\varepsilon\|_\infty}n\ge\frac{\lambda|B|}{2}.
\end{aligned}
$$

This establishes the required active-set inequality without any rank condition on $X$.

For $s>0$, a sufficient [Compatibility condition for the Lasso](../../../../../compatibility-condition-for-the-lasso.md) is

$$
\frac{s\|X\delta\|_2^2}{n}\ge\phi^2\|\delta_S\|_1^2\quad\text{whenever }\|\delta_{S^c}\|_1\le3\|\delta_S\|_1,\qquad\phi>0.
$$

Indeed, for $\delta=\widehat\beta-\beta^0$, comparison of the two [Lasso](../../../../../lasso.md) objective values and the score bound on $\Omega$ give the [Basic inequality for the Lasso](../../../../../basic-inequality-for-the-lasso.md)

$$
P_E+\lambda\|\delta_{S^c}\|_1\le3\lambda\|\delta_S\|_1,\qquad P_E=\|X\delta\|_2^2/n.
$$

It follows that $\delta$ satisfies the [Lasso cone condition](../../../../../lasso-cone-condition.md) and $\|\delta_S\|_1\le\sqrt{sP_E}/\phi$. Thus $P_E\le3\lambda\sqrt{sP_E}/\phi$, including the trivial $P_E=0$ case. This proves the slightly stronger $P_E\le9\lambda^2s/\phi^2$, and in particular the requested $16\lambda^2s/\phi^2$. If $s=0$, the same basic inequality forces $\widehat\beta=0$ on $\Omega$; no nonempty-support compatibility constant is needed.

For the support-size argument, use the stated prediction bound with constant $16$. Set $b=|B|$. By the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and the definition of the [sparse maximum eigenvalue](../../../../../sparse-maximum-eigenvalue.md),

$$
\begin{aligned}
\frac{\operatorname{sgn}(\widehat\beta_B)^TX_B^TX(\beta^0-\widehat\beta)}n
&\le\frac{\|X_B\operatorname{sgn}(\widehat\beta_B)\|_2}{\sqrt n}\frac{\|X(\beta^0-\widehat\beta)\|_2}{\sqrt n}\\
&\le\kappa_b\sqrt b\,\frac{4\lambda\sqrt s}{\phi}.
\end{aligned}
$$

Combining with the lower bound and squaring gives $\boxed{b\le64\kappa_b^2s/\phi^2}$ for every nonempty $B\subseteq\widehat S$. If $m_*<\infty$ and $\widehat s\ge m_*$, choose $B$ of size $m_*$; this contradicts the strict inequality defining $m_*$. If $m_*=\infty$, $\widehat s\le p<\infty$ proves the assertion directly. Hence $\boxed{\widehat s<m_*}$ in both cases.

When $1<m_*\le p$, minimality and monotonicity of the [sparse maximum eigenvalues](../../../../../sparse-maximum-eigenvalue.md) give

$$
\widehat s\le m_*-1\le\frac{64\kappa_{m_*-1}^2s}{\phi^2}\le\frac{64\kappa_{m_*}^2s}{\phi^2}.
$$

When $m_*=1$, the first result gives $\widehat s=0$, so the same final bound holds. Thus the finite-index conclusion is $\boxed{\widehat s\le64\kappa_{m_*}^2s/\phi^2\quad(m_*<\infty)}$.

There is a genuine domain omission in the printed last assertion: the definition of $\kappa_m$ only makes sense for $1\le m\le p$, so $\kappa_{m_*}$ is undefined when $m_*=\infty$. This case can occur: take centered orthogonal columns with $X^TX/n=I_p$, $n\ge p+1$, $s=p$, and $\phi^2=1$. Then $\kappa_m^2=1$ for every available $m$ and none exceeds $64p$, so $m_*=\infty$. A universally defined replacement, from $B=\widehat S$ and monotonicity, is

$$
\boxed{\widehat s\le64\kappa_p^2s/\phi^2.}
$$

Alternatively, explicitly extend the definition by $\kappa_m=\kappa_p$ for $m>p$, including infinity. Under that added convention the printed final expression is meaningful and follows from this replacement bound. Neither convention nor finiteness should be silently assumed.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
