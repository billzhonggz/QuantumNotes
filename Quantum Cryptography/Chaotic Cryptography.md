# Chaotic Cryptography

> See also: https://en.wikipedia.org/wiki/Chaotic_cryptology
> 
> The reference comes directly from my supervisor.

Chaotic Cryptography combines Chaos Theory with modern cryptography. There are several types of Chaotic Cryptography.

## Discrete-Time and Continuous-Time Encryption

Compared with the conventional cryptography which is being used practically in modern systems, despite dealing with discrete values in discrete time, chaotic cryptography can also deal with *continuous values* in both *continuous* and *discrete time*.

- **Discrete-Value Chaotic Cryptosystems** uses *Discretized Chaotic Maps* (block ciphers, symmetric ciphers).
- **Continuous-Value Chaotic Cryptosystems** uses *chaotic nonlinear functions*. These functions dynamics are forced to exhibit chaotic behavior to achieve continuous-value cryptography.
  - Example done by Cuomo et al. (1993) uses *Lorenz-based chaotic circuit*
  - Example done by Murali et al. (2001) uses *chaotic signal encryption*

## Ways of Encoding

There are different ways to encoding information transmitted through a chaotic cryptography system.

### Chaotic Masking (CMask)

*CMask* system works both continuous and discrete information signals.

In a CMask system,

- The *encoder* generates chaotic signal ("noise") from chaotic system.
- These *noise* are added to the information signal (masking).
- The *sum* of the noise and message is transmitted to the receiver.
- The *decoder* uses a equivalent chaotic system to synchronize with the encoder's system, and then reconstruct the signals (noise).
- The *receiver* recovers the message through deducting the noise by above reconstruction.

### Chaos Shift Keying (CSK)

*CSK* systems deal with *discrete* information signals.

In a CSK system,

- The *encoder* consists of more than one *autonomous chaotic systems*. Each of them is having different parameters.
- At every single period of time, *one* of the systems' output signals is chosen to be transmitted.
- The *decoder* has the same number of chaotic systems. They work in in pairs with chaotic systems in the encoder side.
- By *adjusting their parameter values*, only *one* pair of the system can be synchronized at a time.
- Then the *decoder* can recover the encrypted information.
