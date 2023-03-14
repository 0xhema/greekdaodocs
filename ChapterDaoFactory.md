# ChapterDaoFactory



> GreekDao ChapterDao Factory Contract. 





## Methods

### INIT_CODE_PAIR_HASH

```solidity
function INIT_CODE_PAIR_HASH() external view returns (bytes32)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bytes32 | undefined |

### allCollections

```solidity
function allCollections(uint256) external view returns (address)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### allCollectionsIndex

```solidity
function allCollectionsIndex(uint256) external view returns (address)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### collectionCount

```solidity
function collectionCount() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### createChapterDao

```solidity
function createChapterDao(string name_, string symbol_, string baseURI_, address ambassador_, address schoolDao_) external nonpayable returns (address payable collection)
```



*Creates a new ChapterDao collection with the given parameters.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| name_ | string | The name of the new ChapterDao collection. |
| symbol_ | string | The symbol of the new ChapterDao collection. |
| baseURI_ | string | The base URI for the metadata of the new ChapterDao collection&#39;s NFTs. |
| ambassador_ | address | The address of the ambassador to mint the first NFT to. |
| schoolDao_ | address | The address of the SchoolDao contract to link the new ChapterDao collection to. |

#### Returns

| Name | Type | Description |
|---|---|---|
| collection | address payable | The address of the newly created ChapterDao collection. Note: Only the contract owner is allowed to call this function. |

### feePercent

```solidity
function feePercent() external view returns (uint256)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | undefined |

### feeTo

```solidity
function feeTo() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### feeToken

```solidity
function feeToken() external view returns (address)
```






#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### getCollections

```solidity
function getCollections(uint256 _cursor, uint256 _length) external view returns (address[])
```



*Returns an array of ChapterDao collection addresses.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _cursor | uint256 | The starting index of the collections to retrieve. |
| _length | uint256 | The maximum number of collections to retrieve. |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address[] | An array of ChapterDao collection addresses. |

### getFeePercent

```solidity
function getFeePercent() external view returns (uint256)
```



*Returns the current percentage fee charged for each transaction.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | uint256 | The current fee percentage. |

### getFeeTo

```solidity
function getFeeTo() external view returns (address)
```



*Returns the address where transaction fees are sent.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | The current fee recipient address. |

### getFeeToken

```solidity
function getFeeToken() external view returns (address)
```



*Returns the address of the token used for paying transaction fees.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | The address of the current fee token. |

### isCollection

```solidity
function isCollection(address) external view returns (bool)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | bool | undefined |

### owner

```solidity
function owner() external view returns (address)
```



*Returns the address of the current owner.*


#### Returns

| Name | Type | Description |
|---|---|---|
| _0 | address | undefined |

### renounceOwnership

```solidity
function renounceOwnership() external nonpayable
```



*Leaves the contract without owner. It will not be possible to call `onlyOwner` functions anymore. Can only be called by the current owner. NOTE: Renouncing ownership will leave the contract without an owner, thereby removing any functionality that is only available to the owner.*


### setFeePercent

```solidity
function setFeePercent(uint256 _feePercent) external nonpayable
```



*Sets the percentage fee charged for each transaction.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _feePercent | uint256 | The new fee percentage to set. Note: Only the contract owner is allowed to call this function. |

### setFeeTo

```solidity
function setFeeTo(address _feeTo) external nonpayable
```



*Sets the address where transaction fees are sent.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _feeTo | address | The new address to set as the fee recipient. Note: Only the contract owner is allowed to call this function. |

### setFeeToken

```solidity
function setFeeToken(address _feeToken) external nonpayable
```



*Sets the address of the token used for paying transaction fees.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| _feeToken | address | The address of the token to set as the new fee token. Note: Only the contract owner is allowed to call this function. |

### transferOwnership

```solidity
function transferOwnership(address newOwner) external nonpayable
```



*Transfers ownership of the contract to a new account (`newOwner`). Can only be called by the current owner.*

#### Parameters

| Name | Type | Description |
|---|---|---|
| newOwner | address | undefined |



## Events

### CollectionCreated

```solidity
event CollectionCreated(string name, string symbol, string baseURI_, uint256 length, address indexed collection)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| name  | string | undefined |
| symbol  | string | undefined |
| baseURI_  | string | undefined |
| length  | uint256 | undefined |
| collection `indexed` | address | undefined |

### OwnershipTransferred

```solidity
event OwnershipTransferred(address indexed previousOwner, address indexed newOwner)
```





#### Parameters

| Name | Type | Description |
|---|---|---|
| previousOwner `indexed` | address | undefined |
| newOwner `indexed` | address | undefined |



