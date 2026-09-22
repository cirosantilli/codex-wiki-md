<h1 id="5/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An impulse at $a$ shifts the causal [sine](../../../../../sine.md) response. Substituting the [Dirac delta](../../../../../dirac-delta-function.md) in the [convolution](../../../../../convolution.md) from part (i), or using the [Laplace transform time-shift rule](../../../../../laplace-transform-time-shift-rule.md), gives

$$
\boxed{f(x)=H(x-a)\sin(x-a)=
\begin{cases}0,&0\le x<a,\\\sin(x-a),&x\ge a,\end{cases}}
$$

where $H$ is the [Heaviside step function](../../../../../heaviside-step-function.md). The answer is continuous at $a$, while its first [derivative](../../../../../derivative.md) jumps from $0$ to $1$. Consequently its second [distributional derivative](../../../../../distributional-derivative.md) contains exactly one unit [Dirac delta](../../../../../dirac-delta-function.md) at $a$, giving $f''+f=\delta(x-a)$. Since $a>0$, both [initial conditions](../../../../../initial-condition.md) vanish.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
