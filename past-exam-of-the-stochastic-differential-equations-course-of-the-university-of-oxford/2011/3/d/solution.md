<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The initial value can first be subtracted: it is $\mathcal F_0$-measurable and has the same integrability under both measures, since the density has conditional expectation one on $\mathcal F_0$. Put $N=M-\langle M,X\rangle$. Since $dZ=Z\,dX$, the [Itô product rule](../../../../ito-product-rule.md) and the [quadratic covariation](../../../../quadratic-covariation.md) identity $d\langle M,Z\rangle=Z\,d\langle M,X\rangle$ give

$$
d(ZN)=N\,dZ+Z\,dM-Z\,d\langle M,X\rangle+d\langle M,Z\rangle
=N\,dZ+Z\,dM.
$$

This is a local P-martingale. Stop $N$ at increasing bounded levels; the resulting products with $Z$ are true martingales, since they are local martingales dominated at stopping times by a constant times the uniformly integrable density process. Part (c) then shows that the stopped $N$ processes are Q-martingales. Consequently

$$
\boxed{M-\langle M,X\rangle\text{ is a continuous local Q-martingale}.}
$$

The unqualified true-martingale assertion printed in this part needs an additional integrability hypothesis. One sufficient version is a square-integrable P-martingale $M$. Indeed $Z_t\in L^2(P)$ by boundedness of $Y$, and the covariation bound gives

$$
\sup_{s\leq t}|\langle M,X\rangle_s|\leq C\sqrt t\,\langle M\rangle_t^{1/2}.
$$

The [Doob L2 maximal inequality](../../../../doob-l2-maximal-inequality.md), $\mathbb E_P\langle M\rangle_t<\infty$, and [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) therefore give $\mathbb E_Q\sup_{s\leq t}|N_s|<\infty$. Its local martingale identities pass to the limit, making it a true Q-martingale. This is [Girsanov compensation with square-integrable input](../../../../girsanov-compensation-with-square-integrable-input.md).

Here is a counterexample to the broader printed assertion. On $[0,1]$, take $X_s=W_s$, so $Y_s\equiv1$ and $Z_s=e^{W_s-s/2}$. Put $a=1/2$ and

$$
H=\frac{e^{W_a^2}}{1+W_a^2},\qquad
M_s=\begin{cases}0,&s\leq a,\\H(W_s-W_a),&s>a.\end{cases}
$$

Under P, $W_a$ has density $\pi^{-1/2}e^{-x^2}$, so $\mathbb E_PH<\infty$. Independence of future Brownian increments proves $M$ is a continuous true P-martingale. Under Q, $W_s^Q=W_s-s$ is Brownian and the density of $W_a$ is multiplied by $e^{x-1/4}$, so $\mathbb E_QH=\infty$. The compensated process after $a$ is

$$
N_s=H(W_s^Q-W_a^Q).
$$

The future Q-Brownian increment is independent of $H$ and has positive finite expected absolute value. Thus $\mathbb E_Q|N_s|=\infty$ for every $s>a$, so it cannot be a true martingale. This proves that [Bounded Girsanov drift does not preserve true martingales under compensation](../../../../bounded-girsanov-drift-does-not-preserve-true-martingales-under-compensation.md).

For the requested application, the Brownian driver does satisfy the needed conditions. To distinguish the state from the density-driving integral, call the state $U$. Set $Y_s=b(U_s)/a(U_s)$; the stated coefficient bounds make this integrand bounded. Applying the local result to $M=W$ gives

$$
\widetilde W_s=W_s-\int_0^s\frac{b(U_u)}{a(U_u)}du.
$$

It is a continuous local Q-martingale with quadratic variation $s$. The [Lévy characterization of Brownian motion](../../../../levy-characterization-of-brownian-motion.md) therefore makes it a Q-Brownian motion. Substituting $dW_s=d\widetilde W_s+[b(U_s)/a(U_s)]ds$ into the original state equation gives

$$
\boxed{dU_s=a(U_s)\,d\widetilde W_s+b(U_s)\,ds\quad\text{under Q}.}
$$

The Brownian driver after the change is $\widetilde W$; writing it as $W$ again in the last printed equation amounts to renaming that driver.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
