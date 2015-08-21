# Possible Titles
- Multiple estimates of latent demand using survey data
- Appliance acquisition after electricity provision

# Abstract


# Introduction

- **global topic**
- global electricity access is poor
- many areas require private capital to install electricity
- part of problem is upfront investment cost
- due to perceived business risk, upfront capital is costly (citation)
- **oversizing**
- oversized microgrids based on overestimated demand that cannot meet
    revenue targets contribute to this perception
- Schnitzer has shown the consequences of generators with excess
    capacity on microgrid operation
    - EPP thesis work chapter three
- to lower this cost, accurate demand estimation is necessary
- estimating demand in areas without access is challenging
- through more accurate appliance estimation, we may achieve more
    accurate energy estimation
- with more accurate energy estimation, a micro-utility can reduce
    the variance in revenue
- reductions in revenue variance should lead to lower-cost capital
- **study detail**
- this study aims to improve bottom up models in rural areas for
    households
- data set with similar communities with and without access
- survey taken to understand electricity demands and interests
- do you currently own appliance X?
- if electricity available, will you buy appliance X?
- we demonstrate several approaches to estimating eventual ownership
- **related work**
- Wolfram et al have used an econometric approach to predict the
    appliance acquisition as communities encounter wealth
- Jay Taneja IBM Nairobi paper shows district based approach to village
    pairing strategy


# Method

<!-- TODO: look through summer 2014 notes for appliance schnitzer notes -->
- survey supplied by collaborators from AE and Cenderwash University
- survey designed by AE
- data collected by CU students
- data collected and hosted online
- data collected in a single tabular store for analysis
- N = 1184


## Assumptions
- We do not have random sampling
- We do not consider economic effects since we don't observe significant
    income variations in connected areas
- Electricity won't significantly influence disposable income
- Households dominate microgrid energy and power demands


## Appliance ownership

<!-- TODO: create notebooks that have these sections in them -->
- We observe the overall reported percentage of each appliance (fig or
    table)
- We then split the dataset and assign each village to an access type
    (grid, microgrid, no central access)
- We observe the reported percentage of appliance in each type
- fig label appliance_ownership_by_access_type


## Current Appliance Ownership

- We can also categorize the appliances by energy use per day
- We don't expect to find high energy use appliances in areas without
    central access
- Show bar chart with numbers


## Surveyed Appliance Desire

- approach one: for low access areas, add the population currently
    owning appliances and add the population that doesn't own one but
    claims that they will buy
- We look at households that don't currently own an appliance and
    compute the percentage that state desire to buy that appliance
- This should be relatively constant over access types but our data do
    not show that
- Show bar chart with numbers
- label: appliance_desire_to_buy_by_access_type


## Electrified estimate of appliance ownership

- approach two: match villages by other characteristics and find the
    levels of appliance ownership in the connected villages most like
    the unconnected villages.  (we focus on high consumption
    appliances.)  this requires a set of matching criteria.  first
    strategy is to find factors that reduce the variance in ownership
    stats
- Based on the stated desire of survey responses, we can estimate the
    eventual number of appliance owners by appliance category
- estimate increased appliance purchases
- estimate resulting increase in energy usage
- compare results from approaches
- label: appliance_ownership_desire_comparison


## Probability distributions

- approach three: create probability distributions by treating as an
    ensemble of bernoulli probabilities.  you can then create a
    distribution of energy consumptions.
- this allows us to move beyond a point estimate


# Results

- Quantify levels of generator usage observed in no access regions
- TV and lighting above X% in all areas with little variation
- television ownership observed in locations without electricity
    - plot of TV ownership overall, and by access type
    - AE 1.01.10 is related
- Stated preferences for appliance purchases do not match current
    ownership levels in grid regions
- These provide some point estimates of eventual ownership levels


# Future work
- Understanding the amount of shared generation
- Understanding how TV is powered and the cost of that
- What is the least cost temporal provision of assets for these
    locations?  We borrow from the current utility planning literature.

    # Bibliography
- http://www.nber.org/papers/w17747.pdf wolfram how will energy demand
    develop
