## Numerical computation of the firing rate of a LIF neuron

The firing rate of a LIF neuron receiving a Gaussian distributed noise is known analytically:
<img src="rate.png" height="130" />

The detailed derivation can be found [here](yim_derivation_LIF.pdf). I adopted Equation (26) for the numerical calculation and scipy.integrate.quad was used for computing the improper integral. You can find [my codes here](https://github.com/myyim/LIF). One needs to check convergence by tuning the upper limit in the numerical computation. For the range of parameters I have used, the integrand converges pretty fast.
