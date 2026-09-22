# Was It the Car or the Driver?
Separating car performance from driver skill across F1 regulation changes
using an AKM-style two-way fixed effects model.

## Method
Qualifying lap times from five circuits (2018-2026), pulled via FastF1.
Driver movement between teams identifies 35 driver effects and 92
team-season car effects within a connected network. Corrections for
qualifying-segment track evolution and mixed wet/dry sessions are applied
before estimation.

## Reproducing this
1. `pip install -r requirements.txt`
2. Run `F1RegChanges.ipynb` top to bottom. Cached data in `data/` lets you
   skip re-pulling from the FastF1 API.

## Reference
Abowd, J.M., Kramarz, F., & Margolis, D.N. (1999). High Wage Workers and
High Wage Firms. Econometrica, 67(2), 251-333.
