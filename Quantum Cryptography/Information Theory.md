# Information Theory

> Reference: section 3, *Quantum Cryptography and Secret-Key Distillation*

## Source Coding (Encoding)

### Shannon Entropy

> See also: <https://en.wikipedia.org/wiki/Entropy_(information_theory)>

The *Shannon Entropy* of a discrete random variable $X$ is denoted by $H(X)$ and is defined as follow, all logarithms are in base 2.

$H(X) = - \sum_x P_X(x) \log P_X(x)$

The *entropy* of a binary random variable with distribution $\{p, 1-p\}$ for $0 \leq p \leq 1$ is denoted as

$h(p) = -p \log p - (1-p) \log(1-p)$.

**The *Shannon Entropy* is a property of the distribution $P_X(x)$, but not the symbol set $\mathcal{X}$.**

For a particular encoding method, the entropy of a random variable tells us precisely about its compressibility. More on *Huffman Coding* later.

### Properties of source codes

> See also: <https://en.wikipedia.org/wiki/Shannon%27s_source_coding_theorem>

<!-- TODO: Get more materials to understand the source coding theorem. -->

The source coding theorem establishes a limit of data compression.
