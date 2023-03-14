# ChapterDao



> GreekDao ChapterDao Contract. 





## Methods

### adminMint

```solidity
function adminMint(uint256 _mintAmount) external nonpayable
```



*Mints tokens for the contract&#39;s ambassador.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _mintAmount | uint256 | The amount of tokens to mint. Note: Only the ambassador is allowed to call this function. |

### adminWithdraw

```solidity
function adminWithdraw(address _user) external nonpayable
```



*Allows the ambassador to withdraw the dividends of a user.Reverts if the user has no tokens or if the transfer fails.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _user | address | The address of the user whose dividends are being withdrawn. |

### ambassadorId

```solidity
function ambassadorId() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### ambassadorTransfer

```solidity
function ambassadorTransfer(address from, address to, uint256 tokenId) external nonpayable
```



*Allows the ambassador to transfer a token from one address to another.Reverts if the recipient address is invalid.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | The address of the token sender. |
| to | address | The address of the token recipient. |
| tokenId | uint256 | The ID of the token being transferred. |

### approve

```solidity
function approve(address to, uint256 tokenId) external nonpayable
```



*See {IERC721-approve}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| to | address | undefined |
| tokenId | uint256 | undefined |

### balanceOf

```solidity
function balanceOf(address owner) external view returns (uint256)
```



*See {IERC721-balanceOf}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### baseURI

```solidity
function baseURI() external view returns (string)
```



*Base URI for computing {tokenURI}. If set, the resulting URI for each token will be the concatenation of the `baseURI` and the `tokenId`. Empty by default, can be overriden in child contracts.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | string | undefined |

### burn

```solidity
function burn(uint256 _tokenId) external nonpayable
```



*Burns the specified token.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _tokenId | uint256 | uint256 ID of the token to burn. |

### calcFee

```solidity
function calcFee(uint256 _amount) external view returns (uint256)
```



*Calculates the transaction fee for a given amount.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _amount | uint256 | The amount to calculate the fee for. |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | The transaction fee for the given amount. |

### distributeBackFunds

```solidity
function distributeBackFunds(uint256 amount) external nonpayable
```



*Allows the ambassador to distribute funds to the token holders as dividends.Reverts if there are no tokens to distribute, if the supply is zero, or if the transfer fails.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| amount | uint256 | The amount of tokens to be distributed as dividends. |

### dividendEarned

```solidity
function dividendEarned(address _user) external view returns (uint256)
```



*Returns the dividends earned of the `_user`*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _user | address | User address to query |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | amount Dividends earned in eth |

### downgrade

```solidity
function downgrade(uint256 _tokenId, uint8 _level) external nonpayable
```



*Downgrades a token&#39;s level by the given amount.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _tokenId | uint256 | The ID of the token being downgraded. |
| _level | uint8 | The number of levels to downgrade the token. Note: Only the ambassador is allowed to call this function. |

### emergancyWithdraw

```solidity
function emergancyWithdraw() external nonpayable
```



*Allows the ambassador to withdraw all the ETH held in the contract.*


### factory

```solidity
function factory() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### getAmbassadorAddress

```solidity
function getAmbassadorAddress() external view returns (address)
```



*Returns the address of the ambassador associated with the contract.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | The address of the ambassador associated with the contract. |

### getAmbassadorId

```solidity
function getAmbassadorId() external view returns (uint256)
```



*Returns the ambassador ID of the contract.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | The ambassador ID of the contract. |

### getApproved

```solidity
function getApproved(uint256 tokenId) external view returns (address)
```



*See {IERC721-getApproved}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### getFeePercent

```solidity
function getFeePercent() external view returns (uint256)
```



*Returns the percentage of transaction fees taken by the contract.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | The percentage of transaction fees taken by the contract. |

### getFeeTo

```solidity
function getFeeTo() external view returns (address)
```



*Returns the address where transaction fees are sent.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | The address where transaction fees are sent. |

### getFeeToken

```solidity
function getFeeToken() external view returns (address)
```



*Returns the address of the token used for paying transaction fees.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | The address of the token used for paying transaction fees. |

### getSnapshot

```solidity
function getSnapshot() external view returns (string)
```



*Returns the link to the contract snapshot.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | string | The link to the contract snapshot. |

### initialize

```solidity
function initialize(string name_, string symbol_, string baseURI_, uint256 ambassadorId_, address schoolDao_) external nonpayable
```



*Initializes the contract with the given name, symbol, base URI, ambassador ID, and school DAO address.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| name_ | string | The name of the token. |
| symbol_ | string | The symbol of the token. |
| baseURI_ | string | The base URI of the token. |
| ambassadorId_ | uint256 | The ID of the ambassador. |
| schoolDao_ | address | The address of the school DAO. Note: Only the factory is allowed to call this function. |

