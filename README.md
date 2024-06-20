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

# Files

## _<main|dev>NetDeploys.json

### Data

| **Attribute**       | **Type**   | **Description**                                                                                                                                                  |
| :------------------ | :--------- | :--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| _id                 | int        | The unique identifier of the deployment                                                                                                                          |
| deploy_id           | string     | The unique identifier of the deployment                                                                                                                          |
| **chain**           | **object** | The object containing data about the chain                                                                                                                       |
| chain.id            | int        | The unique identifier of the chain. Can be found here: https://chainlist.org/?chain=245022926&testnets=true&search=                                              |
| chain.name          | string     | The name of the chain                                                                                                                                            |
| **currency**        | **object** | The object containing information about the available token for this deployment                                                                                  |
| currency.ticker     | string     | The name of the token that is available on this deployment                                                                                                       |
| past_game_contracts | array      | Addresses of previous smart contracts of the game on this deployment                                                                                             |
| game_contract       | string     | The address of the current smart contract of the game on this deployment                                                                                         |
| start_block         | int        | The number of the blockchain block that will generate the first Siege on this deployment                                                                         |
| gas_token           | string     | The name of the token that is used to confirm transactions                                                                                                       |
| decimals            | int        | Determines how many decimal places are used to represent one unit of the token                                                                                   |
| explorer_link       | string     | Determines how many decimal places to display for `currency.ticker`                                                                                              |
| block_per_second    | int        | The average number of seconds for the formation of a new block of the blockchain. It is used for approximate calculation of the duration of the Battle and Siege |
| nft_marketplace     | string     | A link to the TOCD NFT collection on the marketplace of this blockchain                                                                                          |
| soon                | boolean    | TRUE - displays the inscription "SOON", shows access to the deployment. FALSE - the deployment is available for the game                                         |
| hidden              | boolean    | TRUE - do not display the deployment in the drop-down link on the site. FALSE - the deployment is displayed                                                      |

### Example

```
 {
    "_id": 2,
    "deploy_id": "2",
    "chain": { 
      "id": 4337,
      "name": "Beam Mainnet"
    },
    "currency": {
      "ticker": "BEAM"
    },
    "past_game_contracts": [],
    "game_contract": "0x0Ed8A7EBf16FBBD240D815F52DBe1c80F6663E73",
    "start_block": 1307379,
    "gas_token": "BEAM",
    "decimals": 4,
    "explorer_link": "https://snowtrace.io/",
    "block_per_second": 10,
    "nft_marketplace": "https://sphere.market/beam/collection/0x74d85442a7001e2594fb0947a6767fc1265c8c49",
    "soon": false,
    "hidden": false
  }
```
