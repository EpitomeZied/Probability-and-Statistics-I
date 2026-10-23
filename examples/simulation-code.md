# Simulation code examples

MATLAB and Python (NumPy) listings from Appendix A of the [lecture notes](../notes/lecture-notes.pdf). Original examples by Waleed A. Yousef; Python equivalents by Mahmoud AboZied.

Python listings use NumPy and Matplotlib and reuse variables from earlier listings; read them in order. MATLAB listings are retained as instructional transcripts.

## Listing 1: MATLAB

```matlab
n=100; mu=0; sigma=1;
x = random('normal', mu, sigma, [n,1]);
plot(x, zeros([length(x),1]), '.r');
```

## Listing 2: Python

```python
import numpy as np, matplotlib.pyplot as plt
rng = np.random.default_rng(0)
x = rng.normal(0, 1, 100)
plt.plot(x, np.zeros_like(x), '.r'); plt.show()
```

## Listing 3: MATLAB

```matlab
n=1000; mu=0; sigma=1;
x = random('normal', mu, sigma, [n,1]);
figure; hold on;
[N, xout] = hist(x);
bar(xout, N/(n*(xout(2)-xout(1))), 'barwidth', 1, 'facecolor', 'r');
bar(xout, N/n, 'barwidth', 1, 'facecolor', 'b');
z = -4:.01:4;
y = 1/(sqrt(2*pi)*sigma) * exp(-(z-mu).^2 / (2*(sigma^2)));
plot(z, y, 'k', 'LineWidth', 2);
plot(x, zeros([length(x),1]), '.r');
```

## Listing 4: Python

```python
x = rng.normal(0, 1, 1000)
N, edges = np.histogram(x, bins=10); d = edges[1] - edges[0]; mid = edges[:-1] + d/2
plt.bar(mid, N/(len(x)*d), width=d, color='r'); plt.bar(mid, N/len(x), width=d, color='b')
z = np.linspace(-4, 4, 801); plt.plot(z, np.exp(-z**2/2)/np.sqrt(2*np.pi), 'k', lw=2); plt.show()
```

## Listing 5: MATLAB

```matlab
P = {x1, ..., xM};   % Data Generated
S = 0;
for m = 1:M
    if (R(xm))
        S = S + g(xm);
    end
end
ret = S/M;
```

## Listing 6: Python

```python
P = rng.normal(0, 1, M)              # data generated
ret = np.mean(np.where(R(P), g(P), 0))
```

## Listing 7: MATLAB

```matlab
M=1000; mu=0; sigma=1; K=100;
muhat = zeros([1,K]);
for k = 1:K               % repeating MC
    P = random('normal', mu, sigma, [M,1]);
    S = 0;
    for m = 1:M
        S = S + P(m);
    end
    muhat(k) = S/M;
end
% Shorter:
P = random('normal', mu, sigma, [M,K]);
muhat = mean(P, 1);
```

## Listing 8: Python

```python
muhat = rng.normal(0, 1, (1000, 100)).mean(axis=0)   # K = 100 MC repetitions
print(muhat.std(ddof=1), 1/np.sqrt(1000))            # both about 0.0316
```

## Listing 9: MATLAB

```matlab
M=1000; n=100; mu=0; sigma=1;
y = zeros([M,1]);
for m = 1:M
    D = random('normal', mu, sigma, [n,1]);
    y(m) = max(D);
end
```

## Listing 10: Python

```python
y = rng.normal(0, 1, (1000, 100)).max(axis=1)        # M = 1000 datasets of n = 100
```

## Listing 11: MATLAB

```matlab
P = {x1, ..., xM};   % Data Generated
S = 0; Mprim = 0;
for m = 1:M
    if (e(xm))
        Mprim = Mprim + 1;
        if (R(xm))
            S = S + g(xm);
        end
    end
end
ret = S/Mprim;
```

## Listing 12: Python

```python
keep = e(P)                                           # condition on the event
ret = np.sum(np.where(R(P[keep]), g(P[keep]), 0)) / keep.sum()
```

## Listing 13: Python

```python
urn = np.array([1, 1, 1, 0])
draws = np.array([rng.permutation(urn)[:2] for _ in range(100_000)])
first_red = draws[:, 0] == 1
print(draws[first_red, 1].mean())                   # about 0.667
```
