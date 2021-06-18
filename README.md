## Data Visualizaton

About Dataset

The dataset provided to us deals with cross platform(namely instagram and facebook) digital marketing campaigns with various attributes such as clicks ,ctr(click thhrough rate),cpm(click per millon),expenditure on these campaigns, impressions.

Methodology and considerations for analysis

The aim is to analyze the data thoroughly, we can check how the campaigns are performing on the basis of serveral attributes such as the spend on a specific campaign, clicks on the ad, impressions ,etc. General understanding of the digital marketing concepts will be used in understanding how successful an ad campaign has been, for eg-If we observe that an ad campaign is clicked multiple times , it will be a succesful campaign.
Anlysis will be done with the help of various packages provided in Python like seaborn,matplotlib,numpy,pandas, wherein we will use various visualization concept to gain indepth insights on the data to come up with a plausible conclusion.

Flow of analysis

The data provided is loaded on the system and it is checked for any inconsistency ( presence of NAN values, outliers)
NAN values are checked with the help of heatmap and outliers are checked with the help of a box plot.

After checking for the inconsistency, the data is checked for different sort of features, namely
Numerical Features
Categorical Features
Temporal Featutes(Date-Time Variables)
It is necessary to scan the data for the same, since the analysis run on different type of features are unique

Coming to the initial step,a pairplot is drawn between different numerical features on the basis of different platforms chosen for the analysis, namely-Instagram and Facebook, and some initial conclusions could be drawn from the plot
The plot between clicks and impression was observed to be exponential for Instagram and linear for Facebook



