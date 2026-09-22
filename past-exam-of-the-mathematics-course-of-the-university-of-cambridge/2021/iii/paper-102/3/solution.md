<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A finite-dimensional [Lie algebra representation](../../../../../lie-algebra-representation.md) is a homomorphism $\rho:L\to\mathfrak{gl}(V)$. It is irreducible when $V$ has no invariant subspaces other than $0$ and $V$.

The algebra $\mathfrak{sl}_2$ has basis $e,f,h$ with

$$
[h,e]=2e,\qquad[h,f]=-2f,\qquad[e,f]=h.
$$

For every $n\geq0$, its $(n+1)$-dimensional irreducible module $V(n)$ has basis $v_0,\ldots,v_n$ and action

$$
hv_i=(n-2i)v_i,\qquad
fv_i=v_{i+1},\qquad
ev_i=i(n-i+1)v_{i-1},
$$

with out-of-range vectors zero. Any nonzero invariant subspace contains a weight vector; repeated application of $e$ reaches $v_0$, and repeated application of $f$ then generates the whole module, proving irreducibility. The adjoint module of $\mathfrak{sl}_2$ is $V(2)$, so every ideal is an invariant subspace and $\mathfrak{sl}_2$ is simple.

For a root $\alpha$, nondegeneracy of the Killing pairing between $L_\alpha$ and $L_{-\alpha}$ allows choices $e_\alpha,f_\alpha$ with

$$
h_\alpha=[e_\alpha,f_\alpha],\qquad
\alpha(h_\alpha)=2.
$$

After rescaling, $(e_\alpha,f_\alpha,h_\alpha)$ obey the $\mathfrak{sl}_2$ relations, giving a copy of $\mathfrak{sl}_2$ in $U_\alpha$.

Restrict the adjoint representation of $L$ to this copy. Finite-dimensional $\mathfrak{sl}_2$ theory shows that the $\alpha$-string through zero has one nontrivial summand $V(2)$, with weight spaces $L_{-\alpha}$, $\mathbb Ch_\alpha$, and $L_\alpha$. Any additional vector in $L_\alpha$ would generate another weight-two summand and another independent zero-weight coroot, contradicting nondegeneracy of the root--coroot pairing on $H$. Hence

$$
\boxed{\dim L_\alpha=1.}
$$

For $\beta\notin\mathbb Z\alpha$, the space

$$
W=\bigoplus_{k=-q}^pL_{\beta+k\alpha}
$$

is stable under $e_\alpha,f_\alpha,h_\alpha$. Adjacent raising and lowering maps are nonzero until the endpoints, and every root space is one-dimensional, so $W$ is a simple $\mathfrak{sl}_2$-module of highest weight $p+q$. Its lowest and highest $h_\alpha$-weights give

$$
\beta(h_\alpha)-2q=-(p+q),\qquad
\beta(h_\alpha)+2p=p+q,
$$

and therefore $\beta(h_\alpha)=q-p$. Since $[L_\alpha,L_{-\alpha}]=\mathbb Ch_\alpha$, every $x$ in this bracket line satisfies

$$
\boxed{\beta(x)=\frac{q-p}{2}\alpha(x).}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 102](../../paper-102-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
