# Delphi Case Study

## About Dataset

The dataset provided to us deals with cross platform(namely instagram and facebook) digital marketing campaigns with various attributes such as clicks ,ctr(click thhrough rate),cpm(click per millon),expenditure on these campaigns, impressions.

## Methodology and considerations for analysis

The aim is to analyze the data thoroughly, we can check how the campaigns are performing on the basis of serveral attributes such as the spend on a specific campaign, clicks on the ad, impressions ,etc. General understanding of the digital marketing concepts will be used in understanding how successful an ad campaign has been, for eg-If we observe that an ad campaign is clicked multiple times , it will be a succesful campaign.
Anlysis will be done with the help of various packages provided in Python like seaborn,matplotlib,numpy,pandas, wherein we will use various visualization concept to gain indepth insights on the data to come up with a plausible conclusion.

## Flow of analysis

The data provided is loaded on the system and it is checked for any inconsistency ( presence of NAN values, outliers)
NAN values are checked with the help of heatmap and outliers are checked with the help of a box plot.
![Screenshot (204)](https://user-images.githubusercontent.com/64247518/122635008-02f85880-d0ff-11eb-9106-c3319660ae78.png)
![Screenshot (212)](https://user-images.githubusercontent.com/64247518/122635257-76e73080-d100-11eb-90bb-fccadf3f820c.png)



After checking for the inconsistency, the data is checked for different sort of features, namely
Numerical Features
Categorical Features
Temporal Featutes(Date-Time Variables)
It is necessary to scan the data for the same, since the analysis run on different type of features are unique
![Screenshot (205)](https://user-images.githubusercontent.com/64247518/122635323-d5acaa00-d100-11eb-8f4d-71160127c6d2.png)
![Screenshot (206)](https://user-images.githubusercontent.com/64247518/122635326-d9d8c780-d100-11eb-8da6-d64945d68055.png)

Coming to the initial step,a pairplot is drawn between different numerical features on the basis of different platforms chosen for the analysis, namely-Instagram and Facebook, and some initial conclusions could be drawn from the plot
The plot between clicks and impression was observed to be exponential for Instagram and linear for Facebook

It is observed that there are 4 campaigns, unique clicks and spend with respect to these 4 different campaigns are plotted. It is observed that maximum and minimum expenditure have been done on campaign 1 and campaign 3 respectively, a similar trend is observed with respect to the number of unique clicks.
![Screenshot (207)](https://user-images.githubusercontent.com/64247518/122635329-e0ffd580-d100-11eb-97b1-d199921a3868.png)
![Screenshot (208)](https://user-images.githubusercontent.com/64247518/122635332-e2c99900-d100-11eb-88a7-49932e61460d.png)

In the next step we try to gather data on how much the numerical features are related to each other, it is carried out using a correlation heatmap, which makes it clear that the parameters spend and impressions are correlated,cpp and cpm are highly correlated. On the basis of this correlation statistics, we can choose which of the features are to be used for the analysis purpose. For example- Given that cpp and cpm are highly correlated we can neglect one of the paramters, since a change in one of the parameters would pan out an almost similar change in the other.
![Screenshot (209)](https://user-images.githubusercontent.com/64247518/122635335-e52bf300-d100-11eb-9e51-067bfbf1041f.png)

On reading the excel sheet of the csv file after sorting columns like campaign_name, we could understand that the flow of the ad campaign is from camapign->adset->ad, it was clearly evident that there were some adsets under the campign and further under the adsets there were ads.

To get a better insight of the data, the data was classified on a time line using the temporal(date-time) feature, namely(date_start) and it was tried to observe the number of clicks and individual campaign could get throught the duration of the camapign. It was observed that campign 1 got the maximum nuber of clicks throughout.

![Screenshot (211)](https://user-images.githubusercontent.com/64247518/122635338-e8bf7a00-d100-11eb-98a0-18a6c43c2821.png)
![n2](https://user-images.githubusercontent.com/64247518/122640331-a73cc800-d11c-11eb-8ae8-a117f2f5f74d.png)
![n1](https://user-images.githubusercontent.com/64247518/122640333-a9068b80-d11c-11eb-8527-cc0391cb90a0.png)


Some cross platfrom analysis was carried out to check how do the paramters vary depending on the platfrom, paramters like impressions and ctr were calculated for each platform.

![Screenshot (216)](https://user-images.githubusercontent.com/64247518/122635461-b7937980-d101-11eb-840b-9af755a95fb4.png)
![Screenshot (217)](https://user-images.githubusercontent.com/64247518/122635465-ba8e6a00-d101-11eb-8955-c7f88650f928.png)



Within different campaigns, there were different adsets and under every adset there was an ad , depending on the flow of data, plots were prepared to get a clear idea of how the ads are performing within an adset and how is that particular adset is performing under a campaign, various metric were considered such as ctr, spend, impressions.

### Campaign 1- Adset 1 Spend-Ctr Comaprison
![10](https://user-images.githubusercontent.com/64247518/122638241-b87fd780-d110-11eb-8456-816b2806ca88.png) ![3](https://user-images.githubusercontent.com/64247518/122638231-b61d7d80-d110-11eb-8a89-525d9f1d047d.png)
### Campaign 2- Adset 4 Spend-Ctr Comaprison
![11](https://user-images.githubusercontent.com/64247518/122638239-b87fd780-d110-11eb-8c97-e0d1a07d9db6.png) ![4](https://user-images.githubusercontent.com/64247518/122638230-b584e700-d110-11eb-99e7-c741fdf1b1a5.png)
### Campaign 2- Adset 3 Spend-Ctr Comaprison
![12](https://user-images.githubusercontent.com/64247518/122638237-b7e74100-d110-11eb-8264-632bd850b249.png) ![5](https://user-images.githubusercontent.com/64247518/122638229-b584e700-d110-11eb-9b6c-455553d9047c.png)
### Campaign 3- Adset 4 Spend-Ctr Comaprison
![13](https://user-images.githubusercontent.com/64247518/122638236-b74eaa80-d110-11eb-82eb-1ae7cdc6e235.png) ![6](https://user-images.githubusercontent.com/64247518/122638228-b4ec5080-d110-11eb-9b71-09d7f1f8e548.png)
### Campaign 3- Adset 2 Spend-Ctr Comaprison
![14](https://user-images.githubusercontent.com/64247518/122638235-b74eaa80-d110-11eb-8bc4-589c54cbf158.png) ![7](https://user-images.githubusercontent.com/64247518/122638227-b4ec5080-d110-11eb-8f30-fc6b0e33da78.png)
### Campaign 4- Adset 6 Spend-Ctr Comaprison
![8](https://user-images.githubusercontent.com/64247518/122638225-b3228d00-d110-11eb-81a1-863a60c5fdba.png) ![1](https://user-images.githubusercontent.com/64247518/122638234-b6b61400-d110-11eb-9ab8-1571b1e494cf.png)
### Campaign 4- Adset 5 Spend-Ctr Comaprison
![9](https://user-images.githubusercontent.com/64247518/122638244-b9186e00-d110-11eb-9212-ad6530ac1d6d.png) ![2](https://user-images.githubusercontent.com/64247518/122638232-b6b61400-d110-11eb-8085-9d1db2efd565.png)

## Conlusions and Suggestions

Analyzing the the datasets using the steps mentioned above, it can be concluded that 
 Campaign wise-
     The number of unique clicks is consistent with the the expenditure made on a campaign. Furthermore would like to point out that on reducing the spend beyond a threshold      value the clicks dropped at a faster pace as compared to the drop in expenditure, as observed with Campaign 2.
