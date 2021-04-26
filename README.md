# SyntheticData
a draft for a CRAN task view on Synthetic Data

**Maintainer:** Bruno A Lima                                  
**Contact:**    balima78 at gmail.com                      
**Version:**    2021-04-26                                     
**URL:**        *no link to CRAN*   

<div>

Testing and validating applications or data products requires the use of data that is not always available to us. 
As an alternative to real data, we have the possibility to generate fake or synthetic data in a format similar to real data. This task view collects information on R packages wich include functionalities to generate synthetic data.

[Wikipedia](https://en.wikipedia.org/wiki/Synthetic_data) defines synthetic data as follows: Synthetic data is "any production data applicable to a given situation that are not obtained by direct measurement" according to the McGraw-Hill Dictionary of Scientific and Technical Terms; where Craig S. Mullins, an expert in data management, defines production data as "information that is persistently stored and used by professionals to conduct business processes."

Base **R** allow us to genetare data vectors according to different distributions 
with functions as: `rnorm`, `rexp`, `rpois`, `runif`, `rmultinom`, `sample`...

Also, we can access to several *packages* deployed to generate synthetic data. 

**Builders**

- [charlatan](https://github.com/ropensci/charlatan) - Makes fake data; inspired from and borrowing some code from Python's faker
- [conjurer](https://www.foyi.co.nz/posts/documentation/documentationconjurer/) -Builds synthetic data applicable across multiple domains. This package also provides flexibility to control data distribution to make it relevant to many industry examples as described in the [vignette](https://cran.r-project.org/web/packages/conjurer/vignettes/introduction_to_conjurer.html).
- [datasynthR](https://github.com/jknowles/datasynthR) - Functions to procedurally generate synthetic data in R for testing and collaboration. Allows the user to generate data of known distributional properties with known correlation structures. This is useful for testing statistical model data, building functions to operate on very large datasets, or training others in using R!
- [fabricatr](https://github.com/DeclareDesign/fabricatr) - This package helps researchers imagine what data will look like before they collect it. Researchers can evaluate alternative analysis strategies, find the best one given how the data will look, and precommit before looking at the realized data.
- [fakeR](https://cran.r-project.org/web/packages/fakeR/vignettes/my-vignette.html) - Simulates Data from a Data Frame of Different Variable Types. Generates fake data from a dataset of different variable types. The package contains the functions simulate_dataset and simulate_dataset_ts to simulate time-independent and time-dependent data. It randomly samples character and factor variables from contingency tables and numeric and ordered factors from a multivariate normal distribution. It currently supports the simulation of stationary and zero-inflated count time series.
- [humanleague](https://github.com/virgesmith/humanleague): Synthetic Population Generator. An R package for microsynthesising populations from marginal and (optionally) seed data. 
- [OpenSDPsynthR](https://github.com/opensdp/OpenSDPsynthR) - Generate synthetic education data that is realistic for use by analysts across the education sector. Synthetic data should be able to be generated on-demand and responsive to inputs from the user.
- [sdglinkage](https://rdrr.io/cran/sdglinkage/) - Synthetic Data Generation for Linkage Methods Development. A tool for synthetic data generation that can be used for linkage method development, with elements of i) gold standard file with complete and accurate information and ii) linkage files that are corrupted as we often see in raw dataset.
- [SimMultiCorrData](https://github.com/AFialkowski/SimMultiCorrData) - The goal of SimMultiCorrData is to generate continuous (normal or non-normal), binary, ordinal, and count (Poisson or Negative Binomial) variables with a specified correlation matrix. It can also produce a single continuous variable. This package can be used to simulate data sets that mimic real-world situations (i.e. clinical data sets, plasmodes, as in Vaughan et al., 2009).
- [simstudy](https://cran.r-project.org/web/packages/simstudy/vignettes/simstudy.html) - This package has a collection of functions that allow users to generate simulated data sets in order to explore modeling techniques or better understand data generating processes.
- [synthpop](https://www.synthpop.org.uk/index.html) - This package for R allows users to create synthetic versions of confidential individual-level data for use by researchers interested in making inferences about the population that the data represent. It allows the synthesis process to be customised in many different ways according to the characteristics of the data being synthesised.
- [wakefield](https://github.com/trinker/wakefield) - A pckage designed to quickly generate random data sets. The user passes `n` (number of rows) and predefined vectors to the `r_data_frame` function to produce a `dplyr::tbl_df` object.

**Specific types of data**

- [survsim](https://www.jstatsoft.org/article/view/v059i02) - Simulation of Simple and Complex Survival Data. Simulation of simple and complex survival data including recurrent and multiple events and competing risks.
- [sim.survdata()](https://cran.r-project.org/web/packages/coxed/vignettes/simulating_survival_data.html) function allows to generate a survival dataset. This function belongs to the [coxed](https://github.com/jkropko/coxed) package.
- [synthesis](https://github.com/zejiang-unsw/synthesis#readme) - Synthetic data generator. Generate synthetic time series from commonly used statistical models, including linear, nonlinear and chaotic systems.

**Datasets**

- [rcorpora](https://github.com/gaborcsardi/rcorpora) - A collection of small text corpora of interesting data. Some examples: names of animals: birds, dinosaurs, dogs; foods: beer categories, pizza toppings; geography: English towns, rivers, oceans; humans: authors, US presidents, occupations; science: elements, planets; words: adjectives, verbs, proverbs, US president quotes.
- [NHSRdatasets](https://cran.r-project.org/web/packages/NHSRdatasets/index.html) - Free United Kingdom National Health Service (NHS) and other healthcare, or population health-related data for education and training purposes. This package contains synthetic data based on real healthcare datasets, or cuts of open-licenced official data.
- [fakir](https://thinkr-open.github.io/fakir/) - The goal of {fakir} is to provide fake datasets that can be used to teach R.

**Miscellaneous**

- [bindata](http://finzi.psych.upenn.edu/library/bindata/html/00Index.html) - Generation of correlated artificial binary data.
- [GenOrd](https://rdrr.io/cran/GenOrd/#vignettes) - Simulation of Discrete Random Variables with Given Correlation Matrix and Marginal Distributions. A gaussian copula based procedure for generating samples from discrete random variables with prescribed correlation matrix and marginal distributions.
- [MultiOrd](https://www.tandfonline.com/doi/abs/10.1080/03610918.2013.824097?journalCode=lssp20) - An R Package for Generating Correlated Ordinal Data.
- [PoisBinOrdNonNor](https://onlinelibrary.wiley.com/doi/abs/10.1002/sim.5362) - Generation of a chosen number of count, binary, ordinal, and continuous random variables, with specified correlations and marginal properties.
- [sgr](https://cran.r-project.org/web/packages/sgr/sgr.pdf) - Sample Generation by Replacement simulations. The package can be used to perform fake data analysis according to the sample generation by replacement approach. It includes functions for making simple inferences about discrete/ordinal fake data. The package allows to study the implications of fake data for empirical results.
- [SynthTools](https://github.com/RTIInternational/SynthTools) - Tools and Tests for Experiments with Partially Synthetic Data Sets. A set of functions to support experimentation in the utility of partially synthetic data sets. All functions compare an observed data set to one or a set of partially synthetic data sets derived from the observed data to (1) check that data sets have identical attributes, (2) calculate overall and specific variable perturbation rates, (3) check for potential logical inconsistencies, and (4) calculate confidence intervals and standard errors of desired variables in multiple imputed data sets. Confidence interval and standard error formulas have options for either synthetic data sets or multiple imputed data sets.
- [WikidataR](https://cran.r-project.org/web/packages/WikidataR/vignettes/Introduction.html) - the API client library for Wikidata.

**Key references**

</div>

### CRAN packages:

- [bindata](https://cran.r-project.org/web/packages/bindata/index.html)
- [charlatan](https://cran.r-project.org/web/packages/charlatan/index.html)
- [conjurer](https://cran.r-project.org/web/packages/conjurer/index.html)
- [coxed](https://cran.r-project.org/web/packages/coxed/index.html)
- [fabricatr](https://cran.r-project.org/web/packages/fabricatr/index.html)
- [fakeR](https://cran.r-project.org/web/packages/fakeR/index.html)
- [GenOrd](https://cran.r-project.org/web/packages/GenOrd/index.html)
- [humanleague](https://cran.r-project.org/web/packages/humanleague/index.html)
- [MultiOrd](https://cran.r-project.org/web/packages/MultiOrd/index.html)
- [NHSRdatasets](https://cran.r-project.org/web/packages/NHSRdatasets/index.html)
- [PoisBinOrdNonNor](https://cran.r-project.org/web/packages/PoisBinOrdNonNor/index.html)
- [psychmeta](https://cran.r-project.org/web/packages/psychmeta/index.html)
- [rcorpora](https://cran.r-project.org/web/packages/rcorpora/index.html)
- [sdglinkage](https://cran.r-project.org/web/packages/sdglinkage/index.html)
- [sgr](https://cran.r-project.org/web/packages/sgr/index.html)
- [SimMultiCorrData](https://cran.r-project.org/web/packages/SimMultiCorrData/index.html)
- [simstudy](https://cran.r-project.org/web/packages/simstudy/index.html)
- [synthesis](https://cran.r-project.org/web/packages/synthesis/index.html)
- [synthpop](https://cran.r-project.org/web/packages/synthpop/index.html)
- [SynthTools](https://cran.r-project.org/web/packages/SynthTools/index.html)
- [wakefield](https://cran.r-project.org/web/packages/wakefield/index.html)
- [WikidataR](https://cran.r-project.org/web/packages/WikidataR/index.html)

- []()
- []()
- []()
- []()
- []()


### Related links:

-   [CRAN Task Views](https://cran.r-project.org/web/views/)
-   [How to write CRAN TAsk Views](https://cran.r-project.org/web/packages/ctv/vignettes/ctv-howto.pdf)
-   [CRAN Task View: Missing Data](https://cran.r-project.org/web/views/MissingData.html)
-   [GitHub repository for this Task
    View](https://github.com/balima78/SyntheticData)