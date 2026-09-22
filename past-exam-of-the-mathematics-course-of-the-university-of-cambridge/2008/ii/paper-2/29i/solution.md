<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

The average-cost [Bellman equation](../../../../../bellman-equation.md) is

$$
\boxed{g+\theta(x)=\inf_{a\in A}\left[c(x,a)+\sum_y p_{xy}(a)\theta(y)\right].}
$$

If a constant $g$ and bounded relative cost function $\theta$ solve this equation and a stationary control attains the infimum in each state, that control is optimal and its long-run expected average cost is $g$. Indeed the Bellman inequality telescopes along any controlled trajectory; dividing by the number of steps removes the bounded endpoint terms and gives a lower bound $g$. The attaining policy makes the inequalities equalities. An unbounded $\theta$ requires the corresponding endpoint/transversality justification, which the question permits for this example.

To maximize occupation of zero, minimize $c(x,u)=-1_{\{x=0\}}$ and try $\theta(x)=\mu|x|$ with $\mu>0$. For $x>0$, the expected increment of $\theta$ is $\mu(2u-1)$, minimized at $u=\alpha$; for $x<0$, it is $\mu(1-2u)$, minimized at $u=1-\alpha$. At zero its expected next value is $\mu$, independent of $u$. Thus $g=\mu(2\alpha-1)$ away from zero and $g=-1+\mu$ at zero. Solving gives

$$
\boxed{\mu=\frac1{2(1-\alpha)},\qquad g=-\frac{1-2\alpha}{2(1-\alpha)},\qquad\pi_{\max}=-g=\frac{1-2\alpha}{2(1-\alpha)}.}
$$

An optimal control always biases a nonzero position towards zero: $u=\alpha$ on positive integers, $u=1-\alpha$ on negative integers, and any allowed $u$ at zero.

As an independent occupation check, fix the choice $u_0$ at zero. The stationary positive tail begins at $\pi_1=\pi_0u_0/(1-\alpha)$ and has common ratio $\alpha/(1-\alpha)$; the negative tail begins at $\pi_{-1}=\pi_0(1-u_0)/(1-\alpha)$ with the same ratio. Summing these geometric tails gives $1=\pi_0[1+1/(1-2\alpha)]$, reproducing the boxed optimum. The chain has period two, but its time-averaged occupation still converges to this stationary proportion.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