### isApprovedForAll

```solidity
function isApprovedForAll(address owner, address operator) external view returns (bool)
```



*See {IERC721-isApprovedForAll}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | undefined |
| operator | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### isWhitelisted

```solidity
function isWhitelisted(address) external view returns (bool)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### level

```solidity
function level(uint256) external view returns (uint8)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint8 | undefined |

### mintPrice

```solidity
function mintPrice() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### mintWhiteList

```solidity
function mintWhiteList() external nonpayable
```



*Mints a single token to the caller if they are whitelisted and have not already claimed a token. Note: This function can only be called if the sale is active.*


### name

```solidity
function name() external view returns (string)
```



*See {IERC721Metadata-name}.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | string | undefined |

### ownerOf

```solidity
function ownerOf(uint256 tokenId) external view returns (address)
```



*See {IERC721-ownerOf}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### recoverERC20

```solidity
function recoverERC20(address tokenAddress, uint256 tokenAmount) external nonpayable
```



*Recovers a specific ERC20 token.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddress | address | address Address of the ERC20 token to recover. |
| tokenAmount | uint256 | uint256 Amount of the ERC20 token to recover. |

### recoverERC721

```solidity
function recoverERC721(address tokenAddress, uint256 tokenID) external nonpayable
```



*Recovers a specific ERC721 token.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenAddress | address | address Address of the ERC721 token to recover. |
| tokenID | uint256 | uint256 ID of the ERC721 token to recover. |

### safeTransferFrom

```solidity
function safeTransferFrom(address from, address to, uint256 tokenId) external nonpayable
```



*See {IERC721-safeTransferFrom}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | undefined |
| to | address | undefined |
| tokenId | uint256 | undefined |

### safeTransferFrom

```solidity
function safeTransferFrom(address from, address to, uint256 tokenId, bytes _data) external nonpayable
```



*Transfers a token from one address to another using the safe transfer mechanism.Reverts if the transfer is not authorized.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | The address of the token sender. |
| to | address | The address of the token recipient. |
| tokenId | uint256 | The ID of the token being transferred. |
| _data | bytes | Optional additional data with no specified format. |

### saleActive

```solidity
function saleActive() external view returns (bool)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### schoolDao

```solidity
function schoolDao() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### setApprovalForAll

```solidity
function setApprovalForAll(address operator, bool approved) external nonpayable
```



*See {IERC721-setApprovalForAll}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| operator | address | undefined |
| approved | bool | undefined |

### setMintPrice

```solidity
function setMintPrice(uint256 _price) external nonpayable
```



*Sets the price of minting a token.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _price | uint256 | The new price of minting a token. Note: Only the ambassador is allowed to call this function. |

### setSaleStatus

```solidity
function setSaleStatus(bool _saleStatus) external nonpayable
```



*Sets the sale status of the contract.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _saleStatus | bool | A boolean flag indicating the new sale status. Note: Only the ambassador is allowed to call this function. |

### setSnapshot

```solidity
function setSnapshot(string _link) external nonpayable
```



*Sets the link to a snapshot of the contract.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _link | string | The link to the snapshot. Note: Only the ambassador is allowed to call this function. |

### setURI

```solidity
function setURI(string _uri) external nonpayable
```



*Sets the base URI link for tokens.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _uri | string | The new base URI link for tokens. Note: Only the ambassador is allowed to call this function. |

### supportsInterface

```solidity
function supportsInterface(bytes4 interfaceId) external view returns (bool)
```



*See {IERC165-supportsInterface}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| interfaceId | bytes4 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### symbol

```solidity
function symbol() external view returns (string)
```



*See {IERC721Metadata-symbol}.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | string | undefined |

### tokenURI

```solidity
function tokenURI(uint256 tokenId) external view returns (string)
```



*See {IERC721Metadata-tokenURI}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| tokenId | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | string | undefined |

### tokensOfOwner

```solidity
function tokensOfOwner(address owner) external view returns (uint256[])
```



*Returns an array of token IDs owned by `owner`. This function scans the ownership mapping and is O(`totalSupply`) in complexity. It is meant to be called off-chain. This function is compatiable with ERC721AQueryable.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| owner | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256[] | undefined |

### totalCapitalCollected

```solidity
function totalCapitalCollected() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### totalCapitalRepaid

