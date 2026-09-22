# Shapley value axioms

↑ **Parent:** [Shapley value](shapley-value.md)

[Cooperative-game efficiency](efficiency-of-a-cooperative-game-value.md), [cooperative-game symmetry](symmetry-of-a-cooperative-game-value.md), the [null player](null-player.md) axiom and [cooperative-game additivity](additivity-of-a-cooperative-game-value.md) characterize the [Shapley value](shapley-value.md). The ordering-average definition satisfies all four: marginal totals telescope, relabelling players preserves the ordering average, zero marginals average to zero and marginal contributions add pointwise. The original work gives an equivalent axiomatization combining some of these requirements.[RAND P-295, 1952, abstract: a value deduced from three axioms](a-value-for-n-person-games-by-lloyd-shapley-rand-paper.md)

For uniqueness, write $u_T$ for the [unanimity game](unanimity-game.md) of a nonempty [coalition](coalition-game-theory.md) $T$. Recursively define $a_T=v(T)-\sum_{\varnothing\ne R\subsetneq T}a_R$ in increasing order of $|T|$. Then $v(S)=\sum_{\varnothing\ne T\subseteq S}a_T$, so $v=\sum_{\varnothing\ne T\subseteq N}a_Tu_T$. Apply the axioms to every scaled [unanimity game](unanimity-game.md) $a_Tu_T$. Players outside $T$ receive zero; [cooperative-game symmetry](symmetry-of-a-cooperative-game-value.md) and [cooperative-game efficiency](efficiency-of-a-cooperative-game-value.md) give each player inside $T$ the amount $a_T/|T|$. Every game is a finite [sum](sum.md) of such scaled [unanimity games](unanimity-game.md), and [cooperative-game additivity](additivity-of-a-cooperative-game-value.md) therefore determines every allocation uniquely. Applying the axioms directly to the scaled games avoids assuming real homogeneity from additivity alone.

## ↑ Ancestors (8)

1. [Shapley value](shapley-value.md)
2. [Transferable utility game](transferable-utility-game.md)
3. [Cooperative game theory](cooperative-game-theory.md)
4. [Game theory](game-theory-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [A Value for N-Person Games by Lloyd Shapley (RAND paper)](a-value-for-n-person-games-by-lloyd-shapley-rand-paper.md)
