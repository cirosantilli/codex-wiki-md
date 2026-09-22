<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

At a positive state $x$, the future is constant. At zero, the residual holding time is independent rate-one exponential and the next state is an independent uniform mark. Thus the conditional future given the natural filtration depends only on the present state: $X$ is a [Markov jump process](../../../../../../markov-jump-process.md). For any bounded Borel $g$, its transition semigroup is

$$
P_hg(0)=e^{-h}g(0)+(1-e^{-h})\int_0^1g(y)dy,\qquad P_hg(x)=g(x)\quad(x>0).
$$

The [Lévy kernel of a Markov jump process](../../../../../../levy-kernel-of-a-markov-jump-process.md), written in destination-state convention, is

$$
\boxed{q(x,dy)=\mathbf1_{\{x=0\}}\mathbf1_{(0,1)}(y)dy.}
$$

In displacement convention it has the same expression $K(x,dz)=\mathbf1_{\{x=0\}}\mathbf1_{(0,1)}(z)dz$, since its only nonzero jump rate is from zero. The [Markov jump-process generator](../../../../../../markov-jump-process-generator.md) is $Lg(x)=\mathbf1_{\{x=0\}}(\int_0^1g(y)dy-g(0))$.

We state the generator martingale theorem used here: for a nonexplosive Markov jump process and a bounded $g$ with bounded $Lg$, the process $g(X_t)-g(X_0)-\int_0^t Lg(X_{s-})ds$ is a true martingale. In this one-jump model it also follows directly from part (a), first for mark indicators and then by bounded-function approximation.

Take $g_\theta(x)=e^{\theta x}$, and put

$$
r_\theta=\int_0^1(e^{\theta y}-1)dy=\begin{cases}(e^\theta-1)/\theta-1,&\theta\ne0,\\0,&\theta=0.\end{cases}
$$

Here $Lg_\theta(x)/g_\theta(x)=r_\theta\mathbf1_{\{x=0\}}$. Therefore choose the [previsible process](../../../../../../predictable-process.md)

$$
\boxed{Y_t=\int_0^t r_\theta\mathbf1_{\{X_{s-}=0\}}ds=r_\theta(t\wedge T).}
$$

It is continuous adapted and thus predictable. To verify the exponential, write $dg_\theta(X_t)=dN_t+Lg_\theta(X_{t-})dt$ with the generator martingale $N$. The [semimartingale integration by parts](../../../../../../semimartingale-integration-by-parts.md) formula, using the continuous finite-variation factor $e^{-Y_t}$, gives

$$
d(e^{-Y_t}g_\theta(X_t))=e^{-Y_t}dN_t+e^{-Y_t}\bigl(Lg_\theta(X_{t-})-g_\theta(X_{t-})Y'_t\bigr)dt=e^{-Y_t}dN_t.
$$

Thus $Z_t=e^{\theta X_t-Y_t}$ is a local martingale. On each fixed horizon it is bounded by $e^{|\theta|+|r_\theta|t}$, so it is a true martingale with $Z_0=1$. This is the [exponential martingale from a jump generator](../../../../../../exponential-martingale-from-a-jump-generator.md); for $\theta=0$ it reduces to the constant process one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
