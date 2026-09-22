<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a [locally small category](../../../../../../locally-small-category.md) $\mathcal C$, an object $C$, and a [categorical presheaf](../../../../../../presheaf-category-theory.md) $X:\mathcal C^{\mathrm{op}}\to\mathbf{Set}$, the [Yoneda lemma](../../../../../../yoneda-lemma.md) gives the [natural bijection](../../../../../../natural-bijection.md)

$$
\boxed{\Phi_{C,X}:\operatorname{Nat}(\mathcal C(-,C),X)\cong X(C).}
$$

Its two maps are explicitly

$$
\Phi_{C,X}(\alpha)=\alpha_C(1_C),\qquad
\Psi_{C,X}(x)_A(f)=X(f)(x)\quad(f:A\to C).
$$

For $u:A'\to A$, the equation $X(u)X(f)(x)=X(fu)(x)$ proves [naturality](../../../../../../naturality.md) of $\Psi(x)$. Evaluating it at the [identity morphism](../../../../../../identity-morphism.md) gives $\Phi\Psi(x)=x$. Conversely, [naturality](../../../../../../naturality.md) of $\alpha$ at $f:A\to C$ gives

$$
\alpha_A(f)=X(f)(\alpha_C(1_C)),
$$

so $\Psi\Phi(\alpha)=\alpha$. **Evaluation at the identity and transport of an element along a morphism are mutually inverse.**

The [bijection](../../../../../../bijection.md) is natural in both variables: a [natural transformation](../../../../../../natural-transformation.md) $\theta:X\Rightarrow Y$ sends $\Phi(\alpha)$ to $\theta_C(\Phi(\alpha))$, matching $\Phi(\theta\alpha)$; and $g:C\to C'$ gives

$$
\Phi_{C,X}(\alpha\circ\mathcal C(-,g))
=X(g)(\Phi_{C',X}(\alpha))
\quad\bigl(\alpha:\mathcal C(-,C')\Rightarrow X\bigr).
$$

For completeness, the covariant [Yoneda lemma](../../../../../../yoneda-lemma.md) for $Y:\mathcal C\to\mathbf{Set}$ is $\operatorname{Nat}(\mathcal C(C,-),Y)\cong Y(C)$, with $\alpha\mapsto\alpha_C(1_C)$ and inverse $y\mapsto(f:C\to A\mapsto Y(f)(y))$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
