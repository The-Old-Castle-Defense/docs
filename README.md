# Variables, tags, and documentation markup rules

## Variables
- **{blockchain}**: The name of Blockchain;
- **{block_explorer}**: The link to block explorer of the blockchain;
- **{bps}**: The number of blocks per second in the current blockchain;
- **{token}**: The Treasury token on Blockchain
- **{battle_duration}**: Time until the start of the next battle in the current blockchain;
- **{transactions}**: The link to a transaction of a decentralized referral system in the current blockchain;
- **{knights_market_link}**: The link to the marketplace with Knights NFTs;
- **{creatures_market_link}**: The link to the marketplace with Creatures NFTs;
- **{bank_address}**: The address with treasury pool.

## Editing the main documentation page
The data from the main documentation page is stored in the "_docs Menu.json" file. 
The "_" in front of the file name indicates that this page does not need to be specified in the navigation

## Tags and rules

### A separate block of text
Each separate block of text must be marked with a <div> tag, **skipping the line after the opening tag.** 
Example:
```
<div>

Hello, world!
</div>
```

### Information cards
To highlight information that requires special attention, the "card_info" or "card_warning" tag is used. Example:
```
::card_info
This is additional information or a hint.
::
```
```
::card_warning
This is information that requires special attention
::
```

### Adding Images
All images must be stored in a folder along the path: ".gitbook/assets/i_am_here.png"
For an image that is suitable only for a specific blockchain, it is required to specify the name of the blockchain and the token's treasury through the "_" symbol.

**Example of the image name:**
```
i_am_here_Beam Mainnet_BEAM.png
```
**Example of embedding an image:**
```
<img src="/assets/docs/.gitbook/assets/i_am_here_{blockchain}_{token}.png" alt="">
```

### Embedded links
```
<a href="https://theoldcastle.xyz" target="_blanc" class="doc-link">example</a>
```

### Formulas:
```
::card_formula  
::formula  
<MathFormula formula="RevCost=LVL+1"/>,  
::  
where:  
* **RevCost**: the cost of reviving in ${token};  
* **LVL**: the level of NFT at the time of death.  
::
```

### Navigation:
To comply with the required order of articles and sections, it is required to specify an additional block with a number at the beginning of the document
```
---
navigation  
 order: 2  
---
```

### Buttons
To add a button leading to another document, you need to specify a block:
```
<a href="investors" 
 class="docs-item">
<span>📈</span>
Investors</a>
</div>
```
