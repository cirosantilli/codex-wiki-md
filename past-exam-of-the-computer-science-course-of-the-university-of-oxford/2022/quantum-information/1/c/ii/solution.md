<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $p_{ab}$ denote the conditional winning [probability](../../../../../../probability.md) in the [CHSH game](../../../../../../chsh-game.md). With both settings zero, [computational-basis measurements](../../../../../../quantum-measurement-in-the-computational-basis.md) of the [Bell state](../../../../../../bell-state-split.md) always agree, so $p_{00}=1$. When just one setting is one, Bob's conditional [pure state](../../../../../../pure-state.md) from part (i), or the corresponding calculation with Alice and Bob exchanged, gives agreement [probability](../../../../../../probability.md) $\cos^2\theta$. Hence $p_{01}=p_{10}=\cos^2\theta$.

For $a=b=1$, winning requires different output [bits](../../../../../../bit.md). Alice obtains each of her two outcomes with [probability](../../../../../../probability.md) $1/2$. Given her first outcome, Bob's desired overlap is

$$
\langle f_1(\theta)|e_0(\theta)\rangle=2\sin\theta\cos\theta=\sin2\theta;
$$

given her second outcome, the other desired overlap is $\langle f_0(\theta)|e_1(\theta)\rangle=-\sin2\theta$. Thus $p_{11}=\sin^2(2\theta)$. Averaging over the four equally likely inputs gives

$$
\boxed{p_{\mathrm{win}}(\theta)=\frac{1+2\cos^2\theta+\sin^2(2\theta)}4
=\frac{3+\cos2\theta-\cos^2(2\theta)}4.}
$$

The maximum winning [probability](../../../../../../probability.md) for noncommunicating classical players is $3/4$, the game form of the [CHSH inequality](../../../../../../chsh-inequality.md). Setting $t=\cos2\theta$, strict improvement requires $t-t^2>0$, or $0<t<1$. On the stipulated interval this gives

$$
\boxed{0<\theta<\frac\pi4.}
$$

The endpoints give equality with the classical bound. Within this [reflected real-basis CHSH strategy](../../../../../../reflected-real-basis-chsh-strategy.md), the maximum is $13/16$ at $t=1/2$, namely $\theta=\pi/6$; this follows by completing the square in $t$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Quantum information](../../../../quantum-information-split.md)
5. [2022](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
