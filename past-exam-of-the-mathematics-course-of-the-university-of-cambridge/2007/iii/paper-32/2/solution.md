<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For a [Lipschitz continuous](../../../../../lipschitz-continuity.md) path $x:[0,T]\to V$, define its [signature of a bounded variation path](../../../../../signature-of-a-bounded-variation-path.md) in the [truncated tensor algebra](../../../../../truncated-tensor-algebra.md) by

$$
S_N(x)_{s,t}=\left(1,X^{(1)}_{s,t},\ldots,X^{(N)}_{s,t}\right),\qquad
X^{(k)}_{s,t}=\int_{s<u_1<\cdots<u_k<t}
 dx_{u_1}\otimes\cdots\otimes dx_{u_k}.
$$

The [Riemann-Stieltjes integrals](../../../../../riemann-stieltjes-integral.md) exist since $x$ has [bounded variation](../../../../../total-variation-of-a-function.md). Equivalently, since $x$ is absolutely continuous, the integrand is $x'(u_1)\otimes\cdots\otimes x'(u_k)$ with Lebesgue integration on the ordered simplex. The degree-zero component is $1$, and

$$
|X^{(k)}_{s,t}|\le\frac{|x|_{1\text{-var};[s,t]}^k}{k!}.
$$

The lift solves $dS=S\otimes dx$, starting at the identity. Since its velocities belong to the first layer, its endpoint lies in the [free step-N nilpotent Lie group](../../../../../free-step-n-nilpotent-lie-group.md).

For $s\le t\le u$, partition the degree-$k$ integration simplex according to how many integration variables lie before $t$. If exactly $j$ do, the integral factors as the first $j$-fold integral on $[s,t]$ tensor the last $(k-j)$-fold integral on $[t,u]$. The boundaries with a time equal to $t$ have zero measure. Thus

$$
X^{(k)}_{s,u}=\sum_{j=0}^k X^{(j)}_{s,t}\otimes X^{(k-j)}_{t,u},
$$

which is precisely the [Chen identity](../../../../../chen-identity.md):

$$
\boxed{S_N(x)_{s,u}=S_N(x)_{s,t}\otimes S_N(x)_{t,u}.}
$$

This proves the identity at every level, including $k=0$, rather than just checking the first two levels.

For a strictly increasing continuously differentiable map $\psi:[a,b]\to[0,T]$, the actual [change of variables formula](../../../../../change-of-variables-formula.md) is

$$
\boxed{S_N(x\circ\psi)_{a,b}=S_N(x)_{\psi(a),\psi(b)}.}
$$

To prove it, substitute $u_j=\psi(v_j)$ in each ordered integral. Strict increase preserves the order, and the almost-everywhere chain rule gives $d(x\circ\psi)(v)=x'(\psi(v))\psi'(v)\,dv$. The resulting integral is over $\psi(a)<u_1<\cdots<u_k<\psi(b)$. A vanishing derivative at some points causes no difficulty: monotone continuously differentiable substitution still applies, and the zero derivative contributes no variation.

Therefore **orientation-preserving reparametrisation of the whole segment preserves its [path signature](../../../../../signature-of-a-bounded-variation-path.md)**. On $[0,1]$ the printed equality needs $\psi(0)=0$ and $\psi(1)=1$, equivalently that $\psi$ be onto. These endpoints are not forced by the stated assumptions. For example $x(t)=te_1$ and $\psi(t)=t/2$ satisfy those assumptions, but

$$
S_N(x)_{0,1}=\exp(e_1),\qquad
S_N(x\circ\psi)_{0,1}=\exp(e_1/2),
$$

which already differ at level one for every $N\ge1$. The endpoint-preserving interpretation proves the intended invariance, while the general formula states exactly what remains true without it.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
