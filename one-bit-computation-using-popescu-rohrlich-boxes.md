<h1 id="one-bit-computation-using-popescu-rohrlich-boxes">One-bit computation using Popescu–Rohrlich boxes</h1>

↑ **Parent:** [Popescu–Rohrlich box](popescu-rohrlich-box.md)

Take a [separated Boolean decomposition](separated-boolean-decomposition.md) $f(x,y)=\bigoplus_{\ell}u_\ell(x)v_\ell(y)$. Feed $(u_\ell,v_\ell)$ to one independent [PR box](popescu-rohrlich-box.md), obtaining outputs with $a_\ell\oplus b_\ell=u_\ell v_\ell$. Alice forms $A=\bigoplus_\ell a_\ell$, Bob forms $B=\bigoplus_\ell b_\ell$, and their parities satisfy $A\oplus B=f$. Sending the single bit $A$ lets Bob compute the answer with certainty. The truth-table decomposition needs at most $2^{\min(m,n)}$ boxes for input lengths $m,n$. Each box's local output is uniform, so Bob's uncommunicated output string carries no information about Alice's input; the final parity bit is essential for a general function depending on that input.

## ↑ Ancestors (9)

1. [Popescu–Rohrlich box](popescu-rohrlich-box.md)
2. [No-signalling box](no-signalling-box.md)
3. [CHSH inequality](chsh-inequality.md)
4. [Bell theorem](bell-theorem.md)
5. [Foundations of quantum mechanics](foundations-of-quantum-mechanics.md)
6. [Quantum theory](quantum-theory-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Communication complexity](communication-complexity.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-59/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-59/4/solution.md)
