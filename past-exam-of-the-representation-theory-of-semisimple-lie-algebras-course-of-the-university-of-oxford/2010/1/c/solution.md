<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $V\ne0$ be finite-dimensional. Choose an $H$-[eigenvector](../../../../eigenvector.md) and apply $e$ repeatedly until the last nonzero vector $v$ in that chain. Such a last vector exists because $e$ raises the $H$-[eigenvalue](../../../../eigenvalue.md) by two and $H$ has only finitely many eigenvalues. Then $ev=0$ and $Hv=lv$ for some $l$.

The nonzero $f$-chain cannot continue indefinitely, since its weights are distinct. Part (a), with its zero endpoint included, gives $l\in\mathbb Z_{\ge0}$ and the [basis](../../../../basis.md) $v,fv,\ldots,f^lv$. The raising formula in part (a) shows its span is a [submodule](../../../../submodule.md) isomorphic to $A_l$.

To prove $A_l$ [irreducible](../../../../irreducible-representation.md), a nonzero [submodule](../../../../submodule.md) stable under diagonal $H$ contains a [weight vector](../../../../weight-vector.md): [polynomial interpolation](../../../../polynomial-interpolation.md) in the distinct eigenvalues projects onto individual [representation weight](../../../../weight-of-a-representation.md) lines. Repeated raising reaches $v_0$, and repeated lowering then reaches every $v_k$. Thus the [submodule](../../../../submodule.md) is all of $A_l$. Distinct $l$ give different dimensions $l+1$, so the modules are nonisomorphic. Every finite-dimensional [irreducible](../../../../irreducible-representation.md) [module](../../../../module-mathematics.md) contains one of these nonzero simple submodules and hence equals it. Therefore

$$
\boxed{\{A_l:l\ge0\}\text{ is the complete list of finite-dimensional simple modules}.}
$$

The zero [module](../../../../module-mathematics.md) has no nonzero simple [submodule](../../../../submodule.md) and is dealt with as the empty [direct sum](../../../../direct-sum.md) in part (d).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the representation theory of semisimple Lie algebras course of the University of Oxford](../../../split.md)
5. [Representation theory of semisimple Lie algebras course of the University of Oxford](../../../../representation-theory-of-semisimple-lie-algebras-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
