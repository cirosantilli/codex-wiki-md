<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a probability [measure-preserving system](../../../../../measure-preserving-system.md), the hypothesis is [completely positive entropy](../../../../../completely-positive-entropy.md): every finite [measurable partition](../../../../../measurable-partition.md) with positive static [entropy of a finite measurable partition](../../../../../entropy-of-a-finite-measurable-partition.md) has positive [entropy rate of a measurable partition](../../../../../entropy-rate-of-a-measurable-partition.md). Fix a finite partition $\xi$ and put

$$
\mathcal F_N=\sigma\left(\bigvee_{j\ge N}T^{-j}\xi\right),\qquad\mathcal T(\xi)=\bigcap_{N\ge0}\mathcal F_N.
$$

All [sigma-algebras](../../../../../sigma-algebra.md) are interpreted modulo null sets. We will prove that every finite partition $\alpha$ measurable with respect to this [tail sigma-algebra of a measurable partition](../../../../../tail-sigma-algebra-of-a-measurable-partition.md) has $h_\mu(T,\alpha)=0$. Applying this to a binary partition will force the required triviality. This proves the needed direction of the [Tail characterization of the Pinsker sigma-algebra](../../../../../tail-characterization-of-the-pinsker-sigma-algebra.md) directly, including noninvertible transformations.

Write $h=h_\mu(T,\xi)$. The infinite-future entropy formula and the backwards [chain rule for information entropy](../../../../../chain-rule-for-information-entropy.md) give, for every $L\ge1$, the [block conditional entropy given the infinite future](../../../../../block-conditional-entropy-given-the-infinite-future.md) identity

$$
\boxed{H_\mu(\xi_0^{L-1}\mid\mathcal F_L)=\sum_{j=0}^{L-1}H_\mu(T^{-j}\xi\mid\mathcal F_{j+1})=Lh}.
$$

Each term equals $h$ by invariance of the joint probabilities under a common pullback and continuity of [conditional entropy](../../../../../conditional-entropy.md) under increasing finite future blocks. Invertibility is not needed for this identity.

Fix $\varepsilon>0$. Since $\alpha$ is $\mathcal F_0$-measurable and finite, the [martingale convergence theorem](../../../../../martingale-convergence-theorem.md) and continuity of finite-partition [conditional entropy](../../../../../conditional-entropy.md) allow an $r\ge0$ with

$$
H_\mu(\alpha\mid\xi_0^r)<\varepsilon.
$$

To see the continuity explicitly, for each [partition atom](../../../../../partition-atom.md) $A$ of $\alpha$ the conditional probabilities $\mathbb E[\mathbf1_A\mid\sigma(\xi_0^r)]$ tend to $\mathbf1_A$ almost everywhere; apply [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) to the bounded continuous function $-t\log t$ on $[0,1]$ and sum over the finitely many [partition atoms](../../../../../partition-atom.md).

For $n\ge1$ set $\gamma=\alpha_0^{n-1}$, $L=n+r$, and $\beta=\xi_0^{L-1}$. The [conditional entropy of finite measurable partitions](../../../../../conditional-entropy-of-finite-measurable-partitions.md) satisfies

$$
H(\gamma\mid\beta)\le\sum_{j=0}^{n-1}H(T^{-j}\alpha\mid\beta)\le\sum_{j=0}^{n-1}H(T^{-j}\alpha\mid T^{-j}\xi_0^r)=nH(\alpha\mid\xi_0^r)<n\varepsilon.
$$

The second inequality uses [conditioning reduces entropy](../../../../../conditioning-reduces-entropy.md), since $\beta$ refines each block $T^{-j}\xi_0^r$; the final equality uses measure preservation.

Moreover $\gamma$ is $\mathcal F_L$-measurable. For each $j\ge0$, tail measurability gives $\alpha$ measurable with respect to $\mathcal F_L$, hence $T^{-j}\alpha$ measurable with respect to $T^{-j}\mathcal F_L=\mathcal F_{L+j}\subseteq\mathcal F_L$. Thus [conditioning reduces entropy](../../../../../conditioning-reduces-entropy.md) and the displayed block identity imply

$$
H(\beta\mid\gamma)\ge H(\beta\mid\mathcal F_L)=Lh.
$$

Use the symmetric entropy identity $H(\gamma)=H(\beta)-H(\beta\mid\gamma)+H(\gamma\mid\beta)$ to obtain

$$
0\le\frac1nH(\alpha_0^{n-1})\le\frac{H(\xi_0^{n+r-1})-(n+r)h}{n}+\varepsilon.
$$

The fraction on the right tends to zero: $r$ is fixed and $H(\xi_0^{n+r-1})/(n+r)\to h$ by the definition of [entropy rate of a measurable partition](../../../../../entropy-rate-of-a-measurable-partition.md). Taking $n\to\infty$ and then $\varepsilon\downarrow0$ gives

$$
\boxed{h_\mu(T,\alpha)=0\quad\text{for every finite }\mathcal T(\xi)\text{-measurable partition }\alpha}.
$$

Now let $A\in\mathcal T(\xi)$ and take $\alpha=\{A,X\setminus A\}$. If $0<\mu(A)<1$, its [binary entropy](../../../../../binary-entropy.md) is $-\mu(A)\log\mu(A)-(1-\mu(A))\log(1-\mu(A))>0$, while its entropy rate is zero, contradicting [completely positive entropy](../../../../../completely-positive-entropy.md). Therefore

$$
\boxed{\mu(A)\in\{0,1\}\quad\text{for every }A\in\mathcal T(\xi)}.
$$

Since $\xi$ was arbitrary, every finite-partition tail is trivial. The argument needs only that $\xi$ is finite and the measure is a probability; it does not assume a finite generator, finite total system entropy, or invertibility.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 108](../../paper-108-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
