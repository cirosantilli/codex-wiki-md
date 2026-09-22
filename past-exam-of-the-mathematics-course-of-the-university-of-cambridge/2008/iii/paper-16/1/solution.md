<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

We prove the [Roth theorem on three-term arithmetic progressions](../../../../../roth-theorem-on-three-term-arithmetic-progressions.md) by a [density increment](../../../../../density-increment.md) on an ordinary integer [arithmetic progression](../../../../../arithmetic-progression.md). The required increment will be small, but depend only on the current [subset density](../../../../../density-of-a-finite-subset.md).

First establish the increment step. Suppose $A\subseteq[1,L]$ has [subset density](../../../../../density-of-a-finite-subset.md) $\rho=|A|/L>0$ and no nonconstant three-term [arithmetic progression](../../../../../arithmetic-progression.md). Put $M=4L+1$, regard $[1,L]$ as a [subset](../../../../../subset.md) $I$ of the [cyclic group](../../../../../cyclic-group.md) $\mathbb Z_M$, and [set](../../../../../set-split.md) $f=1_A-\rho1_I$. Then $\mathbb E f=0$ and $|f|\leq1$. Use the normalized [Fourier coefficient on a finite abelian group](../../../../../fourier-coefficient-on-a-finite-abelian-group.md)

$$
\widehat g(r)=\mathbb E_{x\in\mathbb Z_M}g(x)e^{-2\pi irx/M}.
$$

The [character orthogonality](../../../../../character-orthogonality.md) geometric-series identity $\mathbb E_xe^{2\pi irx/M}=1$ for $r=0$ and zero otherwise gives [Fourier inversion on a finite group](../../../../../fourier-inversion-on-a-finite-group.md), [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md), and

$$
T(g_0,g_1,g_2):=\mathbb E_{x,h}g_0(x)g_1(x+h)g_2(x+2h)=\sum_r\widehat g_0(r)\widehat g_1(-2r)\widehat g_2(r).
$$

Since $M$ is odd, multiplication by two permutes its frequencies. If one argument is $f$ and the other two have [absolute value](../../../../../absolute-value.md) at most one, [Cauchy-Schwarz](../../../../../cauchy-schwarz-inequality.md) and the [Parseval identity on a finite group](../../../../../parseval-identity-on-a-finite-group.md) give $|T|\leq\max_r|\widehat f(r)|$.

A modular [arithmetic progression](../../../../../arithmetic-progression.md) whose three entries lie in $I$ satisfies the corresponding integer equation: the [absolute value](../../../../../absolute-value.md) of $x+z-2y$ is less than $2L<M$, so congruence to zero forces equality. Thus $T(1_A,1_A,1_A)=|A|/M^2\leq1/(16L)$, since only constant [arithmetic progressions](../../../../../arithmetic-progression.md) remain. Meanwhile, the choices $1\leq x\leq\lfloor L/2\rfloor$ and $0\leq h\leq\lfloor L/4\rfloor$ give at least $L^2/16$ [arithmetic progressions](../../../../../arithmetic-progression.md) in $I$ for $L\geq8$. As $M\leq5L$, this gives $T(1_I,1_I,1_I)\geq1/400$. Expand $1_A=\rho1_I+f$. The seven terms other than the main term are each bounded by $\max|\widehat f|$. For $L\geq50\rho^{-3}$,

$$
7\max_r|\widehat f(r)|\geq\rho^3/400-1/(16L)\geq\rho^3/800.
$$

Consequently a nonzero frequency $r$ obeys $|\widehat f(r)|\geq\gamma$, where $\gamma=\rho^3/6000$. It is nonzero because $\widehat f(0)=0$.

We turn this coefficient into a local increase. Let $Q=\lfloor\sqrt L\rfloor$. Partition the unit circle into $Q$ equal intervals and consider the $Q+1$ points $jr/M$, $0\leq j\leq Q$, modulo one. Two occupy the same interval, yielding an integer $1\leq q\leq Q$ with $\|qr/M\|_{\mathbb R/\mathbb Z}\leq1/Q$. [Set](../../../../../set-split.md) $\ell=\lfloor\gamma Q/200\rfloor$. If $L$ exceeds a sufficiently large absolute multiple of $\rho^{-6}$, then $\ell\geq1$ and each residue-class [arithmetic progression](../../../../../arithmetic-progression.md) of step $q$ in $[1,L]$ has at least $\ell$ terms. Partition each into pieces of lengths between $\ell$ and $2\ell$, distributing the final remainder among the pieces.

On each such [arithmetic progression](../../../../../arithmetic-progression.md) $P$, the [character of a finite abelian group](../../../../../character-of-a-finite-abelian-group.md) $\chi(x)=e^{-2\pi irx/M}$ differs from its value at the first point by at most $4\pi\ell/Q<\gamma/4$. Write $s_P=\sum_{x\in P}f(x)$. Therefore

$$
\gamma M\leq\left|\sum_{x\in I}f(x)\chi(x)\right|\leq\sum_P|s_P|+\gamma L/4,
$$

so $\sum_P|s_P|\geq3\gamma L/4$. But $\sum_Ps_P=\sum_If=0$, and hence the sum of the positive $s_P$ is at least $3\gamma L/8$. Some piece must consequently satisfy $s_P/|P|\geq\gamma/4$. On that piece,

$$
\frac{|A\cap P|}{|P|}\geq\rho+\gamma/4.
$$

Also, once $\gamma Q\geq400$, $|P|\geq\ell\geq\gamma\sqrt L/800$. This proves the [one-frequency density increment on an integer interval](../../../../../one-frequency-density-increment-on-an-integer-interval.md): for absolute constants $c,C>0$, if $L\geq C\rho^{-6}$, there is a [arithmetic progression](../../../../../arithmetic-progression.md) $P\subseteq[1,L]$ of length at least $c\rho^3\sqrt L$ on which the [subset density](../../../../../density-of-a-finite-subset.md) rises by at least $c\rho^3$. For example one may decrease $c$ to $10^{-7}$ and choose $C$ large enough for the displayed elementary inequalities.

Now fix $0<\delta\leq1$ and suppose the required conclusion fails. On each new [arithmetic progression](../../../../../arithmetic-progression.md), identify its points in order with $[1,L']$. This affine identification preserves all integer [arithmetic progressions](../../../../../arithmetic-progression.md), so its copy of $A\cap P$ is still progression-free. All densities remain at least $\delta$. Put $\varepsilon=c\delta^3$, $H=C\delta^{-6}$, and choose an integer $t>1/\varepsilon$. Every increment raises the [subset density](../../../../../density-of-a-finite-subset.md) by at least $\varepsilon$ and changes the length by $L_{j+1}\geq\varepsilon\sqrt{L_j}$. Iterating the latter inequality gives

$$
\log L_j\geq2^{-j}\log N+2(1-2^{-j})\log\varepsilon\geq2^{-t}\log N+2\log\varepsilon\qquad(j\leq t).
$$

Choose $N>(H/\varepsilon^2)^{2^t}$. Then every length up to step $t$ exceeds $H$, so every increment is available. After $t$ increments the [subset density](../../../../../density-of-a-finite-subset.md) exceeds one, a contradiction. Thus

$$
\boxed{\text{For every }\delta>0\text{, all sufficiently large }N\text{ force a nonconstant three-term progression.}}
$$

For $\delta>1$ there are no [sets](../../../../../set-split.md) satisfying the [subset density](../../../../../density-of-a-finite-subset.md) assumption. The argument above proves the substantive case without invoking the theorem being asked for.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
