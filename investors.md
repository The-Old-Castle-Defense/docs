---
description: >-
  Investors in the Old Castle Defense game are users who invested $MC in one or
  both factions during the Siege.
---

# 📈 Investors

The Investor can participate in determining the outcome of the siege by contributing to one or both factions, helping them achieve victory. If the Faction in which he invested, he receives a reward from the treasury of the losing faction, and all **$MC** invested in the winning Faction is returned. Investors receive 70% of the treasury, while NFT holders receive 30% of the treasury.

Available actions for Investors:

* Buying a Faction Attack;
* Reviving fallen NFT characters for either Faction;
* Boosting level up for any NFT.

## Buying a Faction Attack

Investors can increase the Faction's attack power by spending **$MC**, but each subsequent Attack Boost becomes more expensive than the previous one.

Each Attack Boost will increase the attack power of a Faction. A number is chosen randomly, within range of the current boost level, and added to the Faction's total Attack Power. Each increase in attack power increases an investor's stake, which means a greater share of the prize if the Faction is victorious.

When **$MC** is used to boost a Faction's attack, it is stored in that Faction's treasury. During each Siege, both factions' treasuries also serve as the reward pool, from which the winning Faction is awarded.

Calculation of the range of attack probability and cost:

| Level Increase | Attack Power Increase | Cost ($MC) |
| -------------- | --------------------- | ---------- |
| 1              | 2-5                   | 2          |
| 2              | 3-6                   | 4          |
| 3              | 4-7                   | 6          |
| 4              | 5-8                   | 8          |
| 5              | 6-9                   | 10         |
| ...            | ...                   | ...        |
| 100            | 101-104               | 200        |
| n              | (n+1)-(n+4)           | 2n         |

{% hint style="warning" %}
The cost may vary depending on the exchange rate of $MC.

The price includes a service commission of 6%. After deducting the commission, the $**MC** deposited by the investors is collected in the treasury. All invested funds are returned to the winners as well as an additional reward.
{% endhint %}

### Revival

Investors can revive deceased NFT characters. The cost of each revival is calculated by the formula:

$$
RevCost = LVL + 1,
$$

where:

* **RevCost** is the cost of reviving in **$MC**;
* **LVL** is the level of NFT at the time of death.

{% hint style="warning" %}
The price includes a service commission of 6%. After deducting the commission, the $**MC** deposited by the investors is collected in the treasury. All invested funds are returned to the winners as well as an additional reward.
{% endhint %}

## Reward system

Investors can invest **$MC** in one Faction or both at once. But in each Siege, only one Faction wins. It should be noted that the Investor acts independently and receives remuneration depending on which faction, when, and how much **$MC** was invested.

{% hint style="warning" %}
The investor receives a reward depending on the amount of $**MC** invested in the winning Faction. With each Battle, the "weight" of investments decreases.
{% endhint %}

### Learn more about the weight of investments

The weight of investments decreases with each battle, the invested $**MC** in the first battle will bring the Investor greater rewards than in the last battle.

The formula for calculating the weight of investments (**Wi**):

$$
Wi = (Tr - Cr) / Tr * Ia,
$$

where:

* **Tr** is the total number of rounds;
* **Cr** is the current round number;
* **Ia** is the number of **$MC** invested by the investor.

### Return of Invested $**MC**

All invested $**MC** is collected into a common pool (Treasery) for each Faction. If an Investor belongs to a winning Faction, he will receive back his deposited $**MC**, but **only investments made in the winning Faction**.

### Rewards for winning

Investors receive 70% of the rewards from the winning Faction's reward pool. The distribution of rewards among investors will be carried out depending on the weight of their investments in the winning Faction.

The formula for calculating determining an investor's reward:

$$
InvRew = \frac{SumWi}{SumTotalWi}*RewardForInvestors,
$$

where:

* **SumWi** is the sum of the investor's investment weights;
* **SumTotalWi** is the sum of the investment weights of **all** investors;
* **RewardForInvestors** is 70% of the rewards from the winning Faction's reward pool.

{% hint style="info" %}
Example of determining an investor's reward (assuming that the total number of rounds = 95 and the number of Investors = 2):

* Investor 1 invested 100 **$MC** in Faction "A" on its 3rd Battle (Wi = 96.842) and 1000 **$MC** in Faction "B" on its 10th Battle (Wi = 894.736)
* Investor 2 invested 10,000 **$MC** in Faction "B" on the 5th Battle (Wi = 9473.684)
* The "B" faction wins and receives 100,000 **$MC** (70% of which goes to Investors (70,000 **$MC** )
* The sum of the weight of the invested **$MC** in the Winners' Faction, from all Investors = 894.736 + 9473.684 = 10368.42, is 100%
* The share of Investor 1, taking into account its investment weight, is 8.63%, which means the reward = 6041 **$MC**&#x20;
* The share of Investor 2, taking into account its investment weight, is 91.37%, which means the reward = 63959 **$MC**
{% endhint %}

{% hint style="warning" %}
Remember that the amount of investment increases with each round. The earlier **$MC** is deposited the greater the reward.
{% endhint %}
