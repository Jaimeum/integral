To solve the integral analytically:

$$
\int_0^{\pi/2} \int_{1/(\cos d + \sin d)}^{1} r^3 \, dr \, dd
$$

we continue from the point where we split the integral into two parts:

$$
\int_0^{\pi/2} \left( \frac{1}{4} - \frac{1}{4(\cos d + \sin d)^4} \right) \, dd
$$

### Step 1: Evaluate the Simple Integral
First, we evaluate the simpler part of the integral:

$$
\frac{1}{4} \int_0^{\pi/2} \, dd = \frac{1}{4} \cdot \frac{\pi}{2} = \frac{\pi}{8}
$$

### Step 2: Evaluate the Complex Integral
Now, we need to evaluate the more complex part:

$$
\frac{1}{4} \int_0^{\pi/2} \frac{1}{(\cos d + \sin d)^4} \, dd
$$

To solve this, we use the symmetry and properties of trigonometric functions. Let's use the substitution \( t = \tan(d) \):

For \( d \in [0, \pi/2] \):
- When \( d = 0 \), \( t = 0 \)
- When \( d = \pi/2 \), \( t \to \infty \)

The differential \( dd \) in terms of \( t \) is \( dd = \frac{dt}{1 + t^2} \).

The integral becomes:

$$
\int_0^\infty \frac{1}{(\cos d + \sin d)^4} \cdot \frac{dt}{1 + t^2}
$$

Since \( \cos d = \frac{1}{\sqrt{1 + t^2}} \) and \( \sin d = \frac{t}{\sqrt{1 + t^2}} \):

$$
\cos d + \sin d = \frac{1 + t}{\sqrt{1 + t^2}}
$$

Thus, the integral transforms to:

$$
\int_0^\infty \frac{1}{\left( \frac{1 + t}{\sqrt{1 + t^2}} \right)^4} \cdot \frac{dt}{1 + t^2} = \int_0^\infty \frac{(1 + t^2)^2}{(1 + t)^4} \cdot \frac{dt}{1 + t^2} = \int_0^\infty \frac{1}{(1 + t)^4} dt
$$

Now, simplify and integrate:

$$
\int_0^\infty \frac{dt}{(1 + t)^4}
$$

This integral can be solved using the formula for integrals of the form:

$$
\int_0^\infty \frac{dt}{(1 + t)^n} = \frac{1}{n - 1}
$$

for \( n > 1 \). Here, \( n = 4 \):

$$
\int_0^\infty \frac{dt}{(1 + t)^4} = \frac{1}{3}
$$

Thus, the complex part of the integral evaluates to:

$$
\frac{1}{4} \cdot \frac{1}{3} = \frac{1}{12}
$$

### Step 3: Combine Results
Combining both parts, we get:

$$
\frac{\pi}{8} - \frac{1}{12}
$$

Simplify:

$$
\frac{\pi}{8} - \frac{1}{12} = \frac{3\pi}{24} - \frac{2}{24} = \frac{3\pi - 2}{24}
$$

So, the final result is:

$$
\int_0^{\pi/2} \int_{1/(\cos d + \sin d)}^{1} r^3 \, dr \, dd = \frac{3\pi - 2}{24}
$$
