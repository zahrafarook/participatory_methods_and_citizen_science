# participatory methods and citizen science

research on the citizen science (CNC/non-CNC) data.

## analysis and fitting distributions

1. The main idea behind fitting the temporal distribution of number of observations/identifications is to better understand the collective process of citizen science production of the content. E.g. similarly to what has been done here https://www.nature.com/articles/s41562-018-0474-5?fbclid=IwAR3z5oVNfbw-HSGrKKxCv1yJoPAEyVKTw7FZuMEV6IL-2x3-R5e3Pey2LZI and here https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0270131

The main hypothesis behind the temporal evolution of the collective total number of observations is based on what we see from data:

- collective number of observations has periodic pattern with varying amplitude from year to year,

- despite some obvious differences between number of observations each year (e.g. there are differences between number of observations during COVID years in 2020 or post COVID years like 2022 or 2023), there are however some universal patterns, which are repeating throughout years, which characterize how collective interest is distributed over time.

2. In order to be able to detect those universal patterns from year to year, we are fitting the data points into a smooth curve of the distributions (e.g.
the Gamma, Gumbel, Normal distributions). The idea behind fitting hence is that it is possible to compare two smooth curves between each other, rather than to compare the points (observations which may contain noise as well).

Each of these distributions will have goodness of fit (defined by specific parameters like squared error, see notebook I shared with you on fitting).

3. Since we clearly see the skewed distribution of the number of observations in time, most probably we dealt with the so-called  extreme-value statistics, which are two-parametric distributions (parameter of left slope is alpha, parameter of right slope is betta), described by parameters here https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.gumbel_r.html 
