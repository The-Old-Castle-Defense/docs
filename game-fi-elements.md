---
navigation:
    order: 3
---

# 🎯 Game-Fi Elements

<p>Only teamwork will lead the Faction to victory so that the team does not 
break up, it is necessary to monitor the life and strength of the characters.</p>

::card_warning
The game is built on a smart contract, so any burning of **$SPH** or stake **${token}** 
requires confirmation in the blockchain.
::

## Healing
<div>

After each Battle, the health level of the character drops by 11% of the maximum HP. To restore 1% health, 
users must burn 1 Sapphire (**$SPH**).
</div>

### How to heal NFT?

<div>

Click on the button with the green "+" symbol on the character image:
</div>

<img src="/assets/docs/.gitbook/assets/nft_for_heal.png" alt="">

::card_info
It is better to restore a character's health in time, as each missing point of health 
reduces the attack power of the character by 1%.
::

### The formula for reducing attack depending on the health

::card_formula
::formula
<MathFormula formula="NewAttack=(CurHealth*CurAttack)/MaxHealth)" />,
::
where:
* **NewAttack**: an NFT attack after the Battle;
* **CurHealth**: current NFT health (every time after the Battle: MaxHealth - 11);
* **CurAttack**: current NFT attack at the time of the Battle;
* **MaxHealth**: maximum NFT health.
::

### Example

<table class="docs-table">
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

<div>
    
Investors can revive deceased NFT characters.
</div>

### How to revive NFT?

<div>
    
Click on the button with the image of the first aid kit, to the right of the amount of health of the NFT:
</div>

<img src="/assets/docs/.gitbook/assets/revive_button.png" alt="">

### The formula for calculating the cost of revival

::card_formula
::formula
<MathFormula formula="RevCost=LVL+1" />,
::
where:
* **RevCost**: the cost of reviving in ${token};
* **LVL**: the level of NFT at the time of death.
::

::card_warning
The cost may vary depending on the exchange rate of the Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **${token}** 
invested by the participants is collected in the treasury. After the victory of your 
Faction, the invested funds will be returned and rewards will be distributed.
::

## Level Up (Upgrade)

<div>

Level up your NFT characters to increase strength, and compete with the opposing Faction, 
overpowering them and getting closer to achieving victory.
</div>

### How to upgrade NFT?

<div>

Click on the button with the green arrow up on the character image:
</div>

<img src="/assets/docs/.gitbook/assets/nft_for_upgrade.png" alt="">

<div>

And confirm the start of the upgrade:
</div>

<img src="/assets/docs/.gitbook/assets/modal_for_upgrade_nft.png" alt="">

<div>

$SPH is required to level up a character. Each level increase lasts a certain number of 
blocks, which increases alongside the required amount of $SPH. This process can be 
accelerated using **${token}** (Boost Level Up).
</div>

<table class="docs-table">
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
The cost may vary depending on the exchange rate of the Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **${token}** 
invested by the participants is collected in the treasury. After the victory of your 
Faction, the invested funds will be returned and rewards will be distributed.
::

When a character is leveled up, their attack power increases. The amount of attack increase 
is determined randomly between a certain range. But, after the timer expires, you need to confirm the 
upgrade in the blockchain (read below "Checking the upgrade").

## Boosting the upgrade

<div>

Skip the waiting time before the NFT level is raised.
</div>

### How to boost the upgrade?

<div>

Click on the button with the green clock:
</div>

<img src="/assets/docs/.gitbook/assets/nft_for_boost.png" alt="">

<div>

And confirm the Boost:
</div>

<img src="/assets/docs/.gitbook/assets/modal_for_boost_upgrade_nft_{blockchain}_{token}.png" alt="">

::card_info
If you use the Faction attack boost functionality, you become an Investor.
::

## Checking the update

<div>

After the upgrade timer expires, it is required to confirm the increase in the NFT level to write 
this data to the blockchain:
</div>

### How to check the update?

<div>

Click on the button with the green looped arrows:
</div>

<img src="/assets/docs/.gitbook/assets/upgrade_nft_check.png" alt="">

## Burning of Sapphires (SPH)

<div>

To increase their share of the treasury, NFT owners can burn SPH. This increases their coefficient 
when calculating the reward at the end of the Siege.
</div>

### How to burn SPH

<div>

Click on the button with the green light:
</div>

<img src="/assets/docs/.gitbook/assets/burning_sph.png" alt="">

<div>

Select the number of SPH to burn and confirm the action:
</div>

<img src="/assets/docs/.gitbook/assets/modal_for_burn_sph.png" alt="">

<div>

Read more about the calculation in the section:
</div>

<a href="rewards-after-the-siege" 
 class="docs-item">
<span>⚔️</span>
Rewards After The Siege</a>

## Increasing the Faction's attack with stake

<div>

Investors can increase the faction's attack power in exchange for **${token}**, but each 
subsequent increase costs them more than the previous one.
</div>

### How to stake {token}?

<div>

Click the "Stake to attack" button under the window of one of the Factions:
</div>

<img src="/assets/docs/.gitbook/assets/buy_attack_button.png" alt="">

<div>

Choose the right number of attack boost levels and click the button:
</div>

<img src="/assets/docs/.gitbook/assets/attack_levels_{blockchain}_{token}.png" alt="">

<div>

And confirm the transaction on the website and in your wallet. If the transaction is successfully confirmed, 
you will see a similar notification at the bottom right:
</div>

<img src="/assets/docs/.gitbook/assets/confirmed_transaction.png" alt="">

<div>

Each boost adds a random number to the total attack power of the Faction within the 
range of the current boost level.
</div>

### Calculating the range of attack probability and cost

<table class="docs-table">
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
The cost may vary depending on the exchange rate of the Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **${token}** 
invested by the participants is collected in the treasury. After the victory of your 
Faction, the invested funds will be returned and rewards will be distributed.
::

## Start the next Battle

<div>

TOCD is completely decentralized, where the community manages the game itself.
</div>

### How to start the next Battle?

<div>

To start a new battle, you need to click on the "Next Battle" button in the middle of the page. 
</div>


::card_info
The "Next Battle" button will appear when a sufficient number of blocks in the blockchain are generated
::
