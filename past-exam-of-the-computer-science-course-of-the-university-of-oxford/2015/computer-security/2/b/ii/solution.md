<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Alice can still authenticate Bob when she accepts a genuine fresh ticket and successfully checks $E_{k_{AB}}(\text{Hello Alice})$. The [session key](../../../../../../session-key.md) inside her ticket is Tim's genuine key, protected by her [public key](../../../../../../public-key.md) together with $\mathit{secret}_A$. Tim gives that same key only to Alice and to the holder of Bob's [private key](../../../../../../private-key.md). The adversary cannot derive it, and honest Tim does not send the greeting. Alice has not sent that greeting either. Thus the matching greeting is evidence that Bob obtained the key and participated. The different final greetings prevent simply reflecting Alice's own confirmation back at her.

Bob's intended freshness test is that $\mathit{nonce}_B$ was hidden in his request encrypted for Tim, so a matching answer must follow Tim's processing of that request. This establishes that Tim revealed that [cryptographic nonce](../../../../../../cryptographic-nonce.md); it does not authenticate the adjacent ticket. The substitution attack in [solution](../i/solution.md) may use an old adversary-known $z$ instead of a fresh one. Bob accepts it even though its freshness is false.

$$
\boxed{\text{Alice's check can authenticate Bob; Bob's accepted key need not be fresh.}}
$$

The defect is the absence of a cryptographic binding between Bob's [cryptographic nonce](../../../../../../cryptographic-nonce.md) and his key ticket. A repair must bind the identities, both [cryptographic nonces](../../../../../../cryptographic-nonce.md) and the [session key](../../../../../../session-key.md) under [message authentication](../../../../../../message-authentication.md) verifiable as Tim's, for example a [digital signature](../../../../../../digital-signature.md) by Tim over the response, checked before Bob accepts. Merely moving the nonce inside a public-key-encrypted ticket is insufficient once an attacker knows or predicts it: anyone can create such an [encryption](../../../../../../encryption.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
