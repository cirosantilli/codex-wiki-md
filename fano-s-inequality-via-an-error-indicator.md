<h1 id="fano-s-inequality-via-an-error-indicator">Fano's inequality via an error indicator</h1>

↑ **Parent:** [Fano's inequality](fano-s-inequality.md)

For a guess $f(Y)$ of a finite-alphabet variable $X$, let $Z=1_{X\ne f(Y)}$ and $p_e=P(Z=1)$. The [chain rule for conditional entropy](chain-rule-for-conditional-entropy.md) gives $H(X\mid Y)=H(Z\mid Y)+H(X\mid Z,Y)$. The first term is at most the [binary entropy](binary-entropy.md) $h(p_e)$. The second is zero when the guess is right and at most $\log_2(|J_X|-1)$ when it is wrong, proving $H(X\mid Y)\leq h(p_e)+p_e\log_2(|J_X|-1)$. This needs no optimality assumption on the guess.

## ↑ Ancestors (7)

1. [Fano's inequality](fano-s-inequality.md)
2. [Conditional entropy](conditional-entropy.md)
3. [Information theory](information-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Chain rule for conditional entropy](chain-rule-for-conditional-entropy.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-60/2/ii/c/solution.md)
