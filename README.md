# Upper Confidence Bound (UCB) in Reinforcement Learning

The Upper Confidence Bound (UCB) algorithm is commonly employed in the context of multi-armed bandit problems, which are a type of reinforcement learning scenario. In a multi-armed bandit problem, an agent needs to make decisions (take actions) to maximize cumulative rewards while dealing with uncertainty about the rewards associated with different options (arms).

## UCB Formula

The UCB algorithm tackles the exploration-exploitation trade-off by assigning an upper confidence bound to each arm's estimated reward. The UCB formula is typically expressed as:

\[ \text{UCB}_t(i) = \bar{X}_i + c \sqrt{\frac{\ln(t)}{N_i}} \]

Where:
- \(\text{UCB}_t(i)\) is the upper confidence bound for arm \(i\) at time \(t\),
- \(\bar{X}_i\) is the average reward of arm \(i\) up to time \(t\),
- \(N_i\) is the number of times arm \(i\) has been selected up to time \(t\),
- \(c\) is a parameter controlling the exploration-exploitation trade-off, and
- \(\ln(t)\) is the natural logarithm of \(t\), the total number of time steps.

## Usage in Reinforcement Learning

In reinforcement learning, UCB serves as a strategy for balancing exploration and exploitation in a sequential decision-making process. The agent uses the upper confidence bounds to decide which action to take at each time step, aiming to gain information about uncertain actions while also exploiting actions with potentially high rewards.

Feel free to use or modify this information as needed for your own projects or documentation.
