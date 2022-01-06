# Factor Coding （質的変数のコーディング方法）

Rを使い質的変数（主に名義尺度）をコーディングして統計モデリングを行うための，Schad et al (2020)に対する日本語注解

Schad, D. J., Vasishth, S., Hohenstein, S., & Kliegl, R. (2020). How to capitalize on a priori contrasts in linear (mixed) models: A tutorial. *Journal of Memory and Language*. https://doi.org/10.1016/j.jml.2019.104038

本注釈資料は，下記の統計教科書の各章もカバーしている

1. Vasishth, S., Schad, D., Bürki, A., & Kliegl, R. (In preparation). [*Contrast coding*](https://vasishth.github.io/Freq_CogSci/basic-concepts-illustrated-using-a-two-level-factor.html). In Vasishth, S., Schad, D., Bürki, A., & Kliegl, R. (Eds.), Linear Mixed Models in Linguistics and Psychology: A Comprehensive Introduction. https://vasishth.github.io/Freq_CogSci/basic-concepts-illustrated-using-a-two-level-factor.html
2. Nicenboim, B., Schad, D., and Vasishth, S. (In preparation). [*Contrast coding*](https://vasishth.github.io/bayescogsci/book/ch-contr.html). In Nicenboim, B., Schad, D., and Vasishth, S. (Eds.), An Introduction to Bayesian Data Analysis for Cognitive Science. https://vasishth.github.io/bayescogsci/book/ch-contr.html

## この資料と原著論文との違い

- [`flipbookr`](https://cran.r-project.org/web/packages/flipbookr/index.html)を使い，順を追ってコードを提示した点
  - 資料を読むだけでも，各コマンドでどのような処理が行われているのか追うことができる
  - とりわけ，パイプ処理の各段階でどのような処理がなされているのか把握できる
- [Tidyverseスタイルガイド](https://style.tidyverse.org/)に沿うことで、より効果的で、よりシームレスで、より理解しやすいコードに改めた点
  - 原著論文のコードを [`tidyverse`](https://www.tidyverse.org/) の関数と [ネイティブパイプ `|>`](https://stat.ethz.ch/pipermail/r-announce/2021/000670.html#:~:text=the%20new%20native%20pipe%20operator%20%22%7C%3E%22) を使い書き直した
- 日本語で書かれている点
  - 英語以外の言語による，原著論文への最初の注釈

