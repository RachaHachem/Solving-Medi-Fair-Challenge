# Solving-Medi-Fair-Challenge

MEDI-FAIR Competetion website: https://www.codabench.org/competitions/667/

The goal of this challenge is to recover the causal direction of the relationship between two variables A and B. 4 scenarios are possible:

A causes B
B causes A
A and B are both consequences of a common cause C
A and B are independant
For simplicity, we merge the last two scenarios. The participants are asked to produce a confidence score between -inf and +inf, where a positive score indicates that A causes B, and a negative score indicates that B causes A. The higher (or lower in the negative case) the score, the higher the confidence in the answer. A score close to 0 indicates that A and B are independant, or that A and B are both consequences of a common cause.