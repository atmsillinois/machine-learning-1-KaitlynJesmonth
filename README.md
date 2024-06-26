# ATMS 523 Module-5

Several machine learning techniques including a multiple linear regression, a polynomial regression, and a random forest regressor were used in this module. The main goal was to get more experience with machine learning and to try and predict rainfall rate from several different polarimetric radar parameters. Several error statistics were calculated to determine which model performed the best, including a baseline model calculation which used the formula $Z = 200 R^{1.6}$.

## Setting Up
In order to complete this module in Python, [scikit-learn](https://scikit-learn.org/stable/) will be used. 

The package can be installed using [conda](https://docs.conda.io/projects/conda/en/latest/)
```
conda install -c conda-forge scikit-learn
```

## Demo the code
Run the `Module5.ipynb` file. The necessary dataset is already provided.

## Data
The `radar_parameters.csv` dataset is in the `homework` folder and will be used to train and test the models generated. These polarimetric radar parameters were calculated from disdrometer data in Huntsville, Alabama.

### Columns 

Features (radar measurements):

`Zh` - radar reflectivity factor (dBZ) - use the formula $dBZ = 10\log_{10}(Z)$

`Zdr` - differential reflectivity

`Ldr` - linear depolarization ratio

`Kdp` - specific differential phase

`Ah` - specific attenuation

`Adp` - differential attenuation

Target :

`R` - rain rate

## Key functionalities
- Multiple linear regression
- Polynomial regression with a grid search
- Random forest regressor with a grid and randomized search
- Baseline model calculation
- Calculation of r-squared and root mean square error statistics

## References and Acknowledgements
Scikit-learn: Machine Learning in Python, Pedregosa et al., JMLR 12, pp. 2825-2830, 2011.