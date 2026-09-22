# Recursive powerset mapping

↑ **Parent:** [Well-founded recursion](well-founded-recursion.md)

A map $f:a\to\mathcal P(a)$ is recursive if every map $g:\mathcal P(b)\to b$ admits a unique $h:a\to b$ with $h(y)=g(\{h(x):x\in f(y)\})$. This holds exactly when the predecessor relation $x\in f(y)$ is a [well-founded relation](well-founded-relation.md). For the forward construction, take the union of all consistent partial solutions on downward-closed domains; [well-founded induction](well-founded-induction.md) proves compatibility, and a minimal missing point allows extension. Conversely, a nonempty subset with no minimal point has an upward reachability closure $T$ satisfying $y\in T$ exactly when some predecessor is in $T$. With $b=\{0,1\}$ and $g(S)=1$ exactly when $1\in S$, both the zero map and the indicator of $T$ solve the recursion, contradicting uniqueness.

## ↑ Ancestors (7)

1. [Well-founded recursion](well-founded-recursion.md)
2. [Well-founded relation](well-founded-relation.md)
3. [Set theory](set-theory-split.md)
4. [Foundations of mathematics](foundations-of-mathematics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-4/16g/solution.md)
