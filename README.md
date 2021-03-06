# SharkTraits
Resources for collaborators and data contributors to SharkTraits. This repositoty contains a [data entry template](https://github.com/creeas/SharkTraits/blob/master/SharkTraits-Template.xlsx) and protocol for data collection. To get involved or for any questions regarding data assignments, the resource database, or data template and protocol please contact the [SharkTraits Administrators](mailto:sharktraits@gmail.com).

# Overview

The Shark Traits Database is an open source research initiative that aims to make all observations and measurements of chondrichthyans (sharks, rays, and chimaeras) accessible in order to more rapidly advance resesearch. The framework behind the database is heavily based on the open source [Coral Trait Database](https://www.coraltraits.org). Anyone collecting chondrichthyan life history data can join and contribute to the growing data compilation. Contributors have control over the privacy of their data and greatly benefit from being able to download complementary public data from the database in a standard format for use in their analyses. We hope that private data will become public once the contributor has published them, which will subsequently be cited when their data are used in analyses by other people. The citation system has been carefully designed to ensure full transparency about the origin of each individual data point as well as larger data compilations of other peoples' data (such as data extracted from literature for meta-analyses).

***

## Mission

- Assemble disparate information on life history traits of sharks, rays, and chimaeras
- Provide unrestricted, open-source and easy access to shark trait data
- Avoid redundant data gathering efforts
- Facilitate and encourage the appropriate crediting of original data sources
- Engage the shark and ray research community in the collection and quality control of trait data
- Facilitate reproducible science
- Do the above with a sustainable future for the database in mind, in terms of management and longevity

*[Top](#top)*

***

## Governance

#### Administrator

Contact the Administrators for any information about the database.

- [sharktraits@gmail.com](mailto:sharktraits@gmail.com)

***

## Trait Classes and Traits

The database was designed to contain `population-level` characteristic measurements, which are trait estimates of a species at a given location. These traits are grouped into six use-classes: 

- [Length](#length)
- [Age](#age) 
- [Growth](#growth)
- [Reproduction](#reproduction)
- [Demography](#demography) 
- [Relationships](#relationships) (conversions between different units, such as length to weight)

#### Observations and measurements of traits

Observations bind related trait measurements of the same population. For example, estimates of age at maturity for males and females of the same population results in one observation with two measurements (each corresponding with a different trait of the population).

`Observation-level` data include the chondrichthyan species, location and resource (i.e. reference). These data are the same for all measurements corresponding to the observation. When entering or importing trait data, the following is minimally required:

  - Contributor
  - Access (public or private)
  - Species<sup>1</sup>
  - Location<sup>2</sup>
  - Resource<sup>3</sup>

<sup>1</sup>All observations must be associated with a valid species name. We are using the taxonomy of [Weigmann 2016](https://onlinelibrary.wiley.com/doi/full/10.1111/jfb.12874). Note that this taxonomy does not currently include all the taxonomic nomenclatrual revisions in [Naylor et al 2016](https://www.researchgate.net/publication/311043124_The_Rays_of_the_World_project_-_an_explanation_of_nomenclatural_decisions). The list of valid species names is built in to the spreadsheet template and can be accessed as a dropdown menu. First select the appropriate `species_superorder` (Chimaeriformes, Batoidea, Squalimoroh Sharks, or Galeomorph Sharks) and a reduced taxa set to select from will be provided in the `species_name` column.

<sup>2</sup>Location information can be entered in several formats/columns: (1) `marine_province` is restricted to the desingated [marine longhurst provinces](http://www.marineregions.org/gazetteer.php?p=image&pic=64934), (2) `location_name` is for general locations provided in the study methods (e.g. Southern Calfifornia Bight, Northern Gulf of Mexico), and (3) `lat` and `long` coordinates if provided.

<sup>3</sup> The resource ID should be taken from the unique ID found in the [references database](https://sharktraits-refs.shinyapps.io/shark-resources/). This is a shiny database that contains all materials compiled on [Shark-Refences](https://shark-references.com/).You can filter the reference databse by year and/or search for author, keyword, species, journal, etc. Resource can be left blank for unpublished data, but data must be kept private.

`Measurement-level` data include the sex, trait, value, standard (unit), methodology, estimates of precision (if applicable), and model used. When entering or importing trait data, the following is minimally required:

  - Sex
  - Trait
  - Value
  - Standard

The current list of traits is as follows:

#### Length

A trait should always have a Standard and a Method. In cases where there are multiple models that could be fitted in a method, there should be a Model specified as well. 

Trait                      | Description
---------------------------|:------------------------------------------------------------------------------------------------------
L<sub>mat50</sub>          | Length at 50% maturity
L<sub>mat95</sub>          | Length at 95% maturity
Length at first maturity   | Length at first maturity based on gonadal observation (production of gametes) or clasper calcification
Length of largest immature |
Lenght at maternity        | Age at first observation of pregnancy
L<sub>max</sub>-observed   | Maximum observed length
L<sub>max</sub>-estimated  | Maximum length estimated from model
L<sub>birth</sub>          | Length at birth
 
 Standards | Description
-----------|:---------------
 cm TL     | Total length in centimetres
 cm FL     | Fork length in centimetres
 cm DW     | Disc Width in centimetres
 cm CL     | Chimaera length in centimeters
 cm PCL    | Pre-caudal length length in centimetres
 cm BDL    | Body length length in centimetres
 cm PSCFL  | Pre-supra-caudal fin length in centimetres

Methods                                            | Description
---------------------------------------------------|:---------------------------------------------------------------------------------------
Back-calculated                                    | Estimated from a model output (Model should be specified)
Direcetly observed                                 | 
Histologically                                     |
Macro-dissection                                   |
Smallest free-swimming individual                  |
Largest Embryo                                     |
Free + Embryo                                      | Based on combined observations of largest embryo and smallest free-swimming individual
Embryo growth curve                                | Estimated from a model output (Model should be specified)
L<sub>95</sub>                                     | 95th percentile of observed size distribution
L<sub>99</sub>                                     | 99th percentile of observed size distribution
Max observed size                                  |
Inverse mortality                                  | Estimated from a model parameter (Model should be specified)

Models                       | Description
-----------------------------|:---------------
Back-calculated              |
Directly from growth curves  |
Observational                |
Logistic                     |

[Trait Classes](#trait-classes-and-traits)


### Age


Trait                           | Description
--------------------------------|:----------------------------------------------------------------------------------------------------
A<sub>mat50</sub>               | Age at 50% maturity
A<sub>mat95</sub>               | Age at 95% maturity
Age at first maturity           | Age at first maturity based on gonadal observation (production of gametes) or clasper calcification             
Age of largest immature         |                                    
Age at maternity                | Age at first observation of pregnancy                                   
A<sub>max</sub>-observed        | Maximum observed age
A<sub>max</sub>-estimated       | Maximum age estimated from model
                       

Standards | Description
----------|:---------------
Year      | 

Methods                                            | Description
---------------------------------------------------|:----------------------------------------------------------------------------------------
Back-calculated                                    | Estimated from a model output (Model should be specified)
Direcetly observed                                 |
Histologically                                     |
Macro-dissection                                   |
Smallest free-swimming individual                  |
Largest Embryo                                     |
Free + Embryo                                      | Based on combined observations of largest embryo and smallest free-swimming individual
Embryo growth curve                                |
L<sub>95</sub>                                     | 95th percentile of observed size distribution
L<sub>99</sub>                                     | 99th percentile of observed size distribution
Max observed size                                  |
Inverse mortality                                  | 
Mark-recapture                                     | From mark-recapture data

Models                       | Description
-----------------------------|:---------------
Back-calculated              |
Directly from growth curves  |
Observational                |
Logistic                     |

[Trait Classes](#trait-classes-and-traits)

### Growth

Given that this trait class deals with model outputs, there is only a single placeholder Standard as the units of each Trait are implicit.


Trait            | Description
---------------- | :---------------------------------------------
*k*                | von Bertalanffy growth parameter
L<sub>inf</sub>             | von Bertalanffy asymptotic size parameter
L<sub>0</sub>               | von Bertalanffy length-at-age zero parameter
*t*<sub>0</sub>               | von Bertalanffy age-at-length zero parameter
*t*<sub>1</sub>               | Lester model
T<sub>mat</sub>             | Lester model
H                | Lester model
G                | Lester model
sigma-growth     | error estimate of the growth model
cv_readers       | Coefficient of variation between readers
APE              |
PA               | Percent agreement between readers


Standards     | Description
--------------|:--------------------------------------------------------------
Coefficient   | Coefficient value from model output (Model must be specified)


Method           | Description
-----------------| :---------------------------------------------
Mark-recapture   |
Length-frequency |
Vertebrae        |
Spines           |
Tooth Plates     |
Direct Age       | Estimates from individuals of known ages
Captive          | Data from captive individuals
                 


Model                  | Description
-----------------------| :---------------------------------------------------------------------------------------------------------
VBFG2 Strong Bayes     | Bayesian implementation of 2 parameter von Bertalanffy growth curve with strong priors
VBFG2 Uninformed Bayes | Bayesian implementation of 2 parameter von Bertalanffy growth curve with weak/unifmormative priors
VBFG2 ML               | Maximum Liklihood implementation of 2 parameter von Bertalanffy growth curve
VBFG3 Strong Bayes     | Bayesian implementation of 3 parameter von Bertalanffy growth curve with strong priors
VBFG3 Uninformed Bayes | Bayesian implementation of 3 parameter von Bertalanffy growth curve with weak/unifmormative priors
VBFG3 ML               | Maximum Liklihood implementation of 2 parameter von Bertalanffy growth curve
Gomp Strong Bayes      | Bayesian implementation of Gompertz growth curve with strong priors
Gomp Uninformed Bayes  | Bayesian implementation of Gompertz growth curve with weak/unifmormative priors
Gomp ML                | Maximum Liklihood implementation of Gompertz growth curve
Fabens                 |
Francis                |
Other                  |

[Trait Classes](#trait-classes-and-traits)


### Reproduction


Trait                      | Description
---------------------------|:---------------------------------------------------------------------------------------------------------
Ovarian fecundity          | Maximum number of visible ovarian follicles (generally used in egg-laying species (e.g. skates))
Uterine fecundity          | Max number of visible ovultaed eggs or developing embryos in both embryos
Annual reproductive output | 
Litter size (unspecified)  | Number of ova or developing embryos
Breeding                   | Observed timing of mating
Ovulation                  | Observed timing of ovulation
Parturition                | Observed timing of parutrition
Incubation length          | 
Gestation length           |
Breeding interval          | Biannual, Annual, Biennial, Triennial
Ovum size                  | Maximum observed ova diamter (uterine or recently ovulated)
Offspring mass             |
Max oviducal width         |
Max uterine width          |
Single uterus              | Yes/No
Seasonal                   | Yes/No
Peak parturition           |
Embryonic sex ratio        | In utero ratio of Males:Females within a litter


Standard      | Description
------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------
Number        | Number
mm            | millimetres
g             | grams
Month         | Number of months for length traits (e.g. Incubation or Gestation Length) or Calendar month for phenological traits (e.g. breeding, ovulation, parturition)
Year          | Years for breeding interval (0.5 for biannual, 1 for annual, 2 for biennial, 3 for triennial)
Logical       | Yes/No traits


Method                    | Description
--------------------------| :------------------------------------------------------------------------------------------
Captive Observation       | Observations from captive individuals
Modeled                   | Estmimated from model output (Model must be specified)
Proportion Gravid Females | 
Macroscopic observation   | Observation through macroscopic dissection or observation of free swimming individuals

[Trait Classes](#trait-classes-and-traits)

### Demography


Trait                      | Description
-------------------------- | :---------------------------------------------
Natural mortality          | *M* 
Total mortality            | *Z*  
Fishing mortality          | *F*  
r<sub>max</sub>            | Maximum intrinsic rate of population increase
&#955;                  | Population growth rate 


Standards     | Description
--------------|:---------------
Coefficient   | 


Method        | Description
------------- | :------------------------------------------------------------------------------------------------------------------------
Empirical     | Estimated directly from abundance/catch data (e.g. stock assessments, catch curves)
Derived       | Estimated indirectly from life history traits (e.g. Hoenig 1983, Chen and Watanabe 1983 mortality estimators)

[Trait Classes](#trait-classes-and-traits)

### Relationships

The Relationships Trait Class is a somewhat "catch-all" category that encompasses any time of conversion equations between different types of data, such as length to length conversions (e.g. fork length to total length), and length to weight conversions. The parameters *a* and *b* are the most commonly used ones and represent the coefficients on the typical conversion equations of the form ![basic equation](https://latex.codecogs.com/gif.latex?y%20%3D%20a*x%5Eb). The parameters *c* and *d* will probably be seldom used, but are presented in case a conversion equation has more than two coefficients.


Trait                      | Description
---------------------------|:------------------------------------------------------------
a                          | Multiplier of the equation (intercept if in log scale) 
b                          | Exponent of the equation (coefficient if in log scale) 
c                          | 
d                          | 
sigma-conv                 | Error term of the equation 


Standards     | Description
--------------|:---------------
Coefficient   | 

Model         | Description
--------------|:------------------------------
Length-Length | Length to length conversion
Length-Weight | Length to weight conversion

[Trait Classes](#trait-classes-and-traits)

## Data submission

> The Shark Traits Database is a research tool, not a meta-data catalog.

**A meta-data repository captures `dataset-level` information** about your data set, so that people can easily find it. Examples of meta-data repositories include DRYAD, Ecological Archives and Figshare. You are encouraged to submit data sets to meta-data repositories to help ensure their longevity and the reproducibility of the results for which the data were originally collected.

**The Shark Traits Database captures `data-level` information** so that measurements from multiple data sets can be integrated, extracted, compared and analyzed. 

> One way to think about The Shark Traits Database is as a very large data-set being cobbled together by the elasmobranch community for everyone to use, avoiding redundant efforts, identifying knowledge gaps, informing management, and speeding up science.

#### What information can be contributed

The database currently accepts -level measurements of chondrichthyans. Data must be associated with a species name (i.e., not genus- or family-level data) and public data must be associated with a published resource (e.g., paper, monograph, technical report, or book).

Data accepted:

- Species-level model-derived data that has been published
- Species-level expert or group opinion data that has been published
- Unpublished data if kept private until published

Data not accepted:

- Future predictions
- Data for other taxonomic resolutions (e.g., genus or family).

Unpublished data can also be imported into the database if it is kept private. Private data can be made public once associated with a published resource. Benefits of accepting unpublished data include:

- Being able to easily download the data alongside useful public data for analysis
- Being more likely to contribute the data at end of project and improve its longevity
- Identify duplicate research efforts

To contribute data, you need to email the database [Administrator](mailto:sharktraits@gmail.com) to become a contributor.

> Having a primary, peer-reviewed resource is essential for maintaining data quality, contributor recognition and scientific rigor.

#### Importing a spreadsheet

Even if only entering small amounts of data, the spreadsheet submission process is recommended. We have developed a fillable template which can be accessed [here](https://github.com/creeas/SharkTraits/blob/master/SharkTraits-Template.xlsx). A spreadsheet import is the fastest way to get data into the database. The import function accepts csv-formatted spreadsheets and runs a number of tests to make sure your data fit the database correctly (note that you can export csv-formatted files from Excel using "Save as..."). Any errors will reject the entire import and the system will attempt to tell you where the errors occur, so you can fix these errors and try the import again.

The spreadsheet you import must have a header with *at least* the following column names:

    observation_id, access, user_id, resource_id, species_name, location_id, trait_name, standard_name, methodology_name, value, value_type, precision, precision_type, precision_upper, sample_size, notes

`species_id`, `trait_id`, `method_id`, and `model_id` can be included instead of `species_name`, `trait_name`, `method_name`, and `model_name`, respectively (or you can include both ids and names). Having the names can be useful for navigating large spreadsheets. **These names must exactly reflect the names in the database**, so it is best to copy and paste names directly from the database.

`resource_id` is reserved for the original data resource (i.e., the paper that reports the original collection of the measurement). You can credit papers that compiled large datasets from the literature by adding a column named `resource_secondary_id`. `resource_id` and `resource_secondary_id` may be substituted with `resource_doi` and `resource_secondary_doi`, respectively (the doi should start with "10.", not "doi:"). The resource will automatically be added using Crossref if the doi is not already in the database.

We have collated all the references from [shark-references.com](https://sharktraits-refs.shinyapps.io/shark-resources/) and generated a unique `resource_id` for each reference, so the easiest way to populate this field is by searching for the `resource_id` in the reference list provided.

`user_id` must by your own database user id (i.e., you cannot import data for other people). You can find your user id by clicking on your name in the top right corner and selecting "My Observations".

Copy and paste the above header into a text file and save as `import_trait_author_year.csv`, where author and year correspond with the resource (paper). Alternatively, download a [CSV](/import_template_author_year.csv) or [Excel](/import_template_author_year.xlsx) template.

#### Observation-level data

The first six required columns are associated with the observation.

`observation_id` is an unique integer that groups a set of measurements into one observation. In the example below, the first two rows belong to the same observation of a shark.

`access` is a boolean value indicating if the observation should be accessible (0 denotes private and 1 denotes public). In the example below, the data are public.

`user_id` is the unique ID (name or integer) of the person entering the data. 

`species_name` and/or  `species_id` is the unique name or ID of the species of which the observation was taken. IDs occur in grey to the left of [species](/species) or at the top of a given species' observation page.

`marine_province` is the large marine regions (e.g. longhurst province) where the study was conducted. You can see a global map of provinces and associated names here []()

`location_id` is the unique ID of the location where the observation took place.<!--The location_id 374 in the example is [Turneffe Atoll, Belize](/locations/374).-->

`resource_id` is the unique ID of the resource (paper) where the observation was published. `resource_id` can be empty for unpublished data, in which case `access` must be private (0) until the data are published and the published resource is entered. In the example the resource_id 606 is [Gleason et al. (2009)](/resources/606).


#### Measurement-level data

The remaining columns are associated with measurement-level data. All measurements corresponding to the same observation should have exactly the same observation-level data. 

> **Warning** All measurements corresponding to the same observation should have exactly the same observation-level data. Use copy and paste or fill down to avoid making errors.

`trait_name` and/or `trait_id` is the unique name or ID (integer) of the species-level characteristic that was measured. 

`standard_name` is the unique ID of the standard (measurement unit) that was used to measure the trait. 

`method_name` is the unique ID of the methodology used to measure the trait. 

`model_name` is the unique name of the model being used for the given methodology to measure the trait.

`value` is the actual measured value (number, text, true/false, etc.). If the value is an option of a categorical trait (e.g., growth form), then the value must exactly match the value options for the trait (e.g., massive).

`value_type` describes the type of value. Current options are: 

- `raw_value` for a direct measurement, 
- `mean` if the value represents the mean of more than one value, 
- `median` if the value represents the median of more than one value, 
- `maximum` if the value represents the maximum of more than one value, 
- `minimum` if the value represents the minimum of more than one value, 
- `model_derived` if the value is derived from a model, 
- `expert_opinion` if the actual value has not been measured directly, but an expert feels confident of the value, perhaps based on phylogenetic relatedness or an indirect observation, 
- `group_opinion` if the actual value has not been measured directly, but a group of experts feel confident of the value. 

`precision` is the level of uncertainty associated with the value if it is made up from more than one measurement (e.g., mean). 

`precision_type` is the kind of uncertainty that the precision estimate (above) corresponds with. Current options are:

- `standard_error`
- `standard_deviation`
- `95_ci` 
- `range` 

`precision_upper` is used to capture the maximum (upper) value if range is used (above). 

`sample_size` is the number of data points that were used to calculate the value. Leave this field blank if equal to one (e.g., a raw_value). 


Optional fields include:

`notes` is an optional field for reporting useful information about how the measurement was made.

`dubious` is a optional boolean field noting whether the data being reported is classified as dubious (1) or not (0 or blank) by the user entering the data.

`validated` is a boolean field to be used only for Growth Trait Class measurements, indicating whether any validation of the growth model has been attempted (1) or not (0).

`validation_type` denotes the method used for validating the growth model. At the moment, this is a text field with pre-determined values. 

#### Back-end imports

If your data is well-managed, you can ask a [database programmer](mailto:sharktraits@gmail.com) to upload it for you. The data will be associated with your name and made private. You are required to make the data public yourself (if desired).

#### Submitting data from papers

Entering published data not already in the database in strongly encouraged to improve the data's longevity and augment data analysis. A case in which this might occur is a meta-analysis. The data enterer can keep the data they submit private until their study is published.

> The key objective is to extract data from resources in such a way as to avoid people ever needing to go back to the that resource again.

For example, extracting only the mean value of a trait measurement from a paper, without extracting any measure of variation or the context in which the trait was measured, will mean that the data may not be useful for other purposes. Someone else might need to go back and extract the information again, and there is a chance your initial efforts won't be cited.

- **Primary resources only.** Often people enter data from summary tables in papers that come from other (primary) resources. It is important to enter the data from the primary resource for two reasons: (1) so that the primary resource's author is credited for their work, and (2) to avoid data duplication, where the same data are entered from both the primary and secondary resource. Secondary resources, such as meta-analyses, can be credited for large data compilations.

- **Careful extraction.** Copy values from tables carefully and double check. Extracting data from figures can be done with software like ImageJ or DataThief, where a scale can be set based on axis values and measurements of plotted data made, including error bars.

<!--
- **Gather important context.** Enter contextual data as well, which might require reading the methods. This might be as simple as the time of year or depth or habitat in which animals were collected, and potentially the same for all observations. Such information is very useful. However, contextual information can get complicated quickly. Please contact the database [Administrator](mailto:sharktraits@gmail.com) if you have any questions.
-->

#### Quality control

There are three levels of data review.

1. `Contributor-level` review at time of submission,  Once submitted, data are tagged as *pending*.
2. `Editor-level` review. The relevant Editor/s for traits in your submission are automatically notified by email. The contributor may be contacted by the Editor if there are any issues with the submission. The Editor will *approve* the submission once satisfied.
3. `User-level` review. Anyone signed-in as a database user can report an issue with an observation record, and the submitter and the Editor will be notified by email.

#### Error checking

Basic error checking will ensure data submissions fit into the database. Error checking will improve as different issues arise. Measurement records with the same species, location, resource and value will be flagged as potential duplicates.

*[Top](#top)*

***

