# Quantum Information Theory

> See also: another set of notes specified for quantum information and computation.
> 
> Reference: section 4, *Quantum Cryptography and Secret-Key Distillation*

In this section, the author of *Quantum Cryptography and Secret-Key Distillation* is going to merge concepts from information theory to the quantum fashion, and some features of quantum information will be discussed.

The quantum bits and states were discussed on another folder `Quantum Computation and Information`. I will ignore these sections here.

## Measurements

> See also: <https://en.wikipedia.org/wiki/Observable>, <https://en.wikipedia.org/wiki/Hilbert_space>

### Observable

In quantum mechanics, physical quantities are associated with linear operators called *observables*, a linear operator is a linear application from $\mathcal{H}$ to $\mathcal{H}$.

An operator $O$ is Hermitian iff $\langle\phi|O|\psi\rangle = \langle\psi|O|\phi\rangle^*$ for all $|\psi\rangle$ and $|\phi\rangle$.

### Discrete orthogonal measurements

If observable $O$ is a finite or countable set of eigenvectors, making an orthonormal basis $\{|b\rangle\}$.

*To be continued*

## Density Matrices and Quantum Systems

Density matrices are unifying classical uncertainties and quantum superpositions. And a Density matrix is a linear operator that represents a quantum state.

A classical random variable, yielding state $|\psi_i\rangle$ with the probability $p_i$, gives the density matrix,

$\rho = \sum_i p_i|\psi_i\rangle\langle\psi_i|$.

<!-- TODO: Read the related materials again in more detail way. -->

## Entropies and Coding

Shannon entropy measures the uncertainty of a classical random variable, the *von Neumann entropy* measures some from of uncertainty in a quantum states. It denotes as

$H(\rho) = - Tr(\rho \log \rho) = - \sum_i \lambda_i \log \lambda_i$.
