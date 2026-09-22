<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [truncated tensor algebra](../../../../../../truncated-tensor-algebra.md) $T^{(N)}(\mathbb R^d)=\bigoplus_{k=0}^N(\mathbb R^d)^{\otimes k}$, with truncated concatenation product. The step-$N$ [path signature](../../../../../../signature-of-a-bounded-variation-path.md) is

$$
S_N(x)_{s,t}=1+\sum_{k=1}^N\int_{s<u_1<\cdots<u_k<t}dx_{u_1}\otimes\cdots\otimes dx_{u_k}.
$$

These [iterated integrals of a path](../../../../../../iterated-integral-of-a-path.md) exist as [Riemann-Stieltjes integrals](../../../../../../riemann-stieltjes-integral.md), since a [Lipschitz continuous](../../../../../../lipschitz-continuity.md) path on a compact interval has [bounded variation](../../../../../../total-variation-of-a-function.md). The degree-zero coordinate is $1$, and the degree-one coordinate is $x_t-x_s$.

Let $S_t=S_N(x)_{0,t}$ and write $S_t^{(k)}$ for its degree-$k$ coordinate. Integrating first over all variables except the last gives

$$
S_t^{(k)}=\int_0^t S_u^{(k-1)}\otimes dx_u,\qquad S_t^{(0)}=1.
$$

Thus $dS_t^{(k)}=S_t^{(k-1)}\otimes dx_t$ for $1\leq k\leq N$. If $e_i$ is a standard basis vector, define the linear vector field $W_i(g)=g\otimes e_i$, with degrees above $N$ discarded. The component identities are precisely the controlled [ordinary differential equation](../../../../../../ordinary-differential-equation.md)

$$
\boxed{dS_t=\sum_{i=1}^d W_i(S_t)\,dx_t^i=S_t\otimes dx_t,\qquad S_0=1.}
$$

For a Lipschitz driver this may also be written $\dot S_t=S_t\otimes\dot x_t$ almost everywhere. Recursive integration of its levels proves uniqueness and recovers the signature formula. The [Chen identity](../../../../../../chen-identity.md) follows by splitting each integration simplex at an intermediate time.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
