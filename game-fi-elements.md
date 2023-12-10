# 🎯 Game-Fi Elements

<p>Only teamwork will lead the Faction to victory, so that the team does not 
break up, it is necessary to monitor the life and strength of the characters.</p>

::card_warning
The game is built on a smart contract, so any burning of **$SPH** or investment of **${token}** 
requires confirmation in the blockchain.
::

## Healing
After each Battle, the health level of the character drops by 11% of the maximum HP.

To restore 1% health, users must burn 1 Sapphire (**$SPH**).

It is better to restore a character's health in time, as each missing point of health 
reduces the attack power of the character by 1%.

### Formula

::card_formula
<MathComponent :mathExpression="'CurAttack*(CurHealth/MaxHealth)'" />,
::

where:
* **CurAttack** is current NFT attack;
* **CurHealth** is current NFT health;
* **MaxHealth** is maximum NFT health.

### Example

<table>
  <thead>
    <tr>
      <th>HEALTH LEVEL (MAX = 100)</th>
      <th>ATTACK</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>100</td>
      <td>10</td>
    </tr>
    <tr>
      <td>89</td>
      <td>8.9</td>
    </tr>
    <tr>
      <td>78</td>
      <td>6.942</td>
    </tr>
  </tbody>
</table>

::card_warning
If the health level of the character drops to 0, it is considered "fallen" and cannot participate in the 
current battle, unless it is revived.
::

## Revival

Investors can revive deceased NFT characters. The cost of each revival is calculated by 
the formula.

### Formula

::card_formula
<MathComponent :mathExpression="'RevCost=LVL+1'" /></MathComponent>,
::

where:
* **RevCost** is the cost of reviving in ${token};
* **LVL** is the level of NFT at the time of death.

::card_warning
The cost may vary depending on the exchange rate of Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **${token}** 
invested by the participants is collected in the treasury. After the victory of your 
Faction, the invested funds will be returned and rewards will be distributed.
::

## Level Up

Level up your NFT characters to increase strength, and compete with the opposing Faction, 
overpowering them and getting closer to achieving victory.

$SPH is required to level up a character. Each level increase lasts a certain number of 
blocks, which increases alongside the required amount of $SPH. This process can be 
accelerated using **${token}** (Boost Level Up).

<table>
  <thead>
    <tr>
      <th>TO LEVEL</th>
      <th>BLOCKS</th>
      <th>COST ($SPH)</th>
      <th>COST TO BOOST ({token})</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>60</td>
      <td>10</td>
      <td>1</td>
    </tr>
    <tr>
      <td>2</td>
      <td>120</td>
      <td>20</td>
      <td>2</td>
    </tr>
    <tr>
      <td>3</td>
      <td>180</td>
      <td>30</td>
      <td>3</td>
    </tr>
    <tr>
      <td>n</td>
      <td>n * 60</td>
      <td>n * 10</td>
      <td>n</td>
    </tr>
  </tbody>
</table>

::card_warning
The cost may vary depending on the exchange rate of Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **${token}** 
invested by the participants is collected in the treasury. After the victory of your 
Faction, the invested funds will be returned and rewards will be distributed.
::

When a character is leveled up, their attack power increases. The amount of attack increase 
is determined randomly between a certain range.

## Boost Level Up

::card_info
If you use the Faction attack boost functionality, you become an Investor.
::

## Buy Faction Attack

Investors can increase the faction's attack power in exchange for **${token}**, but each 
subsequent increase costs them more than the previous one.

Each boost adds a random number to the total attack power of the Faction within the 
range of the current boost level.

### Calculating the range of attack probability and cost

<table>
  <thead>
    <tr>
      <th>LEVEL OF INCREASE</th>
      <th>ATTACK INCREASE RANGE</th>
      <th>COST ({token})</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>1</td>
      <td>2 - 5</td>
      <td>1</td>
    </tr>
    <tr>
      <td>2</td>
      <td>3 - 6</td>
      <td>2</td>
    </tr>
    <tr>
      <td>3</td>
      <td>4 - 7</td>
      <td>3</td>
    </tr>
    <tr>
      <td>4</td>
      <td>5 - 8</td>
      <td>4</td>
    </tr>
    <tr>
      <td>5</td>
      <td>6 - 9</td>
      <td>5</td>
    </tr>
    <tr>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <td>100</td>
      <td>101 - 104</td>
      <td>100</td>
    </tr>
    <tr>
      <td>n</td>
      <td>(n+1) "-" (n+4)</td>
      <td>n</td>
    </tr>
  </tbody>
</table>

::card_warning
The cost may vary depending on the exchange rate of Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **${token}** 
invested by the participants is collected in the treasury. After the victory of your 
Faction, the invested funds will be returned and rewards will be distributed.
::