# covid-19_priority_measures_japan

## Table of contents
* [Overview of this repository](#overview-of-this-repository)
* [Overview of priority measures such as the prevention of the spread of disease in Japan](#overview-of-priority-measures-such-as-the-prevention-of-the-spread-of-disease-in-japan)
* [Description of files](#description-of-files)
* [Description of columns in `covid-19_priority_measures_japan.csv`](#description-of-columns-in-covid-19_priority_measures_japancsv)
* [Data source of `covid-19_priority_measures_japan.csv`](#data-source-of-covid-19_priority_measures_japancsv)
* [Citation](#citation)
* [Reference](#reference)
* [Acknowledgement](#acknowledgement)


## Overview of this repository
Date-range data of the priority measures such as the prevention of the spread of disease (まん延防止等重点措置; _Manenboushitoujutensochi_, in Japanese) for the prefectures in Japan. The priority measures in this dataset are those issued by the government of Japan and prefectural governments of Japan.

## Overview of priority measures such as the prevention of the spread of disease in Japan
The priority measures such as the prevention of the spread of disease (まん延防止等重点措置; _Manenboushitoujutensochi_, in Japanese) by the Government of Japan are designed to limit the damage to the population caused by the spread of the pandemic and to prevent the spread of COVID-19 in certain areas with a negative impact on their life and economy.

This measure is based on the definition of Chapter 3 of the "Act on Special Measures for Pandemic Influenza and New Infectious Diseases Preparedness and Response", a law in Japan (e-Gov, Japan, 2020; Cabinet Secretariat, Japan, 2021a). and consists of the following requirements (Cabinet Secretariat, Japan, 2021b, 2021c, 2021d)

* Requests to restaurants and other businesses to shorten their opening hours
* Requests for restaurants to take thorough measures to avoid contact with the spread of the pandemic
* Requests to theatres, cinemas, department stores and other facilities to shorten their opening hours in order to reduce contact opportunities
* Requests to businesses to make use of telework and to promote the use of leave in order to reduce the need to attend work
* Requests to railway companies to reduce the number of trains on holidays on routes to and from the areas under the measures

As the priority measures under this law are issued by the government, which can limit the areas covered by these declarations more flexibly compared to emergency declarations ([Katafuchi, 2020](https://github.com/yuya-katafuchi/covid-19_emergency_statement_japan); Cabinet Secretariat, Japan, 2021b), their implementation varies from one region to another, especially at the prefectural level where they have been implemented. This repository consists of data constructed to capture this heterogeneity of priority measures at the prefectural level and to provide data-based analysis, as well as R code to support analysis using the data.

## Description of files
* `covid-19_priority_measures_japan.csv`: data file of the priority measures issued by the government of Japan.
* `make_long_covid19_priority_measures_japan.R`: An R script of function which converts the above file into a long format data frame represented by a binary variable that indicates under which priority measures was issued and times. This also supports multiple declarations of priority measures.


## Description of columns in `covid-19_priority_measures_japan.csv`
* `id`: ID assigned to prefectures in Japan in accordance with the JIS code (JIS X 0401).
* `prefecture_en`: Names of prefectures in Japan, in English.
* `priority_measures_start`: The date on which the Government of Japan declared priority measures for COVID-19 infection.
* `priority_measures_end`: The date on which the Government of Japan declared that the priority measures is over because it has recognized that it is no longer necessary to implement priority measures.
* `times`: Integer data indicating the number of times a priority measure was issued in the region.


## Data source of `covid-19_priority_measures_japan.csv`
* Declaration in 2021: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/04/01. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210401.pdf. (Accessed on April 18, 2021).
  * 1st Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/04/09. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210409.pdf. (Accessed on April 18, 2021).
  * 2nd Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/04/16. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210416.pdf. (Accessed on April 18, 2021).
  * 3rd Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/04/23. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210423.pdf. (Accessed on April 24, 2021).
  * 4th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/05/07. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210507.pdf. (Accessed on May 10, 2021).
  * 5th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/05/14. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210514.pdf. (Accessed on May 15, 2021).
  * 6th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/05/21. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210521.pdf. (Accessed on May 21, 2021).
  * 7th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/06/10. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210610.pdf. (Accessed on June 10, 2021).
  * 8th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/06/17. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210617.pdf. (Accessed on June 17, 2021).
  * 9th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/07/08. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210708.pdf. (Accessed on July 8, 2021).
  * 10th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/07/30. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210730.pdf. (Accessed on July 30, 2021).
  * 11th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/08/05. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210805.pdf. (Accessed on August 5, 2021).
  * 12th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/08/17. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210817.pdf. (Accessed on August 17, 2021).
  * 13th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/08/25. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210825.pdf. (Accessed on August 25, 2021).
  * 14th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/09/09. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210909.pdf. (Accessed on September 9, 2021).
  * 15th Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/09/28. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210928.pdf. (Accessed on September 28, 2021).
* Declaration in 2022: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2022/01/07. URL: https://corona.go.jp/expert-meeting/pdf/kihon_r_20220107.pdf. (Accessed on January 7, 2022).

## Citation
Katafuchi, Y. (2021). covid-19_priority_measures_japan. URL: https://github.com/yuya-katafuchi/covid-19_priority_measures_japan.


## Reference
* e-Gov, Japan. (2020). Act on Special Measures for Pandemic Influenza and New Infectious Diseases Preparedness and Response. in Japanese. URL: https://elaws.e-gov.go.jp/document?lawid=424AC0000000031. (Accessed on April 24, 2021).
* Cabinet Secretariat, Japan. (2021a). Public Notice on Priority Measures such as the Prevention of the Spread of Novel Coronavirus Disease. in Japanese. URL: https://corona.go.jp/emergency/pdf/kouji_20210401.pdf. (Accessed on April 24, 2021).
* Cabinet Secretariat, Japan. (2021b). Emergency Measures and Priority Measures such as the Prevention of the Spread of Disease. in Japanese. URL: https://corona.go.jp/emergency/pdf/kinkyujitaisochi_20210419.pdf. (Accessed on April 24, 2021).
* Cabinet Secretariat, Japan. (2021c). Measures to Strengthen Priority Measures such as the Prevention of the Spread of Disease. in Japanese. URL: https://corona.go.jp/emergency/pdf/manbou_kyokasaku_20210423.pdf. (Accessed on April 24, 2021).
* Cabinet Secretariat, Japan. (2021d). Basic Policy for the Control of Novel Coronavirus Disease. in Japanese. 2021/04/23. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210423.pdf. (Accessed on April 24, 2021).
* Katafuchi, Y. (2020). covid-19_emergency_statement_japan. URL: https://github.com/yuya-katafuchi/covid-19_emergency_statement_japan (Accessed on April 24, 2021).

## Acknowledgement
Development of this repository is supported in part by JSPS KAKENHI Grant Number 20K22142 and 21K13320.