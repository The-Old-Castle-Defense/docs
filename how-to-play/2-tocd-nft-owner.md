# Warrior - Owner of TOCD NFT
<div>

Players owning TOCD NFT earn ${token} if the NFT was staked, the NFT's faction won, and the NFT has more than 0 HP.
</div>

<div>

Owners of TOCD NFTs do not need to stake ${token}; they use game tokens - SPH. To increase the reward that the NFT 
owner receives at the end of the Siege, they need to level up and monitor the HP of the NFT.
</div>

## Buying TOCD NFT

::card_info
TOCD supports the policy: **80%** of all NFT will be distributed to active users and influencers.
::

You can find the complete collection at: https://element.market/collections/tocdnft

## Staking

<div>

1. On the “Game” page, press the “Stake NFT” button in the middle of the page:
<img src="/assets/docs/.gitbook/assets/stake.png" alt="">
</div>

<div>

2. You will see a window to select your NFT:
<img src="/assets/docs/.gitbook/assets/selected_nft.png" alt="">
</div>

<div>

3. Select the NFT to stake it for the duration of the Siege:
<img src="/assets/docs/.gitbook/assets/selected_nft.png" alt="">
</div>

<div>

**Ready!** The game will start immediately after investing in one of the Factions.
<img src="/assets/docs/.gitbook/assets/stake_ready.png" alt="">
</div>

## Leveling Up

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

### Boost Level Up

<div>

You can skip the waiting time before the NFT level is raised.
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

### Confirm Level Up

<div>

After the upgrade timer expires, it is required to confirm the increase in the NFT level to write 
this data to the blockchain:
</div>

### How to check the update?

<div>

Click on the button with the green looped arrows:
</div>

<img src="/assets/docs/.gitbook/assets/upgrade_nft_check.png" alt="">

## Healing

<div>

After each Battle, the character's health level drops by 11% of the maximum HP. To restore 1% health, 
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

### The formula for reducing attack depends on the health

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


### Reviving

<div>
    
You can revive deceased NFT characters.
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

## Sapphires

<div>

Sapphires (SPH) are a crucial in-game currency in The Old Castle Defense, used primarily for healing 
and upgrading NFT characters. NFT Owners earn Sapphires every Battle in the Siege.
</div>

### Buying Sapphires

::card_info
The funds transferred to the Dealer in exchange for Sapphires will be invested in the treasury of the 
staked NFT faction.
::

<div>

Players of the "Terrible Creatures" and "Knights Of The Kingdom" Factions can purchase 
Sapphires ($SPH) from the Dealer to level up their NFTs or heal them.
</div>

::card_info
Sapphires are always sold at a fixed price: 1 $SPH = {sph_cost} {token}".
::

::card_warning
The cost may vary depending on the exchange rate of the Treasury Token (if it is not $USDT).\
The price includes a service fee of 6%. After the commission is deducted, the **${token}** 
invested by the participants is collected in the treasury. After the victory of your 
Faction, the invested funds will be returned and rewards will be distributed.
::

### Burning Sapphires

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

## Start the Next Battle

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
