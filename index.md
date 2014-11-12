---
title       : Institutional Implications for Revenue Choice
subtitle    : An Analysis of Fiscal Behavior in Colorado
author      : Marvin Ward Jr., Congressional Budget Office
job         : Analyst
framework   : io2012        # {io2012, html5slides, shower, dzslides, ...}
highlighter : highlight.js  # {highlight.js, prettify, highlight}
hitheme     : tomorrow      # 
widgets     : []            # {mathjax, quiz, bootstrap}
mode        : selfcontained # {standalone, draft}

---
  
## Do Tax and Expenditure Limitations Strengthen Fiscal Federalism?
  
  **Spoiler:** This study does not provide the answer ... but it does explore the foundation.

Before knowing whether TELs align the actions of elected officials and voter preferences, it would be helpful to know what voter preferences are.

1. Can baseline exemption propensity be predicted via socioeconomic characteristics?
2. What is the marginal impact of ballot design?

$$latex
f(x;\mu,\sigma^2) = \frac{1}{\sigma\sqrt{2\pi}} 
e^{ -\frac{1}{2}\left(\frac{x-\mu}{\sigma}\right)^2 }
$$
  
  


---
  
## What Do TELs Look Like in Colorado?
  
+ Taxpayer's Bill of Rights (TABOR)
+ Voter approval required for tax increases;
+ Limit on the annual growth in revenue;
+ Creates obstacles for modification of existing limits; and,
+ Permits local overrides (i.e. DeBrucing).
+ Gallagher Amendment (GA)
+ Holds constant the statewide residential share of property assessment value.
+ Statewide Limit on Property Tax Revenue (SLPTR)
+ Restricts annual growth in property tax revenue to 5.5%.

---

## Finances of General Purpose Jurisdictions in Colorado

!['CO_fin']('CO_gen_juris_fin.png')

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

---

## Can Exemption Be Predicted with Socioeconomic Indicators?
# Data (1993-2009)

USA Counties Database
+ 521 variables
+ Data capture demographics, income, political attitudes, industrial base
+ Irregular reporting frequency across variables

Colorado Counties, Inc.
+ Ballot-level indicators (e.g. requested property tax rate increase)
+ 527 votes


---

## Can Exemption Be Predicted with Socioeconomic Indicators?
# Approach

What's Wrong with Logistic Regression?

!['logit'](http://upload.wikimedia.org/wikipedia/commons/thumb/8/88/Logistic-curve.svg/320px-Logistic-curve.svg.png)

The Logistic Function 

What are Support Vector Machines?

---
  
## Can Exemption Be Predicted with Socioeconomic Indicators?
# Performance
  
  Classification Accuracy = 58.3%

Probabilities were recoverable via Platt Scaling.

---
  
## What Role Does Ballot Design Play?
  
Operationalizing Ballots
+ Revenue Source
+ Expenditure Target
+ Scope of Change

Additional Variables of Interest
+ Propensity to Exempt
+ TABOR/SLPTR Constraint
+ Gallagher Ratio

---
  
## Results
