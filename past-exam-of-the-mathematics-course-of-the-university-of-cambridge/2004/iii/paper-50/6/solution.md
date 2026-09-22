<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Work on the physical domain

$$
s=S+\bar S>0,\qquad t=T+\bar T-|C|^2>0,
$$

and abbreviate $A=ae^{-\alpha S}$, $W=C^3+A+b$, and $B=W-sW_S=C^3+b+(1+\alpha s)A$. There are no [vector multiplets](../../../../../supersymmetric-vector-multiplet.md) specified, hence no additional gauge [D-term](../../../../../d-term.md). In Planck units the [supergravity F-term potential](../../../../../supergravity-f-term-potential.md) and upper-index [supergravity auxiliary fields](../../../../../supergravity-auxiliary-field.md) are

$$
V=e^K(K^{i\bar j}D_iW\,\overline{D_jW}-3|W|^2),\qquad
F^i=-e^{K/2}K^{i\bar j}\overline{D_jW},\qquad e^K=\frac1{st^3}.
$$

The overall auxiliary-field sign is a convention; its vanishing and [norm](../../../../../norm.md) are invariant statements.

The [Kähler covariant derivatives of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) here are

$$
D_SW=-\alpha A-\frac Ws=-\frac Bs,\qquad
D_TW=-\frac{3W}t,\qquad
D_CW=3C^2+\frac{3\bar C W}t.
$$

The [Kähler metric](../../../../../kahler-metric.md), with rows $S,T,C$ and columns their barred partners, is

$$
K_{i\bar j}=\begin{pmatrix}
s^{-2}&0&0\\
0&3/t^2&-3C/t^2\\
0&-3\bar C/t^2&3/t+3|C|^2/t^2
\end{pmatrix}.
$$

Its $T,C$ block is positive definite because its leading diagonal and determinant $9/t^3$ are positive. In the inverse-tensor convention $K_{i\bar j}K^{k\bar j}=\delta_i^k$, the nonzero upper components are

$$
K^{S\bar S}=s^2,\qquad
\begin{pmatrix}K^{T\bar T}&K^{T\bar C}\\K^{C\bar T}&K^{C\bar C}\end{pmatrix}
=\frac t3\begin{pmatrix}t+|C|^2&\bar C\\C&1\end{pmatrix}.
$$

In particular the conjugations in the off-diagonal components matter.

To verify the [no-scale supergravity](../../../../../no-scale-supergravity.md) cancellation explicitly, temporarily write $u=D_TW=-3W/t$ and $v=D_CW=W_C+3\bar CW/t$. Their part of the metric contraction is

$$
\frac t3\{(t+|C|^2)|u|^2+\bar C\,u\bar v+C\,v\bar u+|v|^2\}
=3|W|^2+\frac t3|W_C|^2.
$$

The terms involving $C W_C\bar W$ and its conjugate cancel between the mixed and diagonal contributions. The remaining $3|W|^2$ cancels the universal negative term. Since $W_C=3C^2$, the exact [matter-logarithm no-scale potential](../../../../../matter-logarithm-no-scale-potential.md) is therefore

$$
\boxed{V=\frac{|C^3+b+(1+\alpha s)ae^{-\alpha S}|^2}{st^3}
+\frac{3|C|^4}{st^2}\ge0.}
$$

It differs from a model where $|C|^2$ appears outside the logarithm in the [Kähler potential](../../../../../kahler-potential.md).

Substitution into the auxiliary-field formula gives

$$
\boxed{F^S=e^{K/2}s\bar B,\qquad
F^T=e^{K/2}t(\bar A+\bar b),\qquad
F^C=-e^{K/2}t\bar C^2.}
$$

For example $F^T=e^{K/2}t(\bar W-\bar C\,\overline{W_C}/3)$, which reduces to the displayed expression for the cubic [superpotential](../../../../../superpotential.md). To test unbroken [supersymmetry](../../../../../supersymmetry-split.md) at any finite point, $F^C=0$ first forces $C=0$. Then $F^T=0$ forces $A+b=0$, whereas $F^S=0$ forces $(1+\alpha s)A+b=0$. Subtracting gives $\alpha sA=0$. Because $s>0$, $\alpha>0$ and $e^{-\alpha S}\ne0$ at a finite point, all auxiliaries can vanish only if **$a=b=0$**. Thus every nontrivial choice of $(a,b)$ breaks [supersymmetry](../../../../../supersymmetry-split.md) at finite field values.

