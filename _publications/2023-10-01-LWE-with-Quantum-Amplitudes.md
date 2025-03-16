---
title: "LWE with Quantum Amplitudes: Algorithm, Hardness, and Oblivious Sampling"
collection: publications
category: preprint
permalink: /publication/2023-10-01-LWE-with-Quantum-Amplitudes
excerpt: ''
date: 2023-10-01
venue: 'Cryptology ePrint Archive'
slidesurl: 
paperurl: 'https://arxiv.org/pdf/2310.00644'
citation: 'Chen Y, Hu Z, Liu Q, et al. LWE with Quantum Amplitudes: Algorithm, Hardness, and Oblivious Sampling[J]. Cryptology ePrint Archive, 2023.'
---

The learning with errors problem (LWE) is one of the most important building blocks for post-quantum cryptography. To better understand the quantum hardness of LWE, it is crucial to explore quantum variants of LWE. To this end, Chen, Liu, and Zhandry [Eurocrypt 2022] defined \\(\mathsf{S|LWE\rangle}\\) and \\(\mathsf{C|LWE\rangle}\\) problems by encoding the error of LWE samples into quantum amplitudes, and showed efficient quantum algorithms for a few interesting amplitudes. However, algorithms or hardness results of the most interesting amplitude, Gaussian, were not addressed before.

In this paper, we show new algorithms, hardness results and applications for \\(\mathsf{S|LWE\rangle}\\) and \\(\mathsf{S|LWE\rangle}\\) with real Gaussian, Gaussian with linear or quadratic phase terms, and other related amplitudes. Let \\(n\\) be the dimension, \\(q\\) be the modulus of LWE samples. Our main results are

1. There is a \\(2^{\Theta(\sqrt{n\log(q)})}\\)-time algorithm for \\(\mathsf{S|LWE\rangle}\\) with Gaussian amplitude with known phase, given \\(2^{\Theta(\sqrt{n\log(q)})}\\) many quantum samples. The algorithm is modified from Kuperberg's sieve, and in fact works for more general amplitudes as long as the amplitudes and phases are completely known.

2. There is a polynomial time quantum algorithm for solving \\(\mathsf{S|LWE\rangle}\\) and \\(\mathsf{C|LWE\rangle}\\) for Gaussian with quadratic phase amplitudes, where the sample complexity is as small as \\(\tilde{O}(n)\\). As an application, we give a quantum oblivious LWE sampler where the core quantum sampler requires only quasi-linear sample complexity. This improves upon the previous oblivious LWE sampler given by  Debris-Alazard, Fallahpour, Stehlé [STOC 2024], whose core quantum sampler requires \\(\tilde{O}(nr)\\) sample complexity, where r is the standard deviation of the error.

3. There exist polynomial time quantum reductions from standard LWE or worst-case GapSVP to \\(\mathsf{S|LWE\rangle}\\) with Gaussian amplitude with small unknown phase, and arbitrarily many samples. Compared to the first two items, the appearance of the unknown phase term places a barrier in designing efficient quantum algorithm for solving standard LWE via \\(\mathsf{S|LWE\rangle}\\).