# MuesliSwap Token Verification 🪙✔

The official repository to verify your token @ AdaMuesliSwap  
Being verified will get your token listed in the [featured section](https://ada.muesliswap.com/markets/featured) of Muesliswap.

## Fees
Using the Community section, it is possible to trade **any** token on Cardano **without** being verified.  
However, verification will give you more visibility and increase the trust of the community.  
To account for processing each verifiaction manually and to prevent people from spamming request we require a verification fee of **50 ADA**. 

## How can I get verified?
Submit a Pull Request to this repository that that adds three things: 

📄 A correct JSON token description in the [tokens](tokens) folder  
🖼️ An image for the token in the [images](images) folder.  
💸 A comment, with the transaction id showing you submitted 50 ADA to the [Payment address](addr1vysu7s7uvdr09w7mz8uz7mj4pw8qp57rja58jlfpag7zzsqq49n6f)

The folder `tokens` contains [JSON](https://en.wikipedia.org/wiki/JSON) files that describe each verified token listed at AdaMuesliSwap.
Each file contains information on what the coin is called, its supply and other important information.
The name of the file is the string `<policy_id>.<name>.json`.

In the folder `images`, an image is listed for each token that should be traded.
This is required so that an image can be displayed for the token on the website.
The name of the file is the string `<policy_id>.<name>.png`.

### Contents of the listing file

| Field | Description | Example |
| ----- | ----------- | ------- |
| `policyId` | The policy id of the token | `8a1cfae21368b8bebbbed9800fec304e95cce39a2a57dc35e2e3ebaa` |
| `name` | The asset name of the token | `MILK` |
| `symbol` | A trading symbol of the token | `MILK` or `CDOG` |
| `website` | Homepage of the corresponding token | `https://ada.muesliswap.com` |
| `description` | A very short description of the token | `Your favorite pre-sale token, making you stronger` |
| `totalSupply` | The total minted amount of the token | `100000000` |
| `amounts` | A list of integers of the trade size options |`[1000, 5000, 10000]` |
| `decimalPlaces` | The number of decimal places when displaying the token. | ADA has 6 decimal places. 1 token = 1 Lovelace = 0.000001 ADA, displayed as "6 zeroes" |

See [tokens/8f52f6a88acf6127bc4758a16b6047afc4da7887feae121ec217b75a.SNOW.json](tokens/8f52f6a88acf6127bc4758a16b6047afc4da7887feae121ec217b75a.SNOW.json) for an example file.
Also check the token on [cardanoscan.io](https://cardanoscan.io/token/8a1cfae21368b8bebbbed9800fec304e95cce39a2a57dc35e2e3ebaa4d494c4b) if you are unsure about some values.
