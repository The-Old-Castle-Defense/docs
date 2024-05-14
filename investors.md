---
navigation:
   order: 5
---

# 📈 Investors

<p>Investors in The Old Castle Defense are users who stake **${token}** in one or both factions 
during the Siege. The Investor can participate in determining the outcome of the siege by contributing to one or 
both factions, helping them achieve victory.</p>

<div>
   
### If the Faction in which he staked wins, he receives:
* A reward from the treasury of the losing faction;
* All his **${token}** staked in the winning Faction.
</div>

Investors receive 70% of the treasury, while NFT holders receive 30% of the treasury.
</div>

<div>

### Available actions for Investors:
* Buying a Faction Attack;
* Reviving fallen NFT characters for either Faction;
* Boosting level up for any NFT.
</div>

<div>

Learn more about it:

<a href="game-fi-elements" 
 class="docs-item">
<span>🎯</span>
Game-Fi elements</a>
</div>

## Reward system

<div>

Investors can stake **${token}** in one Faction or both at once. But in each Siege, only one 
Faction wins. It should be noted that the Investor acts independently and receives 
remuneration depending on which faction, when, and how much **${token}** was staked.
</div>

::card_warning
The Investor receives a reward depending on the amount of **${token}** staked in the winning 
Faction. With each Battle, the "weight" of stakes decreases.
::

### The formula for calculating the weight of stakes

<div>

The weight of stakes decreases with each battle, the staked **${token}** in the first battle 
will bring the Investor greater rewards than in the last battle.
</div>

::card_formula
::formula
<MathFormula formula="Wi=(Tr-Cr)/Tr*Ia" />,
::
where:
* **Tr:** the total number of rounds;
* **Cr**: the current round number;
* **Ia**: the number of **${token}** staked by the Investor.
::

::card_warning
The cost may vary depending on the exchange rate of Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **{token}** 
staked by the participants is collected in the treasury. After the victory of your 
Faction, the staked funds will be returned and rewards will be distributed.
::

## Return of staked {token}
All staked **${token}** is collected into a common pool (Treasury) for each Faction. If an Investor 
belongs to a winning Faction, he will receive back his deposited **${token}**, but only stakes 
made in the winning Faction.

## Rewards for winning
Investors receive 70% of the rewards from the winning Faction's reward pool. The distribution 
of rewards among Investors will be carried out depending on the weight of their stakes in 
the winning Faction.

### The formula for calculating determining an Investor's reward

::card_formula
::formula
<MathFormula formula="InvRew = \frac{SumWi}{SumTotalWi}*RewardForInvestors" />,
::
where:
* **SumWi**: the sum of the Investor's investment weights;
* **SumTotalWi**: the sum of the investment weights of all Investors;
* **RewardForInvestors**: 70% of the rewards from the winning Faction's reward pool.
::

::card_info
Example of determining an Investor's reward (assuming that the total number of rounds = 95 
and the number of Investors = 2):
* **Investor 1** staked **100 {token}** in Faction "A" on its 3rd Battle (Wi = 96.842) and **1000 {token}** in 
Faction "B" on its 10th Battle (Wi = 894.736)
* **Investor 2** staked **10,000 {token}** in Faction "B" on the 5th Battle (Wi = 9473.684)
* The "B" faction wins and receives **100,000 {token}** (70% of which goes to Investors (**70,000 {token}**)
* The sum of the weight of the staked **{token}** in the Winners' Faction, from all Investors = 
894.736 + 9473.684 = 10368.42, is 100%
* The share of **Investor 1**, taking into account its investment weight, is 8.63%, which means the 
reward = **6041 {token}** 
* The share of **Investor 2**, taking into account its investment weight, is 91.37%, which means the 
reward = **63959 {token}**
::

::card_warning
Remember that the amount of investment increases with each round. The earlier **${token}** is deposited the 
greater the reward.
::