```solidity
function totalCapitalRepaid() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### totalSupply

```solidity
function totalSupply() external view returns (uint256)
```



*See {IERC721Enumerable-totalSupply}.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### transferFrom

```solidity
function transferFrom(address from, address to, uint256 tokenId) external nonpayable
```



*See {IERC721-transferFrom}.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| from | address | undefined |
| to | address | undefined |
| tokenId | uint256 | undefined |

### upgrade

```solidity
function upgrade(uint256 _tokenId, uint8 _level) external nonpayable
```



*Upgrades a token&#39;s level by the given amount.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _tokenId | uint256 | The ID of the token being upgraded. |
| _level | uint8 | The number of levels to upgrade the token. Note: Only the ambassador is allowed to call this function. |

### userClaimableBalance

```solidity
function userClaimableBalance(address _address) external view returns (uint256)
```



*Returns the claimable balance for a user.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _address | address | The user&#39;s address. |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | The user&#39;s claimable balance. |

### userTotalBalance

```solidity
function userTotalBalance(address _address) external view returns (uint256)
```



*Returns the total balance of a user.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _address | address | The user&#39;s address. |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | The total balance of the user. |

### whitelistClaimed

```solidity
function whitelistClaimed(address) external view returns (bool)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### whitelistForMint

```solidity
function whitelistForMint(address[] _addresses, bool _toggle) external nonpayable
```



*Whitelists or un-whitelists addresses for minting tokens.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _addresses | address[] | An array of addresses to whitelist or un-whitelist. |
| _toggle | bool | A boolean flag indicating whether to whitelist or un-whitelist the addresses. Note: Only the ambassador is allowed to call this function. |

### withdraw

```solidity
function withdraw() external nonpayable
```



*Allows a token holder to withdraw their dividends.Reverts if the caller has no tokens or if the transfer fails.*


### withdrawFunds

```solidity
function withdrawFunds() external nonpayable
```



*Withdraws funds from the contract, transferring a fee to the designated recipient and the remaining balance to the caller. Note: Only the ambassador is allowed to call this function.*




## Events

### AdminBurn

```solidity
event AdminBurn(uint256 _tokenId, uint256 _blockNumber)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _tokenId  | uint256 | undefined |
| _blockNumber  | uint256 | undefined |

### AdminWithdrawlMade

```solidity
event AdminWithdrawlMade(address indexed withdrawer, uint256 amount)
```



*Emitted when `withdrawer` withdraws the `amount` of dividends earned*

#### Parameters

| Name | Type | Description |
|---|---|---|
| withdrawer `indexed` | address | undefined |
| amount  | uint256 | undefined |

### Approval

```solidity
event Approval(address indexed owner, address indexed approved, uint256 indexed tokenId)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| owner `indexed` | address | undefined |
| approved `indexed` | address | undefined |
| tokenId `indexed` | uint256 | undefined |

### ApprovalForAll

```solidity
event ApprovalForAll(address indexed owner, address indexed operator, bool approved)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| owner `indexed` | address | undefined |
| operator `indexed` | address | undefined |
| approved  | bool | undefined |

### DividendDeposited

```solidity
event DividendDeposited(uint256 _blockNumber, uint256 _amount)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _blockNumber  | uint256 | undefined |
| _amount  | uint256 | undefined |

### FundsWithdrawn

```solidity
event FundsWithdrawn(uint256 _blockNumber, uint256 _balance)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _blockNumber  | uint256 | undefined |
| _balance  | uint256 | undefined |

### SaleStatusSet

```solidity
event SaleStatusSet(bool _saleStatus)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _saleStatus  | bool | undefined |

### Transfer

```solidity
event Transfer(address indexed from, address indexed to, uint256 indexed tokenId)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| from `indexed` | address | undefined |
| to `indexed` | address | undefined |
| tokenId `indexed` | uint256 | undefined |

### WithdrawlMade

```solidity
event WithdrawlMade(address indexed withdrawer, uint256 amount)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| withdrawer `indexed` | address | undefined |
| amount  | uint256 | undefined |



## Errors

### DepositFailed

```solidity
error DepositFailed()
```






### HoldingZeroTokens

```solidity
error HoldingZeroTokens()
```






### InvalidInputZeroAddress

```solidity
error InvalidInputZeroAddress()
```






### NoTokensToDistribute

```solidity
error NoTokensToDistribute()
```






### NonexistentToken

```solidity
error NonexistentToken(uint256 _tokenId)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _tokenId | uint256 | undefined |

### NotAmbassador

```solidity
error NotAmbassador()
```






### NotFactory

```solidity
error NotFactory()
```






### NotWhitelisted

```solidity
error NotWhitelisted()
```






### SaleNotActive

```solidity
error SaleNotActive()
```






### SupplyIsZero

```solidity
error SupplyIsZero()
```






### UnauthorizedTransfer

```solidity
error UnauthorizedTransfer()
```






### WhitelistClaimed

```solidity
error WhitelistClaimed()
```






### WithdrawlFailed

```solidity
error WithdrawlFailed()
```







