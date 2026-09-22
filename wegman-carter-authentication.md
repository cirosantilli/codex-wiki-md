<h1 id="wegman-carter-authentication">Wegman–Carter authentication</h1>

↑ **Parent:** [Message authentication code](message-authentication-code.md)

Combine a secret randomly selected [almost strongly universal hash family](almost-strongly-universal-hash-family.md) member with a fresh secret output mask. An observed [message authentication code](message-authentication-code.md) tag leaves the hash-selection key hidden, and the conditional hash bound controls substitution forgery probability. The message itself need not be encrypted. Mask reuse can reveal hash differences; repeated-use guarantees require fresh masks and an appropriate analysis of verification information. A one-use polynomial construction needs only two secret field elements, even for a much longer message.

## ↑ Ancestors (5)

1. [Message authentication code](message-authentication-code.md)
2. [Message authentication](message-authentication.md)
3. [Cryptography](cryptography.md)
4. [Computer science](computer-science-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-54/3/solution.md)
