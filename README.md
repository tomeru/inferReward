# inferReward

this README refers to probabilistic programming model for an infant development experiment 
run by Shari Liu, Tomer Ullman, Josh Tenenbaum & Elizabeth Spelke. 

## Prerequisites

You will need the following things properly installed on your computer:

* [webchurch](https://github.com/probmods/webchurch)


## Installation

```bash
git clone https://github.com/tomeru/inferReward.git
```

##  Running the model

The main model is found in rewardInference.txt ; the code there can be directly pasted into a
browser implementation of Church, such as in [probmods.org](https://probmods.org).

However, it is advised to reduce the number of mh-samples if using a browser, as inference
can take several minutes and cause the browser to crash.

To run the code locally, navigate to your webchurch installiation and run:

```bash
church rewardInference.txt
```

### Output

If (infer-agent-reward) is commented in: the output will be a list of pairs of samples from 
the posterior probability P(Reward(Blue) | Familiarization Action) & P(Reward(Yellow) | Familiarization Action). 
"Blue" is a stand-in for the agent that the Protagonist in the experiment exerted more effort to reach. 

If (predict-agent-action) is commented in: the output will be a list of pairs of actions, 
sampled from the predicted probability distribution P(Action | Inferred Rewards). 
Pairs are used as the test stimuli involved pairs of actions. 

### Visualization

The raw output can be visualized and analyzed in different ways. 

We provide a Python implementation using Seaborn. This code assumes you have run rewardInference and
saved the appropriate output. 






