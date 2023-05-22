# ML_COMP

## Kaggle Link :

https://www.kaggle.com/antoinegoubert/ml-comp

### Data Import and Transformation

ExpectedDividend's NaN can be replaced by 0's. 

When the traded volume of the day is 0 ; Open, High, Low and Close are empty. Every NaN value of 'Target' is included in those rows. Should we just drop them ? Is there a better way to fill at least Open, High, Low and Close and then only drop 238 rows ?

Use secondary_stock_prices.csv and/or options.csv to train the model ?

Can we use the other csv files ?

Drop Date/SecuritiesCode/RowId ?


### Different ideas for data augmentation (not everything needs to be implemented) :

https://arxiv.org/pdf/2206.13508.pdf

https://arxiv.org/pdf/1902.10755.pdf

- Stock^X, X!=0
- f(Stock) with f non-linear
- 2*Max(Stock)-Stock
- 2*(Max(Stock)-Stock)
- X*Stock, X>0
- Integral(Stock) from t=-X to t=0, X>0
- Noise introduction (Gaussian error term)
- Flipping
- Time translation
- Permutation of series slices
- Stretch/Compress time-wise
- Fourier transform

### Use generators instead of the entire dataframe at once.

### Baseline Model
Some ideas to improve on the model :

- https://paperswithcode.com/paper/self-distillation-for-gaussian-process
- https://paperswithcode.com/paper/delay-sde-net-a-deep-learning-approach-for
- https://paperswithcode.com/paper/variational-operator-learning-a-unified
- https://paperswithcode.com/paper/enhancing-safe-exploration-using-safety-state
- Model focused Curriculum Learning
- Attention Mechanism
- More layers (Dropout, Conv, ...)
