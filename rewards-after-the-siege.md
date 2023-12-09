# 🎇 Rewards After The Siege

After 80,640 blocks (~14 days), One faction is declared the victor of the Siege. The Faction with the 
most Battle victories will receive rewards:
* **Winners are returned any {token}** they have invested during the entirety of the Siege;
* **30%** of the invested {token} from the losing Faction is distributed among the Winning Faction;
* **70%** of the losing Faction's treasury is rewarded to the Investors.

## Reward for NFT Owners

The reward for the winning Faction is distributed using the following formulas.

### The Warrior's preliminary coefficient (PreK)

<MathComponent :mathExpression="'PreK={PlayerDMG} \over {TeamDMG}+{PlayerSPH} \over {TeamSPH}'" /></MathComponent>,

where:
* PlayerDMG: the sum of attacks of all NFTs of one Player at the end of the Siege;
* TeamDMG: the sum of the attacks of all NFTs in the Faction at the end of the Siege;
* PlayerSPH: the number of sapphires on the Player's balance at the end of the Siege;
* TeamSPH: the sum of the number of Sapphires on the balance of all Players of the Faction at the end of the Siege.

### The sum of the preliminary coefficients of all Players in the winning Faction (TeamK)

<MathComponent :mathExpression="'TeamK =(\sum_{i=Player}^{TeamAmount}PreK_i)'" /></MathComponent>,

where:
* PreK: the Player's preliminary coefficient;
* TeamAmount: the number of players in the winning Faction.

### The final coefficient of the Player (Koef)

<MathComponent :mathExpression="'Koef={PreK \over TeamK}'" /></MathComponent>,

where:
* PreK: the Player's preliminary coefficient;
* TeamK: the sum of the preliminary coefficients of the other Players.

### The reward for the Player (PlayerR)

<MathComponent :mathExpression="'PlayerR=TeamR*Koef'" /></MathComponent>,

where:
* Team: 30% of the amount invested in the losing Faction;
* Koef: the final coefficient of the Player.

### Example

* Invested in the losing Faction: 10000 {token};
* The winning Faction has only 5 NFTs;
* The Gamer_1 has 2 NFT in possession, with an attack power of 10 and 15;
* Gamer_1 has 100 pieces of Sapphires on the balance;
* The rest of the players have NFT with attack power: 11, 8 and 5;
* Total Sapphires on the balance of the Players of the Winning Faction 250;

Calculation of the Player_1 reward:
1. PlayerDMG = 10+15 = 25
2. TeamDMG = 11+8+5+10+15 = 49
3. PlayerSPH = 100
4. TeamSPH = 250
5. TeamR = 10000 * 0.8 = 8000
6. PreK =  25/49 + 100/250 = 0.91
7. The sum of the preliminary coefficients of the other Players = 24/49 + 150/250 = 1.08
8. TeamK = 0.91 + 1.08 = 1.99
9. Koef = 0.91/1.99 = 0.4572
10. **PlayerR = 8000 * 0.4572 = 3657.6**

## Reward for Investors
Investors can invest **${token}** in one Faction or both. But only one Faction is declared winner for each 
siege. It should be noted that each Investor acts by their own will and receives rewards based on where, 
when, and how much **${token}** is invested.\
Investors receive rewards depending on how much {token} has been invested in the winning Faction. With each 
Battle, the "weight" of investments falls.\
Learn more:

{% content-ref url="investors.md" %}
[investors.md](investors.md)
{% endcontent-ref %}

## Other Rewards

After the Siege ends, 10% of the collected commission (in **${token}**) is automatically Airdropped to users, that voted 
for the winning Faction.\
An additional 10% of the collected commission is distributed as a reward to active users, content makers, 
bloggers, artists, etc.