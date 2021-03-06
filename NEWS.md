# dendroTools 1.0.7.
* Bootstrapping is now available for all metrics, monthly and daily functions
* Seacorr is now available also for monthly data, including bootstrapping
* swit272 daily precipitation dataset is added
* swit272 monthly temperature dataset is removed
* KNMI_daily_transform() is now called data_transform(). The entire function is updated and now also enables transformation of daily data into monthly.

# dendroTools 1.0.6.
* Bootstrapping of correlation coefficients is introduced. To do so, use the argument boot in daily_response() and monthly_response(). Bootstrapping is currently available only for correlation coefficients. In future version, it will also be available for model fitting. 
* Package version is changed to 1.0.6

# dendroTools 1.0.5.
* new function: monthly_response_seascorr()
* titles of plot_extreme, plot_specific and plot_heatmap are updated
* for daily_response() and monthly_response(), it is now possible to define method for correlation coefficient: "pearson", "kendall", "spearman". To do so, use , cor_method argument
* daily_response output list is class "dmrs"
* Using newly defined class "dmrs", new summary function is defined
* Package version is changed to 1.0.5

# dendroTools 1.0.4.
* New data is available for examples demonstration: swit272_monthly_temperatures
* New function is available: daily_response_seascorr(). This function implements partial correlations in the analysis of daily response functions
* Package version is changed to 1.0.4

# dendroTools 1.0.3.
* Package version is changed to 1.0.3
* There is new function introduced: KNMI_daily_transform() which transforms daily data obtained from KNMI Climate explorer into data frame suitable for daily_response(). 
* New TRW chronology is included, swit272
* New function: monthly_response()
* New data: LJ_monthly_temperatures
* New data: LJ_monthly_precipitation

# dendroTools 1.0.2.
* Package version is changed to 1.0.2
* There have been many issues with RWeka package, which depends on rJava. Therefore, functions from RWeka are replaced with other functions. For random forest model we now use randomForest package
* There are six new output elements, all of them are residual diagnostic plots for calibration, holdout and edge data.
* Due to many problems related to rJava in R, MT and BMT methods from RWeka are now joined and replaced by cubist function from Cubist r package. Cubist fits a model tree or ensemble of model trees, if committees argument is more than 1.
