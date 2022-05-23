## API Report File for "web3-net"

> Do not edit this file. It is a report generated by [API Extractor](https://api-extractor.com/).

```ts
import { DataFormat } from 'web3-common';
import { DEFAULT_RETURN_FORMAT } from 'web3-common';
import { HexString } from 'web3-utils';
import { NumberTypes } from 'web3-common';
import { Web3Context } from 'web3-core';
import { Web3RequestManager } from 'web3-core';

// @public (undocumented)
export function getId<ReturnFormat extends DataFormat>(
	web3Context: Web3Context<Web3NetAPI>,
	returnFormat: ReturnFormat,
): Promise<NumberTypes[ReturnFormat['number']]>;

// @public (undocumented)
function getId_2(requestManager: Web3RequestManager<Web3NetAPI>): Promise<string>;

// @public (undocumented)
export function getPeerCount<ReturnFormat extends DataFormat>(
	web3Context: Web3Context<Web3NetAPI>,
	returnFormat: ReturnFormat,
): Promise<NumberTypes[ReturnFormat['number']]>;

// @public (undocumented)
function getPeerCount_2(requestManager: Web3RequestManager<Web3NetAPI>): Promise<string>;

// @public (undocumented)
export const isListening: (web3Context: Web3Context<Web3NetAPI>) => Promise<boolean>;

// @public (undocumented)
function isListening_2(requestManager: Web3RequestManager<Web3NetAPI>): Promise<boolean>;

declare namespace rpcMethods {
	export { getId_2 as getId, getPeerCount_2 as getPeerCount, isListening_2 as isListening };
}
export { rpcMethods };

// @public (undocumented)
class Web3Net extends Web3Context<Web3NetAPI> {
	// (undocumented)
	getId<ReturnFormat extends DataFormat = typeof DEFAULT_RETURN_FORMAT>(
		returnFormat?: ReturnFormat,
	): Promise<NumberTypes[ReturnFormat['number']]>;
	// (undocumented)
	getPeerCount<ReturnFormat extends DataFormat = typeof DEFAULT_RETURN_FORMAT>(
		returnFormat?: ReturnFormat,
	): Promise<NumberTypes[ReturnFormat['number']]>;
	// (undocumented)
	isListening(): Promise<boolean>;
}
export { Web3Net };
export default Web3Net;

// @public (undocumented)
export type Web3NetAPI = {
	net_version: () => string;
	net_peerCount: () => HexString;
	net_listening: () => boolean;
};

// (No @packageDocumentation comment for this package)
```