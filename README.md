# covid-19_priority_measures_japan

## Table of contents
* [Overview of this repository](#overview-of-this-repository)
* [Overview of priority measures such as the prevention of the spread of disease in Japan](#overview-of-priority-measures-such-as-the-prevention-of-the-spread-of-disease-in-japan)
* [Description of files](#description-of-files)
* [Description of columns in `covid-19_priority_measures_japan.csv`](#description-of-columns-in-covid-19_priority_measures_japancsv)
* [Data source of `covid-19_priority_measures_japan.csv`](#data-source-of-covid-19_priority_measures_japancsv)
* [Citation](#citation)
* [Reference](#reference)


## Overview of this repository
Date-range data of the priority measures such as the prevention of the spread of disease for the prefectures in Japan. The priority measures in this dataset are those issued by the government of Japan and prefectural governments of Japan.

## Overview of priority measures such as the prevention of the spread of disease in Japan
Work in progress

## Description of files
* `covid-19_priority_measures_japan.csv`: data file of the priority measures issued by the government of Japan.
* `make_long_covid-19_priority_measures_japan.R`: An R script that converts the above file into a long format data frame represented by a binary variable that indicates under which priority measures was issued. This also supports multiple declarations of priority measures.


## Description of columns in `covid-19_priority_measures_japan.csv`
* `id`: ID assigned to prefectures in Japan in accordance with the JIS code (JIS X 0401).
* `prefecture_en`: Names of prefectures in Japan, in English.
* `priority_measures_start`: The date on which the Government of Japan declared priority measures for COVID-19 infection.
* `priority_measures_end`: The date on which the Government of Japan declared that the priority measures is over because it has recognized that it is no longer necessary to implement priority measures.
* `times`: Integer data indicating the number of times a priority measure was issued in the region.


## Data source of `covid-19_priority_measures_japan.csv`
* Declaration in 2021: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic policy for the control of novel coronavirus diesease. in Japanese. 2021/04/01. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210401.pdf. (Accessed on April 18, 2021).
  * 1st Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic policy for the control of novel coronavirus diesease. in Japanese. 2021/04/09. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210409.pdf. (Accessed on April 18, 2021).
  * 1st Amendment: Office for Novel Coronavirus Disease Control, Cabinet Secretariat, Government of Japan. Basic policy for the control of novel coronavirus diesease. in Japanese. 2021/04/16. URL: https://corona.go.jp/expert-meeting/pdf/kihon_h_20210416.pdf. (Accessed on April 18, 2021).


## Citation
Katafuchi, Y. (2021). covid-19_priority_measures_japan. URL: https://github.com/yuya-katafuchi/covid-19_priority_measures_japan.


## Reference
Work in progress