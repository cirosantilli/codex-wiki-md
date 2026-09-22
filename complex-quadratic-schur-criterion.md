# Complex quadratic Schur criterion

↑ **Parent:** [Schur stability criterion](schur-stability-criterion.md)

For a complex [polynomial](polynomial-split.md) $p(z)=az^2+bz+c$, assume $|a|>|c|$ and put $D=|a|^2-|c|^2$ and $E=\overline a b-c\overline b$. Both [roots of a polynomial](root-of-a-polynomial.md) lie in the closed unit disk if and only if $|E|\leq D$. Strict inequality puts both roots in the open disk. Under the strict product assumption $|c/a|<1$, any unit-modulus root is automatically simple.

To prove the strict version, define $p^\#(z)=z^2\overline{p(1/\overline z)}$ and $q=\overline a p-cp^\#=z(Dz+E)$. On the unit circle $|p^\#|=|p|$, so the [Rouche theorem](rouche-s-theorem.md) shows that a stable $p$ and $q$ have the same two interior zeros. Conversely $Dp=aq+cq^\#$, and the same [Rouche theorem](rouche-s-theorem.md) implies that two interior zeros of $q$ give two interior zeros of $p$. The nonzero root of $q$ is $-E/D$, proving the criterion. The closed version follows by continuity, replacing $b$ by $(1-\varepsilon)b$ in the sufficiency direction. In the necessity direction with a boundary root, replace $p(z)$ by $p(z/r)$ for $r<1$ close to one and let $r\to1$. The product of the two [roots of a polynomial](root-of-a-polynomial.md) excludes two unit-modulus roots and excludes a repeated unit-modulus root.

## ↑ Ancestors (6)

1. [Schur stability criterion](schur-stability-criterion.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [A-stable third-order two-step multiderivative method](a-stable-third-order-two-step-multiderivative-method.md)
- [Bounded-root stability set of the symmetric two-derivative formula](bounded-root-stability-set-of-the-symmetric-two-derivative-formula.md)
- [Empty strict decay domain of the symmetric two-derivative formula](empty-strict-decay-domain-of-the-symmetric-two-derivative-formula.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/4/ii/solution.md)
