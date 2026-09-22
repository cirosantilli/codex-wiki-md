<h1 id="2/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

An unpredictable random $64$-[bit](../../../../../../bit.md) [cryptographic nonce](../../../../../../cryptographic-nonce.md) is better for Alice than a predictable counter, provided repetitions are detected or made sufficiently unlikely. Alice wants a matching ticket to imply a response to her present challenge, and the [protocol](../../../../../../communication-protocol.md) lets anyone ask Tim for a ticket containing a chosen $\mathit{nonce}_A$.

Suppose an adversary predicts that Alice's next challenge for Bob will be $a$. Before Alice starts that run, the adversary sends $(A,B,a)$ to Bob as message 1. Bob asks Tim for a [session key](../../../../../../session-key.md) $k$ and returns the genuine pair $(U,E_k(\text{Hello Alice}))$ in message 4. The adversary stores that pair and lets the early run lapse. Later, when Alice really emits $(A,B,a)$, the adversary blocks it and delivers the stored pair. Alice's ticket and greeting checks pass, despite the key and Bob's participation predating her run. This is a [preplay attack](../../../../../../preplay-attack.md) on freshness and recent participation. Bob need not accept Alice's eventual message 5 for Alice's acceptance to have failed its freshness goal.

Success requires the predicted value and identities to match, an early run that yields the matching ticket and greeting, and Alice to accept solely from the outstanding value without additional expiry or run binding. No [session key](../../../../../../session-key.md) disclosure is needed to defeat freshness; if that old key has also been compromised, impersonation and loss of [cryptographic confidentiality](../../../../../../cryptographic-confidentiality.md) follow as well.

$$
\boxed{\text{Use an unpredictable fresh nonce to resist advance collection of valid replies.}}
$$

A guess at a particular uniformly random value has [probability](../../../../../../probability.md) $2^{-64}$ per independent attempt, with success approximately $r/2^{64}$ for $r$ distinct guesses when that ratio is small. Random choice does not itself guarantee uniqueness: among $t$ independent values the [birthday problem](../../../../../../birthday-problem.md) collision scale is approximately $t(t-1)/2^{65}$. Counter uniqueness and unpredictability are different requirements.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
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
