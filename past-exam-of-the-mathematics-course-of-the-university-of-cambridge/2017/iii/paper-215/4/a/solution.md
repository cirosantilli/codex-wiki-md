<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\langle f,g\rangle_\pi=\sum_x\pi(x)f(x)g(x)$. The [Dirichlet form of a Markov chain](../../../../../../dirichlet-form-of-a-markov-chain.md) is

$$
\boxed{\mathcal E(f,f)=\langle f,(I-P)f\rangle_\pi=\frac12\sum_{x,y}\pi(x)P(x,y)(f(x)-f(y))^2.}
$$

The equality follows by expanding the square and using row sums one and the [stationary distribution](../../../../../../stationary-distribution.md) identity. For the [reversible Markov chain](../../../../../../reversible-markov-chain.md), [detailed balance](../../../../../../detailed-balance.md) makes $P$ a [self-adjoint operator](../../../../../../self-adjoint-operator.md), with real [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) $f_1\equiv1,f_2,\ldots,f_m$ and ordered [eigenvalues](../../../../../../eigenvalue.md) $1=\lambda_1>\lambda_2\geq\cdots\geq\lambda_m$.

Adding a constant changes neither the [variance](../../../../../../variance-split.md) nor the [Dirichlet form of a Markov chain](../../../../../../dirichlet-form-of-a-markov-chain.md). Expand the centered function as $f-\pi(f)=\sum_{j\geq2}a_jf_j$. Then

$$
\operatorname{Var}_\pi(f)=\sum_{j\geq2}a_j^2,\qquad
\mathcal E(f,f)=\sum_{j\geq2}(1-\lambda_j)a_j^2.
$$

For every nonconstant $f$ the quotient is at least $1-\lambda_2$, and equality is attained at $f=f_2$. This proves

$$
\boxed{\gamma=1-\lambda_2=\min_{\operatorname{Var}_\pi(f)>0}\frac{\mathcal E(f,f)}{\operatorname{Var}_\pi(f)}.}
$$

Equivalently minimize the [Dirichlet form of a Markov chain](../../../../../../dirichlet-form-of-a-markov-chain.md) over centered unit-norm functions. This is the variational characterization underlying the [Poincare inequality for a reversible Markov chain](../../../../../../poincare-inequality-for-a-reversible-markov-chain.md), and does not require the [transition matrix](../../../../../../stochastic-matrix.md) to have nonnegative [eigenvalues](../../../../../../eigenvalue.md). For a one-state chain there is no nonconstant test function; the displayed minimization concerns $m\geq2$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