A finite zero-energy minimum requires both nonnegative terms of $V$ to vanish:

$$
\boxed{C=0,\qquad b+(1+\alpha s)ae^{-\alpha S}=0.}
$$

There cannot be a finite positive-energy stationary point: keeping $S,C$ fixed and varying the real part of $T$, equivalently $t$, gives

$$
\frac{\partial V}{\partial t}=-\frac{3|B|^2}{st^4}-\frac{6|C|^4}{st^3},
$$

which is strictly negative unless $B=C=0$. Hence these zero-energy solutions are all the possible finite minima.

Because $a,b$ were allowed to be arbitrary, existence must be checked. If both are nonzero, put $x=\alpha s>0$ and $r=|b/a|$. The magnitude equation is

$$
r=(1+x)e^{-x/2}.
$$

The function on the right starts at one at the excluded boundary $x=0$, tends to zero as $x\to\infty$, and has derivative $\tfrac12(1-x)e^{-x/2}$. Its maximum is $2e^{-1/2}$ at $x=1$. Therefore a finite [cubic-matter no-scale vacuum with an exponential dilaton](../../../../../cubic-matter-no-scale-vacuum-with-an-exponential-dilaton.md) exists exactly when

$$
\boxed{a,b\ne0\quad\text{and}\quad0<|b/a|\le2e^{-1/2}.}
$$

There is one finite positive root for $0<r\le1$, two for $1<r<2e^{-1/2}$, and one merged root at the maximum. The complex phase equation fixes $\operatorname{Im}S$ modulo $2\pi/\alpha$. If exactly one of $a,b$ vanishes, or the ratio exceeds the bound, no finite minimum exists; the potential instead has infimum zero along the runaway $t\to\infty$. A zero infimum at an infinite-field boundary is not an attained finite vacuum.

On a nontrivial finite branch, $W=A+b=-\alpha sA\ne0$, so

$$
\boxed{V_{\min}=0,\qquad F^S=F^C=0,\qquad
F^T=e^{K/2}t\bar W\ne0.}
$$

This proves [supersymmetry breaking](../../../../../supersymmetry-breaking.md) at the intended no-scale vacuum. Its zero energy is consistent with the negative gravitational term: $K_{T\bar T}|F^T|^2=3e^K|W|^2$, which cancels $3e^K|W|^2$ in $V$. It is not a counterexample to the global-supersymmetry positivity argument in question 3.

Both real components of $T$ are exactly flat on the vacuum family: $\operatorname{Im}T$ never enters the potential, and at $B=C=0$ every allowed positive $\operatorname{Re}T$ gives the same zero energy. Generically both components of $S$ are fixed. Although the matter field has no quadratic mass there, it is not an exact flat direction: for $S$ fixed at its root, $B=C^3$ and the leading positive potential is $3|C|^4/(st^2)$. At the special merged root $x=1$, the real-$S$ quadratic curvature also vanishes, but higher orders lift it; this does not add a continuous flat vacuum direction. If $a=b=0$, by contrast, $C=0$ is a supersymmetric zero-energy family with both complex $S$ and $T$ flat and all auxiliaries zero. This exception prevents an unconditional breaking assertion for arbitrary constants.

Finally the [gravitino mass from a superpotential](../../../../../gravitino-mass-from-a-superpotential.md) is

$$
\boxed{m_{3/2}=e^{K/2}|W|=\frac{|C^3+ae^{-\alpha S}+b|}{\sqrt{st^3}}.}
$$

At a nontrivial finite minimum it becomes

$$
\boxed{m_{3/2}=\frac{\alpha\sqrt s\,|ae^{-\alpha S}|}{t^{3/2}}
=\frac{\alpha\sqrt s\,|b|}{(1+\alpha s)t^{3/2}}>0.}
$$

Its value varies along the flat volume modulus; the classical potential does not select a unique supersymmetry-breaking or gravitino-mass scale. On the trivial supersymmetric branch $a=b=C=0$, it is zero.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
