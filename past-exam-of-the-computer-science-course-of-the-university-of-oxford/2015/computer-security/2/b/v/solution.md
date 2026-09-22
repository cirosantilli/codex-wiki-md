<h1 id="2/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Bob especially needs unpredictability, because $\mathit{nonce}_B$ is intended to be secret until Tim processes the request. A predictable counter destroys even that limited assurance.

If the adversary knows Bob's next value $b$, it initiates a run with Alice's name and intercepts Bob's request. Without consulting Tim, it chooses a key $z$, constructs $V^*=E_{\mathit{pk}_B}(A\Vert B\Vert z)$, and sends $(U^*,b,V^*)$ as message 3, with any suitably shaped opaque ticket $U^*$ for Alice. Bob cannot inspect that ticket. He accepts $z$, sends message 4, and accepts the adversary's $E_z(\text{Hello Bob})$. Alice and Tim need not participate.

This [preplay attack](../../../../../../preplay-attack.md) requires a correct prediction of Bob's outstanding value, knowledge of his [public key](../../../../../../public-key.md), and the ability to intercept or race the genuine response. Observing an earlier unencrypted response may expose a counter value from which to predict the next. With an independent uniformly random hidden $64$-[bit](../../../../../../bit.md) value, blind prediction succeeds with [probability](../../../../../../probability.md) $2^{-64}$ per attempt.

$$
\boxed{\text{A random hidden nonce blocks prediction, but not message-3 substitution.}}
$$

In particular, random [cryptographic nonces](../../../../../../cryptographic-nonce.md) do not make the printed [protocol](../../../../../../communication-protocol.md) sound. After the genuine message 3 reveals $b$, the adversary can use exactly the substitution in [solution](../i/solution.md). Predictability allows an earlier attack without Tim; lack of response binding allows an attack even with perfect unpredictability.

## ↑ Ancestors (12)

1. [V](../v.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Computer security](../../../../computer-security-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
