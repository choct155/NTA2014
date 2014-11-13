---

title       : Institutional Implications for Revenue Choice
subtitle    : An Analysis of Fiscal Behavior in Colorado
author      : Marvin Ward Jr., Congressional Budget Office
job         : Analyst
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : [mathjax]            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}

---
<style>

.title-slide {
  background-color: #331FA3;
  color: #FFFFFF ; 
}

.title-slide hgroup > h1{
 background-image: url('https://github.com/choct155/CBO_Talk/blob/master/TEL_intensity_2009.png');
 font-family: 'Oswald', 'Helvetica', sanserif;
 color: #FFFFFF ; 
}

.title-slide hgroup > h1, 
.title-slide hgroup > h2 {
  background-image: url('https://github.com/choct155/CBO_Talk/blob/master/TEL_intensity_2009.png');
  color: #FFFFFF ;  
}

article p, article li, article li.build, section p, section li{
  font-family: 'Open Sans','Helvetica', 'Crimson Text', 'Garamond',  'Palatino', sans-serif;
  text-align: justify;
  font-size:22px;
  line-height: 1.5em;
  color: #444444;
}

slide:not(.segue) h2{
  font-family: 'Calibri', Arial, sans-serif;
  font-size: 52px;
  font-style: normal;
  font-weight: bold;
  text-transform: normal;
  letter-spacing: -2px;
  line-height: 1.2em;
  color: #331FA3;
}
</style>

## The Congressional Budget Office...

### ... has nothing to with this.

<br>

Any implications, opinions, or findings conveyed in this presentation are the author's, and the author's alone.  Not only does CBO not vouch for these findings, they barely condone me talking about them.

<br>

Official Disclaimer: The views expressed in this paper are the author's and should not be interpreted as CBO's.
==================== 



---

## Do Tax and Expenditure Limitations Strengthen Fiscal Federalism?

<br>
**Spoiler:** This study does not provide the answer ... but it does explore the foundation.
==========

<br>

Before knowing whether TELs align the actions of elected officials and voter preferences, it would be helpful to know what voter preferences are.  Voter preferences can be partially revealed by understanding "de-Brucing."

1. Can baseline exemption propensity be predicted via socioeconomic characteristics?
2. What is the marginal impact of ballot design?
  
  


--- &twocol

## What Do TELs Look Like in Colorado?

*** =left
  
### Taxpayer's Bill of Rights (TABOR)
  + Voter approval required for tax increases;
  + Limit on the annual growth in revenue;
  + Creates obstacles for modification of existing limits; and,
  + Permits local overrides (i.e. DeBrucing).
  
### Gallagher Amendment (GA)
  + Holds constant the statewide residential share of property assessment value.
  
### Statewide Limit on Property Tax Revenue (SLPTR)
  + Restricts annual growth in property tax revenue to 5.5%.
  
*** =right

<div style='text-align: center;'>
  <img width='500' src=https://raw.githubusercontent.com/choct155/CBO_Talk/master/TEL_intensity_2009.png />
</div>

--- &twocol

## Finances of General Purpose Jurisdictions in Colorado

*** =left
<div style='text-align: center;'>
  <img width='400' src=https://raw.githubusercontent.com/choct155/NTA2014/master/CO_gen_juris_fin.png />
</div>

*** =right
+ Property taxes are predominately levied by counties
+ Taxes are the dominant revenue source for GPJs
+ Counties play a major role in the delivery of direct services


---

## Do TELs Alter Fiscal Behavior?

+ TELs are often passed with the voter assumption that service delivery need not change (Cutler, Elmendorf, Zeckhauser 1997)
+ TELs reduce growth in tax revenue (Mullins & Joyce 1996)
+ Recent literature increasingly affirms this result (Ballal & Rubenstein 2009)
+ TELs increase reliance on miscellaneous revenue sources (Shadbegian 1999)
+ TELs increase reliance on state aid (Skidmore 1999)
+ TELs exacerbate fiscal stress during recessions (Cutler, Elmendorf, Zeckhauser 1997)
+ TELs reduce local spending (Bails & Tieslau 2000)
+ TEL constraints are more binding on less affluent communities (Mullins 2004)

--- &twocol

## Can Exemption Be Predicted with Socioeconomic Indicators?

# Data (1993-2009)

*** =left

### USA Counties Database
+ 521 variables
+ Data capture demographics, income, political attitudes, industrial base
+ Irregular reporting frequency across variables

*** =right
### Colorado Counties, Inc.
+ Ballot-level indicators (e.g. requested property tax rate increase)
+ 527 votes


--- &twocol

## Can Exemption Be Predicted with Socioeconomic Indicators?
# Approach

*** =left

What's Wrong with Logistic Regression?

!['Logistic Function'](http://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Logistic-curve.svg/320px-Logistic-curve.svg.png)

+ Distrbutional Assumptions
+ Linear Separating Hyperplane
+ Overlapping Groups

*** =right 

What are [Support Vector Machines](https://www.youtube.com/watch?v=3liCbRZPrZA)?

<div style='text-align: center;'>
  <img width='400' src=http://upload.wikimedia.org/wikipedia/commons/1/1b/Kernel_Machine.png />
</div>

+ High-Dimensional Performance
+ Overlap Accommodation
+ Post Hoc Processing for Probability
+ "Macro"" Processing for Interpretation

---
  
## Can Exemption Be Predicted with Socioeconomic Indicators?
# Performance
  
  Classification Accuracy = 58.3%

Probabilities were recoverable via Platt Scaling.

<div style='text-align: center;'>
  <img width='800' src=https://raw.githubusercontent.com/choct155/NTA2014/master/vote_probs.png />
</div>


--- &twocol_right
  
## What Role Does Ballot Design Play?

*** =left

Operationalizing Ballots
+ Revenue Source
+ Expenditure Target
+ Scope of Change

Additional Variables of Interest
+ Propensity to Exempt
+ TABOR/SLPTR Constraint
+ Gallagher Ratio

*** =right

Why TEL Intensity and the Gallagher Ratio?

<div style='text-align: left;'>
  <img width='700' src=https://raw.githubusercontent.com/choct155/CBO_Talk/master/TABOR_vs_SLPTR.png />
</div>

<div style='text-align: left;'>
  <img width='700' src=https://raw.githubusercontent.com/choct155/CBO_Talk/master/gallagher_dist.png />
</div>


---
  
## Results

+ There is considerable overlap in the classifier results, but the regression output highlights largely
different aspects.

+ Proposals seeking to improve the function of government with commissions or studies
(administrative) adversely impact the likelihood of passage.

+ Proposals that do not extend spending authority (no waiver) are statistically significant across
models, but the signs of the effect differ across the classification and regression approaches.
+ The same could be said of restricting funding sources to non-property revenues
(ss_nonproperty).

+ Open ended spending targets (open) are clear drivers of the classification results, but figure only
modestly in the regression approach.
+ Changes to sales tax rates (sales_change) are consistently negative, but lack substantive
significance. The same could be said of public safety (public_safety) and changes to the
property tax rate (prop_change).

---

## Questions?

<div style='text-align: center;'>
  <img width='400' src=http://www.codeinstitute.net/wp-content/uploads/2014/10/python-logo.png />
  <img width='400' src=http://ipython.org/_images/9_home_fperez_prof_grants_1207-sloan-ipython_proposal_fig_ipython-notebook-specgram.png />
  <img width='300' src=http://scikit-learn.org/stable/_static/scikit-learn-logo-small.png />
  <img width='200' src=http://cran.us.r-project.org/Rlogo.jpg />
</div>
