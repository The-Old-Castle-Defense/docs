---
navigation:
    order: 9
---

# ⚔️ Rewards After The Siege

<div>

At the end of each Siege, there is a distribution of ${token}. The amount of ${token} 
is determined by the formula.
</div>

<div>

After {siege_duration} blocks, One faction is declared the victor of the Siege. The Faction with the 
most Battle victories will receive rewards:
* **Winners are returned any ${token}** they have staked during the entirety of the Siege;
* **30%** of the treasury of the losing Faction is shared by the NFT Owners of the winning Faction;
* **70%** of the treasury of the losing Faction is rewarded to the Investors.
</div>

## Reward for NFT Owners

The reward for the winning Faction is distributed using the following formulas.

### The NFT's preliminary coefficient (NFTreK)

::card_formula
::formula
<MathFormula formula="NFTreK=\frac{NftDMG}{TeamNftDMG} + \frac{BurnedNftSPH}{BurnedTeamSPH}" />,
::
where:
* **NftDMG**: the attack of NFT at the end of the Siege;
* **TeamNftDMG**: the sum of the attacks of all NFTs in the Faction at the end of the Siege;
* **BurnedNftSPH**: the number of Burned Sapphires of the Player at the end of the Siege;
* **BurnedTeamSPH**: the sum of the number of Burned Sapphires of the Faction at the end of the Siege.
::

### The sum of the preliminary coefficients of all Players in the winning Faction (TeamK)

::card_formula
::formula
<MathFormula formula="TeamK =(\sum_{i=Player}^{TeamAmount}NFTreK_i)"/>,
::
where:
* **NFTreK**: the Player's preliminary coefficient;
* **TeamAmount**: the number of players in the winning Faction.
::

### The final coefficient of the Player (Koef)

::card_formula
::formula
<MathFormula formula="Koef={NFTreK \over TeamK}" />,
::
where:
* **NFTreK**: the Player's preliminary coefficient;
* **TeamK**: the sum of the preliminary coefficients of the other Players.
::

### The reward for the Player (PlayerR)

::card_formula
::formula
<MathFormula formula="PlayerR=TeamR*Koef"/>,
::
where:
* **TeamR**: reward for NFT Owners;
* **Koef**: the final coefficient of the Player.
::

### Example

<div>

* Staked in the losing Faction: 10,000 {token};
* The winning Faction has only 5 NFTs;
* Alice has NFT with an attack power of 10;
* Alice has 100 $SPH on the balance;
* The rest of the Players have NFT with attack power: 11, 8 and 5;
* Total Sapphires on the balance of the Players of the Winning Faction = 250.
</div>

<div>

**Calculation of the Alice reward:**
1. TeamDMG = 11+8+5+10 = 34
2. PlayerSPH = 100
3. TeamSPH = 250
4. TeamR = 10,000*0.3 = 3,000
5. NFTreK =  10/34 + 100/250 = 0.69
6. The sum of the preliminary coefficients of the other NFTs = 24/34 + 150/250 = 1.3
8. TeamK = 0.69 + 1.3 = 1.99
9. Koef = 0.69/1.99 = 0.3467
10. **PlayerR = 3,000 * 0.3467 = 1,040.1**

**Alice will be rewarded with 1,040.1 ${token}**
</div>

## Reward for Investors

<div>

Investors can invest **${token}** in one Faction or both. But only one Faction is declared winner for each 
siege. It should be noted that each Investor acts by their own will and receives rewards based on where, 
when, and how much **${token}** is invested.\
Investors receive rewards depending on how much {token} has been invested in the winning Faction. With each 
Battle, the "weight" of investments falls. Learn more:

<a href="investors" 
 class="docs-item">
<span>📈</span>
Investors</a>
</div>

## Other Rewards

<div>

After the Siege ends, 10% of the collected commission (in **${token}**) is automatically Airdropped to users, that voted 
for the winning Faction.\
An additional 10% of the collected commission is distributed as a reward to active users, content makers, 
bloggers, artists, etc.
</div>