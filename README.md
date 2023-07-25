# KeyGenes

[KeyGenes] ([Roost et al., 2015]) is an algorithm that uses the 
transcriptional profile of human fetal organs of different gestational ages as
well as adult tissues (training set) and can predict the identity of your
differentiated samples (test set), provided you input their transciptional
data. Keygenes will determines the identity scores of your queried samples
(test set) using the transcriptional profiles of the queried data (test set)
and matches them to sets of transcriptional profiles of the human organs or
cell types (training set). KeyGenes uses a 10-fold cross validation on the
basis of a LASSO (Least Absolute Shrinkage and Selection Operator) regression
available in the R package “glmnet” ([Friedman et al., 2010]).

## WebApp
The keygenes algorithm can be run online through the keygenes website:
[http://keygenes.nl/tool](http://keygenes.nl/tool).

## Installation
The package can be installed using the following commands in R:

```R
library(devtools)
install_github("chuvalab/KeyGenes")
```

## Usage
Please see the [vignette].

## References

Roost, M. S., van Iperen, L., Ariyurek, Y., Buermans, H. P., Arindrarto, W.,
Devalla, H. D., Passier, R., Mummery, C. L., Carlotti, F., de Koning, E. J. P.,
van Zwet, E. W., Goeman, J. J., & Chuva de Sousa Lopes, S. M. (2015). KeyGenes, a
Tool to Probe Tissue Differentiation Using a Human Fetal Transcriptional Atlas. In
Stem Cell Reports (Vol. 4, Issue 6, pp. 1112–1124). Elsevier BV.
[https://doi.org/10.1016/j.stemcr.2015.05.002][Roost et al., 2015]

Friedman, J., Hastie, T., & Tibshirani, R. (2010). Regularization Paths for
Generalized Linear Models via Coordinate Descent. In Journal of Statistical
Software (Vol. 33, Issue 1). Foundation for Open Access Statistic.
[https://doi.org/10.18637/jss.v033.i01][Friedman et al., 2010]

[KeyGenes]: http://keygenes.nl/
[vignette]: https://chuvalab.github.io/KeyGenes/v2.0.0.html
[Roost et al., 2015]: https://doi.org/10.1016/j.stemcr.2015.05.002
[Friedman et al., 2010]: https://doi.org/10.18637/jss.v033.i01