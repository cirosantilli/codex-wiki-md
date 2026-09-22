<h1 id="19g/solution">Solution</h1>

↑ **Parent:** [19G](../19g.md)

On a maximal torus element $\operatorname{diag}(t,t^{-1})$, the [SU(2) representation](../../../../../representation-theory-of-su-2.md) $V_2$ has weights $2,0,-2$. A monomial with respective multiplicities $a,b,c$ has weight $2(a-c)$, giving

$$
\boxed{\chi_{\operatorname{Sym}^n(V_2)}(t)=\sum_{a+b+c=n}t^{2(a-c)}.}
$$

For $0\leq\ell\leq n$, its weight-$2\ell$ multiplicity is $\lfloor(n-\ell)/2\rfloor+1$, and multiplicities are symmetric in $\ell$. An irreducible $V_{2j}$ contributes one at each weight $2j,2j-2,\ldots,-2j$, so subtracting adjacent multiplicities yields the [symmetric powers of the three-dimensional SU2 representation](../../../../../symmetric-powers-of-the-three-dimensional-su2-representation.md) decomposition

$$
\operatorname{Sym}^n(V_2)\cong\bigoplus_{j=0}^{\lfloor n/2\rfloor}V_{2n-4j}.
$$

It contains the trivial representation once when $n$ is even, and never when $n$ is odd. Therefore

$$
\boxed{\dim\operatorname{Sym}^n(V_2)^{SU(2)}=\begin{cases}1,&n\text{ even},\\0,&n\text{ odd}.\end{cases}}
$$

The double cover $SU(2)\to SO(3)$ identifies $V_2$ with the complexified standard three-dimensional representation. It is self-dual, so the same invariant dimensions apply to homogeneous polynomials. The quadratic form $q=x^2+y^2+z^2$ is invariant, and its powers give nonzero invariants in every even degree. Since each such degree has dimension one and each odd degree has dimension zero, every invariant is a polynomial in $q$. There is no polynomial relation on $q$, as seen by setting $y=z=0$. Thus

$$
\boxed{\mathbb C[x,y,z]^{SO(3)}=\mathbb C[x^2+y^2+z^2].}
$$

## ↑ Ancestors (10)

1. [19G](../19g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
