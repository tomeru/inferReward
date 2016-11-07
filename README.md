# inferReward

This README outlines the details of a probabilistic programming model for an infant development experiment 
run by Shari Liu, Tomer Ullman and Elizabeth Spelke. 

## Prerequisites

You will need the following things properly installed on your computer.

* [webchurch](https://github.com/probmods/webchurch)


## Installation

```bash
git clone https://github.com/tomeru/inferReward.git

###  Running the model

The main model is found in rewardInference.txt ; the code there can be directly pasted into a
browser implementation of Church, such as in [probmods.org](https://probmods.org).

However, it is advised to reduce the number of mh-samples if using a browser, as inference
can take several minutes and cause the browser to crash.

To run the code locally, navigate to your webchurch installiation and run:

* church rewardInference.txt




