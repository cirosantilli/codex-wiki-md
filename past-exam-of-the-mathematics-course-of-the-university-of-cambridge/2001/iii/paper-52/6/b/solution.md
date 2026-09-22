<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under the standard [two-condition criterion for evolutionary stability](../../../../../../two-condition-criterion-for-evolutionary-stability.md), the strict claim fails. [Tit for tat](../../../../../../tit-for-tat.md) and [always cooperate](../../../../../../always-cooperate.md) both cooperate in every round when playing either each other or their own type under the specified initial memories. Hence

$$
e({\rm TFT},{\rm TFT})=e({\rm ALLC},{\rm TFT})
=e({\rm TFT},{\rm ALLC})=e({\rm ALLC},{\rm ALLC})=R.
$$

Both stability comparisons tie. The [neutrality between Tit for tat and unconditional cooperation](../../../../../../neutrality-between-tit-for-tat-and-unconditional-cooperation.md) proves that **Tit for tat is not an evolutionarily stable strategy in the stated strategy space**, and cannot strictly invade every strategy. The final differently spelled name is interpreted as the same $(1,0)$ rule, since no second strategy is defined.

There is a useful qualified invasion result. For a resident $M=(p,q)$ with $|p-q|<1$, put $z=q/(1-p+q)$. The [long-run payoff of reactive strategies](../../../../../../long-run-payoff-of-reactive-strategies.md) gives

$$
e({\rm TFT},M)=e(M,{\rm TFT})=e(M,M)
=g(z)=Rz^2+(S+T)z(1-z)+P(1-z)^2.
$$

Thus, if the fraction of [Tit for tat](../../../../../../tit-for-tat.md) players is $\varepsilon$, their [payoff](../../../../../../payoff.md) advantage is

$$
\boxed{w_{\rm TFT}-w_M=\varepsilon[R-g(z)].}
$$

Moreover $R-g(z)=(1-z)[R-P+(R+P-S-T)z]$. Under the additional cooperative-efficiency condition $2R\ge S+T$, this is positive whenever $z<1$. [Tit for tat invasion of a reactive resident](../../../../../../tit-for-tat-invasion-of-a-reactive-resident.md) then occurs from every positive frequency, although its invasion exponent at frequency zero vanishes. The [replicator equation](../../../../../../replicator-equation.md) is $\dot\varepsilon=[R-g(z)]\varepsilon^2(1-\varepsilon)$, so the initial increase is slow and frequency-dependent. Residents with $p=1$ remain cooperative on all reached histories and tie instead. If $S+T>2R$, some almost-cooperative residents have $g(z)>R$, and even this qualified invasion conclusion fails.

For the exceptional opposite-response resident $(0,1)$, its self-payoff is $h=(R+P)/2$ while its [payoff](../../../../../../payoff.md) in either order against [Tit for tat](../../../../../../tit-for-tat.md) is $g=(R+S+T+P)/4$. The advantage is $(1-\varepsilon)(g-h)+\varepsilon(R-g)$. Under $2R\ge S+T$, invasion at arbitrarily small frequency requires $S+T\ge R+P$; otherwise it needs

$$
\boxed{\varepsilon>\frac{R+P-S-T}{2(2R-S-T)}.}
$$

Finally, taking an infinite undiscounted average before the rare-mutant [limit](../../../../../../limit-of-a-function.md) is essential. In an $L$-round match against [always defect](../../../../../../always-defect.md), the first round contributes $S$ to [Tit for tat](../../../../../../tit-for-tat.md) and $T$ to the defector, followed by $L-1$ rounds of [payoff](../../../../../../payoff.md) $P$. The [finite-horizon invasion threshold of Tit for tat against unconditional defection](../../../../../../finite-horizon-invasion-threshold-of-tit-for-tat-against-unconditional-defection.md) is

$$
\boxed{\varepsilon>\frac{P-S}{L(R-P)-(T+S-2P)}},
$$

provided the denominator is positive and the threshold is below one. Thus a finite horizon generally prevents invasion from an arbitrarily rare introduction. The source's absent [payoff](../../../../../../payoff.md) table prevents choosing which extra [payoff](../../../../../../payoff.md) inequalities were intended, but the symbolic cases and the strict-ESS counterexample do not depend on guessing it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
