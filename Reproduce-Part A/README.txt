README file for data associated with the article: "Long-term and year-to-year stability and its drivers in a Mediterranean grassland"


DATASET DESCRIPTION

The dataset contains the data from a 14-year study of a species-rich semi-natural Mediterranean grassland, as analysed in the published article "Long-term and year-to-year stability and its drivers in a Mediterranean grassland". We studied the relative importance of richness, synchrony, species stability and functional traits on community stability. We also applied a fertilization treatment to assess land-use change effects on stability. Finally, we distinguished stability patterns produced by year-to-year fluctuations from those caused by long-term trends.


Data consist of an excel file containing the data used in the analyses and a group of R scripts showing the main statistical analyses carried out in the study.


Each sheet from excel file shows the following:
	
- "boxplotindices": data used to carry out the analyses shown in "models_boxplots.R". Columns show: the number of the plot or community (12 plots), stability, synchrony and richness values for each plot or community, the approach used to calculate each index (long-term or year-to-year), and the treatment applied in each plot (control or fertilized).Rows show each of the communities or plots studied.
	
- "matrixalldatacom": data used to carry out the analyses at the community level shown in "models_stability_communitylevel.R" and "SEMs.R". Columns show: the number of the plot or community (12 plots), stability, synchrony, richness, functional composition (Community Weighted Mean) and diversity (Rao) of the five traits studied (plant height, Leaf Dry Matter Content, Specific Leaf Area, Leaf Area, Seed Mass), and treatment (control or fertilized).For each of these variables there are two columns, one with the variable calculated using the long-term approach (in this case the variable name starts with "longterm_" or with "cum_") and the other one for the variable calculated using the year-to-year approach (in this case the variable name starts with "yeartoyear_" or "mean_").Rows show each of the communities or plots studied.

- "matrixalldataspp": data used to carry out the analyses at the species level shown in "models_stability_splevel.R" and "spstability.R". Columns show species name, long-term species stability, year-to-year species stability, species values for plant height, Leaf Dry Matter Content (LDMC), Specific Leaf Area (SLA), Leaf Area (LA) and Seed Mass (SM), and treatment (control or fertilized). Rows show each of the species studied. Missing values are indicated by NAs.


Each script shows the following:

- "indicescom.R": calculation of richness, synchrony and stability indices at the community level.

- "functionalindicescom.R": calculation of functional composition (Community Weighted Mean) and diversity (Rao) for the five traits studied (plant height, Leaf Dry Matter Content, Specific Leaf Area, Leaf Area, Seed Mass), at the community level.

- "spstabilityindices.R": calculation of stability indices at the species level. 
	
- "models_boxplots.R": multiple linear regression models analysing the relationship between richness, synchrony or stability values and the approach used (long-term or year-to-year), treatment (control or fertilized) and the interaction between approach and treatment.
	
- "models_stability_communitylevel.R": simple and multiple linear regression models analysing the effect of richness, synchrony, treatment (control and fertilized), functional composition (as Community Weighted Mean) and functional diversity (as Rao) of plant height, Leaf Dry Matter Content (LDMC), Specific Leaf Area (SLA), Leaf Area (LA) and Seed Mass (SM).
	
- "SEMs.R": Piecewise Structural Equation Models showing the relationships between stability, synchrony, richness, treatment (control or fertilized) and the functional composition (Community Weighted Mean) and diversity (Rao) of the traits that were significantly related to stability in simple regressions (Seed Mass and Specific Leaf Area). One SEM was carried out for the long-term approach and other for the year-to-year approach.
	
- "models_stability_splevel.R": simple and multiple linear regression models analysing the effect of functional traits such as plant height, Leaf Dry Matter Content (LDMC), Specific Leaf Area (SLA), Leaf Area (LA) and Seed Mass (SM), on long-term and year-to-year species stability (log transformed). Multiple regression models had as explanatory variables the traits selected as significant or marginally significant in simple regression models, treatment (control and fertilized), and the interaction between trait and treatment.
	
- "spstability.R": Pearson's correlations and paired t-tests showing the effects of treatment and long-term trends on species stability (log transformed).
	

