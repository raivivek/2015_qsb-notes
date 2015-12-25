## Quantifying mutation rates

Mutations are difficult to detect.

- Phenotype
- Sequencing


A classic experiment to detect mutations is Luria Delbruck Experiment.


### Why the lag?

Several examples of cancer data where exposure to carcinogens is followed by
a lag period before cancer is detected.

Hypothesis: It takes time to accumulate mutations in critical cancer genes.

Model: **Target Theory - A Poisson Process**

What is the probability of getting cancer as a function of age?

Let say, mutations strike rate = constant, probability = uniform/length

P(m) = Bin(N,m,p)

N is large, p is small.

Can't directly measure N or p. But possible to measure cancer rate k = p/del(t)
from the data. Using that,

P(m) = Bin(N,m,kT/N)

Which under the assumptions simplifies to a Poisson distribution:

P(m) = Poisson(kT, m)

Now, we apply the model to the real-world data.

What is the probability that a cancer gene gets NO strikes is P(m=0) and gets
ONE or MORE strikes is (1-P(m=0)).

The probability of n genes struck NOT struck one or more times is
(1-exp(-kT))^n. This we call survival probability.


Q: Introduction of virus into cells for transduction


Multiplicity of infection - No of viruses that infect one cell.


Ref: Hecht et. al, 1942
