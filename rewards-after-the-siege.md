# 🎇 Rewards After The Siege

After 80,640 blocks (\~14 days), One faction is declared the victor of the Siege. The Faction with the most Battle victories will receive rewards:

* Winners are returned any **$MC** they have invested during the entirety of the Siege;
* 30% of the invested **$MC** from the losing Faction is distributed among the Winning Faction;
* 70% of the losing Faction's treasury is rewarded to the Investors.

## Reward for NFT Owners

The reward for the winning Faction is distributed using the following formulas:

1. **PreK** is the Player's preliminary coefficient

$$
PreK = {{PlayerDMG} \over {TeamDMG}} +{{PlayerSPH} \over {TeamSPH}},
$$

where:

* **PlayerDMG** is the sum of attacks of all NFTs of one Player at the end of the Siege;
* **TeamDMG** is the sum of the attacks of all NFTs in the Faction at the end of the Siege;
* **PlayerSPH** is the number of sapphires on the Player's balance at the end of the Siege;
* **TeamSPH** is the sum of the number of Sapphires on the balance of all Players of the Faction at the end of the Siege.



&#x20;  2\. **TeamK** is the sum of the preliminary coefficients of all Players in the winning Faction

$$
TeamK =(\sum_{i=Player}^{TeamAmount}PreK_i),
$$

where:

* **PreK** is the Player's preliminary coefficient;
* **TeamAmount** is the number of players in the winning Faction.



&#x20;  3\. **Koef** is the final coefficient of the Player

$$
Koef = {PreK \over TeamK},
$$

where:

* **PreK** is the Player's preliminary coefficient;
* **TeamK** is the sum of the preliminary coefficients of the other Players.



&#x20;   4\. **Player** is a reward for the Player

$$
PlayerR = TeamR * Koef,
$$

where:

* **Team** is 30% of the amount invested in the losing Faction;
* **Koef** is the final coefficient of the Player.

{% hint style="info" %}
Example:

* Invested in the losing Faction: 10000 **$MC;**
* The winning Faction has only 5 NFTs;
* The Gamer\_1 has 2 NFT in possession, with an attack power of 10 and 15;
* Gamer\_1 has 100 pieces of Sapphires on the balance;
* The rest of the players have NFT with attack power: 11, 8 and 5;
* Total Sapphires on the balance of the Players of the Winning Faction 250;

&#x20;&#x20;

Calculation of the Player\_1 reward:

* **PlayerDMG = 10+15 = 25**
* **TeamDMG = 11+8+5+10+15 = 49**
* **PlayerSPH = 100**
* **TeamSPH = 250**
* **TeamR = 10000 \* 0.8 = 8000**

**PreK =  25/49 + 100/250 = 0.91**

**The sum of the preliminary coefficients of the other Players = 24/49 + 150/250 = 1.08**

**TeamK = 0.91 + 1.08 = 1.99**

**Koef = 0.91/1.99 = 0.4572**

<mark style="color:green;">**PlayerR = 8000 \* 0.4572 = 3657.6**</mark>
{% endhint %}

## Reward for Investors

Investors can invest **$MC** in one Faction or both. But only one Faction is declared winner for each siege. It should be noted that each Investor acts by their own will and receives rewards based on where, when, and how much **$MC** is invested.

Investors receive rewards depending on how much **$MC** has been invested in the winning Faction. With each Battle, the "weight" of investments falls.

Learn more:

{% content-ref url="investors.md" %}
[investors.md](investors.md)
{% endcontent-ref %}

## Other Rewards

After the Siege ends, 10% of the collected commission (in **$MC**) is automatically Airdropped to users, that voted for the winning Faction

An additional 10% of the collected commission is distributed as a reward to active users, content makers, bloggers, artists, etc.
