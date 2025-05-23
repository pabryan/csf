---
jupytext:
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.16.4
kernelspec:
  display_name: Python 3 (ipykernel)
  language: python
  name: python3
---

# The Curve Shortening Flow

## Definition

$$
\partial_t c = \vec{\kappa} = -\kappa N.
$$

Let's take a look at an example.

## Example

**The Shrinking Circle**

$$
c(u, t) = \sqrt{1-r_0^2} (\cos u, \sin u)
$$

```{code-cell} ipython3
:tags: [remove-input]

import numpy as np
import sympy as sp

import pandas as pd

import plotly.express as px
import plotly.graph_objects as go

import plotly.io as pio
pio.templates.default  = "plotly_dark"

import imageio.v3 as iio
```

```{code-cell} ipython3
t = np.linspace(0, 2*np.pi, 100)

xval = np.cos(t)
yval = np.sin(t)

fig = px.line(x = xval, y = yval)
fig.update_yaxes(scaleanchor = "x", scaleratio = 1)

# Hide axes
fig.update_layout(xaxis=dict(visible=False), yaxis=dict(visible=False))

# Make plots transparent
fig.update_layout(
paper_bgcolor = 'rgba(0,0,0,0)', plot_bgcolor='rgba(0,0,0,0)')

fig
```

## Lemma

In a parametrisation, the CSF is the evolution equation
$$
\partial_t (x, y) =
$$
