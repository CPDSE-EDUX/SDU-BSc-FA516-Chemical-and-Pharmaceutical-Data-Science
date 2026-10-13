# Track 4: Statistical Learning

How the FA516 course predicts a measured property from a structure: a model that maps
descriptors to a number, fitted by least squares, judged on molecules it has never seen,
and extended from one descriptor to several and from straight lines to curves, until it
starts learning the noise.

Every model is fitted with SciPy and scored with error measures you write yourself.
scikit-learn arrives in track 5, once you know what it does for you.

Assumes tracks 1 to 3.

## Topics

- **Linear regression**: what a regression model is and why it is judged on held-out molecules, fitting a straight line, R-squared, error measures and residuals, where a straight line goes wrong, fitting a dose-response curve (optional)
- **Multiple & polynomial regression**: several descriptors at once, reading the coefficients, curved relationships and polynomial features, overfitting, modelling the logarithm of a property (optional)

## The Two Classes

| Class | Covers |
|---|---|
| [1](class/) | Linear regression with [SciPy](https://scipy.org/): fitting a straight line, judging the fit and seeing where it goes wrong |
| [2](class/) | Multiple and polynomial regression, reading the coefficients, and overfitting |

## Material
Video lectures for [FA516 Track 4: Statistical Learning](https://www.youtube.com/playlist?list=PLGWXuesSP4Gs) are available online.

For each video there is a short exercise in `prepare/`.

**NB: Not ready yet** For each 2 h class there is a worksheet in `class/`
