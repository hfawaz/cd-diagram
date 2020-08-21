# Critical Difference Diagrams 
This repository contains the necessary code to generate a critical difference diagram based on the Wilcoxon-Holm method to detect pairwise significance. 

## Result 
By running the ```python3 main.py``` you will generate a critical difference diagram with Wilcoxon-Holm post-hoc analysis for the data present in the [example.csv](https://github.com/hfawaz/cd-diagram/blob/master/example.csv) file.
![cd-diagram-example](https://github.com/hfawaz/cd-diagram/blob/master/cd-diagram.png)
First the Friedman test is performed to reject the null hypothesis, we then proceed with a post-hoc analysis based on the Wilcoxon-Holm method. 
We can clearly see how on average ```clf3``` and ```clf5``` were the best algorithms over the 15 datasets. 
A thick horizontal line groups a set of classifiers that are not significantly different. 

## Relevant projects
### Deep learning for time series classification: a review 
In this [paper](https://arxiv.org/abs/1809.04356v3) we used the critical difference diagram to compare the recent deep learning models for time series classification where we evaluated 9 different architectures on 85 different datasets from the [UCR/UEA archive](https://www.cs.ucr.edu/~eamonn/time_series_data/). 

Check out the [code](https://github.com/hfawaz/dl-4-tsc)!

### Deep Neural Network Ensembles for Time Series Classification
In this [paper](https://arxiv.org/abs/1903.06602) we used the critical difference diagram to show how ensembling hybrid architectures will allow deep learning models to reach even better accuracy when evaluated on 85 different datasets from the [UCR/UEA archive](https://www.cs.ucr.edu/~eamonn/time_series_data/).

Check out the [code](https://github.com/hfawaz/ijcnn19ensemble)!

## Requirements
To run this code you will need the following python packages: 
* [numpy](https://www.numpy.org/)
* [pandas](https://pandas.pydata.org/)
* [matplotlib](https://matplotlib.org/)
* [scipy](https://www.scipy.org/)
* [networkx](https://networkx.github.io/)

## Reference 

If you re-use this work, please cite:

```
@article{IsmailFawaz2018deep,
  Title                    = {Deep learning for time series classification: a review},
  Author                   = {Ismail Fawaz, Hassan and Forestier, Germain and Weber, Jonathan and Idoumghar, Lhassane and Muller, Pierre-Alain},
  journal                  = {Data Mining and Knowledge Discovery},
  Year                     = {2019},
  volume                   = {33},
  number                   = {4},
  pages                    = {917--963},
}
```
