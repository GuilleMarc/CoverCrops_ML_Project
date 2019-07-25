**Cover crops** are species known to improve soil and water quality relative to
a bare-ground if planted after or along with commercial crops. The success of
a cover crop depends however on good establishment and healthy growth during and 
after the winter months. If early on the season growers could anticipate how much 
growth they expect from the cover crop, late field operations can be scheduled 
more effectively (e.g. termination of the cover crop, harvesting or planting 
the next cash crop, etc.). **Statistical learning (~ Machine Learning)**, 
built upon statistical and computational algorithms to "learn" from data may help to 
accurately predict cover crop biomass and shoot-N contents across N limited 
environments based on early-season field information.

This repository features an end-to-end Machine learning project where two supervised
regression based algorithms were trained, optimized, and validated on a set of remote
sensing and field observed allometric features of winter-seeded rye grown at different 
N rates in the Mid-Atlantic US. Random Forests capture additional information gains of
data-splitting strategies, such as those in decision trees, and add statistical power via
resampling and bagging. LASSO (Least Absolute Shrinkage and Selection Operators), in turn,
penalizes long and likely overfitting models, such as multiple regression on highly
collinear datasets, and help balancing accurate but otherwise unstable models (i.e. 
low bias- high variance models).

The notebook summarizes the full data analysis process,
from exploratory checks, to feature selection and creation, up to model training
and validation. Lastly, a final test on unseen data revealed the potential of modern
intensive approaches to characterize end-season preformance of winter cover crops and
small grains alike, and may be adapted to data-oriented support tools that optimize farm 
decision making.

X= Selected features from a three-year study on rye adaptation at 
   different fall-spring N rate applications (MD, PA). 
   Common to each, features recorded or created* at stages GS20, and GS30: 
   remote sensed NDVI, C and N shoot-contents, C/N-ratios*, early-season biomass, 
   tiller-counts, tiller-efficiency relative to seeding rate*, NUE relative to groundbase soil N*.
   `Files (.csv): data_25, data_30`
   
   In addition, a third independent dataset (NC) used for model testing includes features
   available at GS30. It is included in `data_30.csv`
  
y= Dry-weight biomass (Kg.ha), Shoot-Nitrogen content (Kg.ha), recorded at GS60
   `colnames in above files: ["biomass_60_y"],["shoot_n_kg_ha_60_y"]`

## Additional resources:

- To learn more about the integration of digital and data-driven solutions for sustainable
  and profitable agriculture, please visit:

Precision Sustainable Agriculture
- [https://precisionsustainableag.org]

Goatech (Gathering for open Agricultural Technology)
A very cool group of folks who advocate open source hardware and software to meet, learn, share, 
and establish a common vision for creating technologies for our food system)
- [http://goatech.org/]

Sustainable Agricultural Systems Laboratory: Beltsville, MD (USDA-ARS)
- [https://www.ars.usda.gov/people-locations/person?person-id=42691]


- To learn more about current and historical impact of cover crops on US corn and other systems:
- [http://www.jswconline.org.proxy.lib.iastate.edu/content/72/3/226.full.pdf]
- [http://miguezlab.agron.iastate.edu/OldWebsite/Research/CoverCrops/WCC_MetaA.pdf]
- [https://practicalfarmers.org/]



