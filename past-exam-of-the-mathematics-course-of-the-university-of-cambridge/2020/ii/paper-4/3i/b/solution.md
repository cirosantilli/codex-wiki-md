<h1 id="3i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Perform every addition in the [finite field](../../../../../../finite-field.md) $\mathbb F_2$. From the two transmitted strings $c_i=a_i+k_i$ and $d_i=a_i+k_{i+1}$ one obtains

$$
c_i+d_i=k_i+k_{i+1}\qquad(1\leq i\leq N).
$$

Choosing one candidate value of $k_1$ recursively determines $k_2,\ldots,k_{N+1}$, and hence determines the candidate plaintext $a_i=c_i+k_i$. There are only two candidates: changing $k_1$ complements every recovered key bit and every plaintext bit. The information that the message makes sense normally selects the intended candidate.

Once this ambiguity is resolved, any other ciphertext positions encrypted with the recovered segment $k_1,\ldots,k_{N+1}$ can be decrypted. Key bits outside that segment remain [independent](../../../../../../independent-random-variables.md) and uniformly distributed, so this mistake gives no information about messages using only those bits. This is the [two-time pad attack](../../../../../../two-time-pad-attack.md): reusing related one-time-pad key material destroys [perfect secrecy](../../../../../../perfect-secrecy.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3I](../../3i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
