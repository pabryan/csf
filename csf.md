# The Curve Shortening Flow

## Introduction

The [Curve Shortening Flow ](https://en.wikipedia.org/wiki/Curve-shortening_flow) is a _geometric evolution equation_ whereby a curve is deformed in the direction of its curvature vector. It is the geometric heat equation for curves in the sense that the speed is the Laplacian with respect to the arc-length parameter.

Despite the initial impression, the Curve Shortening Flow is a quasi-linear parabolic equation since the arc-length parameter depends on first derivatives of the embedding. As a heat equation, it enjoys smoothing properties. It is a reaction-diffusion equation and as such there is an interplay between the diffusion and reaction terms. Perhaps the most important theorem is that for simple, closed curves in the plane, the diffusion terms dominates leading to long time convergence to a static solution; namely a circle, after rescaling. This result is known as the [Gage-Hamilton-Grayson Theorem](https://en.wikipedia.org/wiki/Curve-shortening_flow#Gage%E2%80%93Hamilton%E2%80%93Grayson_theorem).

## Curve Theory

- Parametrisation
- Arc-length
- Length
- Area
- Curvature

## The Curve Shortening Flow

### Definition

\begin{equation}
\partial_t c = \vec{\kappa} = -\kappa N.
\end{equation}

Let's take a look at an example.

### Example

**The Shrinking Circle**

\begin{equation}
c(u, t) = \sqrt{1-r_0^2} (\cos u, \sin u)
\end{equation}

### Lemma

In a parametrisation, the CSF is the evolution equation
\begin{equation}
\partial_t (x, y) =
\end{equation}

## Evolution Equations

### Lemma

The commutator of arc length and time derivatives is
\begin{equation}
[\partial_t, \partial_s] = - \kappa^2 \partial_s
\end{equation}

## Long Time Behaviour

### Theorem

[Gage-Hamilton-Grayson Theorem](https://en.wikipedia.org/wiki/Curve-shortening_flow#Gage%E2%80%93Hamilton%E2%80%93Grayson_theorem)

The CSF exists on the maximal time interval \([0, T)\) where \(T = \tfrac{A_0}{2\pi}\) where \(A_0\) is the initial area. Upon rescaling to fix the total length, the CSF converges smoothly to a circle of total length \(L_0\) as \(t \to T\) where \(L_0\) is the initial length.

## Numerical Simulation

Here we investigate the behaviour of the CSF via numerical simulations.

## References
