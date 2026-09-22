<h1 id="18h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First make the irreducible polynomial monic; for a nonmonic polynomial restore its leading coefficient in front of the product below. If $\alpha$ is one root, $K=\mathbb F_q(\alpha)$ has degree $n$ and cardinality $q^n$. Thus every element satisfies $x^{q^n}=x$. The [Frobenius automorphism](../../../../../../frobenius-automorphism.md) $x\mapsto x^q$ fixes $\mathbb F_q$ and permutes the roots. If the orbit of $\alpha$ had size $d<n$, its orbit product would be a degree-$d$ polynomial fixed by Frobenius, hence with coefficients in $\mathbb F_q$, contradicting irreducibility. Therefore

$$
\boxed{P(X)=\prod_{j=0}^{n-1}(X-\alpha^{q^j}).}
$$

The roots are distinct, since $X^{q^n}-X$ has derivative $-1$. They all lie in $K$ and include its generator $\alpha$, so **the [splitting field](../../../../../../splitting-field.md) is $\mathbb F_{q^n}$**. Frobenius has order $n$ there; a degree-$n$ extension has at most $n$ automorphisms, so

$$
\boxed{\operatorname{Gal}(\mathbb F_{q^n}/\mathbb F_q)\cong C_n.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
