<h1 id="cea-s-lemma">Céa's lemma</h1>

↑ **Parent:** [Galerkin orthogonality](galerkin-orthogonality.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Céa's_lemma)

For a continuous coercive bilinear form with continuity constant $M$ and coercivity constant $\alpha$, a conforming finite-element solution satisfies

$$
\|u-u_h\|_V\leq\frac M\alpha
\inf_{v_h\in V_h}\|u-v_h\|_V.
$$

For a symmetric problem measured in its [energy norm](energy-norm.md), the constant is one.

For any $v_h\in V_h$, [Galerkin orthogonality](galerkin-orthogonality.md) gives $a(e,e)=a(e,u-v_h)$, where $e=u-u_h$. Coercivity and continuity yield $\alpha\|e\|_V^2\leq M\|e\|_V\|u-v_h\|_V$. Divide by $\|e\|_V$ when it is nonzero and take the infimum. In the symmetric case, the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) in the [energy norm](energy-norm.md) gives the constant one.

**Table of contents**

- [Aubin–Nitsche duality argument](aubin-nitsche-duality-argument.md)

## ↑ Ancestors (7)

1. [Galerkin orthogonality](galerkin-orthogonality.md)
2. [Finite element method](finite-element-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
