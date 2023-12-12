---
navigation:
   order: 5
---

# 📈 Investors

<p>Investors in the Old Castle Defense game are users who invested **${token}** in one or both factions 
during the Siege.</p>

<div>
The Investor can participate in determining the outcome of the siege by contributing to one or 
both factions, helping them achieve victory. If the Faction in which he invested, he receives 
a reward from the treasury of the losing faction, and all **${token}** invested in the winning Faction 
is returned. Investors receive 70% of the treasury, while NFT holders receive 30% of the treasury.
</div>

<div>
Available actions for Investors:
* Buying a Faction Attack;
* Reviving fallen NFT characters for either Faction;
* Boosting level up for any NFT.
</div>

<div>
Learn more about it:

<a href="game-fi-elements" 
 class="docs-item">Game-Fi elements</a>
</div>

## Reward system
Investors can stake **${token}** in one Faction or both at once. But in each Siege, only one 
Faction wins. It should be noted that the Investor acts independently and receives 
remuneration depending on which faction, when, and how much **${token}** was invested.

::card_warning
The investor receives a reward depending on the amount of **${token}** invested in the winning 
Faction. With each Battle, the "weight" of investments decreases.
::

### The formula for calculating the weight of investments
The weight of investments decreases with each battle, the invested **${token}** in the first battle 
will bring the Investor greater rewards than in the last battle.

::card_formula
::formula
<MathFormula formula="Wi=(Tr-Cr)/Tr*Ia" />,
::
where:
* Tr: the total number of rounds;
* Cr: the current round number;
* Ia: the number of **${token}** invested by the investor.
::

::card_warning
The cost may vary depending on the exchange rate of Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **{token}** 
invested by the participants is collected in the treasury. After the victory of your 
Faction, the invested funds will be returned and rewards will be distributed.
::

## Return of Invested {token}
All invested **${token}** is collected into a common pool (Treasury) for each Faction. If an Investor 
belongs to a winning Faction, he will receive back his deposited **${token}**, but only investments 
made in the winning Faction.

## Rewards for winning
Investors receive 70% of the rewards from the winning Faction's reward pool. The distribution 
of rewards among investors will be carried out depending on the weight of their investments in 
the winning Faction.

### The formula for calculating determining an investor's reward

::card_formula
::formula
<MathFormula formula="InvRew = \frac{SumWi}{SumTotalWi}*RewardForInvestors" />,
::
where:
* SumWi: the sum of the investor's investment weights;
* SumTotalWi: the sum of the investment weights of all investors;
* RewardForInvestors: 70% of the rewards from the winning Faction's reward pool.
::

::card_info
Example of determining an Investor's reward (assuming that the total number of rounds = 95 
and the number of Investors = 2):
* **Investor 1** invested **100 {token}** in Faction "A" on its 3rd Battle (Wi = 96.842) and **1000 {token}** in 
Faction "B" on its 10th Battle (Wi = 894.736)
* **Investor 2** invested **10,000 {token}** in Faction "B" on the 5th Battle (Wi = 9473.684)
* The "B" faction wins and receives **100,000 {token}** (70% of which goes to Investors (**70,000 {token}**)
* The sum of the weight of the invested **{token}** in the Winners' Faction, from all Investors = 
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