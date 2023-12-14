---
navigation:
    order: 8
---

# 💎 Rewards After The Battle

<p>Each Battle won brings one of the sides closer to victory in the Siege.</p>

<div>
During the battle, the task of the Faction of Terrible Creatures is to return as many Sapphires as possible. 
The task of the Knights Faction is to protect the Old Castle, because, in case of their victory, the King 
will generously reward his defenders.

<img src="/assets/docs/.gitbook/assets/rewards_after_the_battle.png" alt="">
</div>

<div>

There is a check on the strength of the attack power of both factions every 960 blocks. The Faction with 
the superior attack power wins the battle (~4 hours).\
The victorious battle is recorded in the total score of the Siege of the Castle. At the end of the 
Siege (~14 days), the team with the most victories in battles is considered the winner.
</div>

### Battle Reward

At the end of each battle, there is a distribution of $SPH. The amount of $SPH is determined by the formula.

## Formula

::card_formula
::formula
<MathFormula formula="RewardSPH=4000*(StakedNFTsAmount/200)"/>,
::
where:
* **AmountNFT**: the total number of NFTs in the game at the time of the Battle;
* **4000** is the maximum amount of $SPH that is distributed after the Battle;
* **200** is the maximum total number of NFTs in a game.
::

<div>

The sum of the attack power of both sides is 100%, each Faction will receive an amount of $SPH from the 
total pool, but depending on the amount of attack power as a percentage.
</div>

::card_info
**Example:** 
* **Faction 1:** 170 attack power;
* **Faction 2:** 280 attack power;
* **Faction 2 wins** the battle 170 + 280 = 450 (100%);
* **Faction 1 will receive** 1511.2 SPH (170 attack power is 37.78% of 450);
* **Faction 2 will receive** 2488.8 SPH (280 attack power is 62.22% of 450)
::

::card_warning
The distribution of rewards within the faction also occurs depending on the strength of the attack. The 
character with the highest attack power will get the biggest reward. The calculation takes place for 
each NFT separately.
::

<div>

The distribution of $SPH within the faction is determined by the formula.
</div>

## Formula

::card_formula
::formula
<MathFormula formula="RewardForNFT = \frac{NFTAttack}{FactionAttack}*FactionSPHReward"/>,
::
where:
* **NFTAttack**: an attack of a single NFT;
* **FactionAttack**: an attack of the Faction to which the NFT belongs (without strengthening the Faction's 
attack);
* **FactionSPHReward**: the total Faction reward for the past battle ($SPH).
::