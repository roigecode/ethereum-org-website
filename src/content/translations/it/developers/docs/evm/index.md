---
title: Macchina virtuale Ethereum (EVM)
description: Introduzione alla macchina virtuale Ethereum e al suo ruolo per quanto riguarda stato, transazioni e Smart Contract.
lang: it
---

La creazione di istanze fisiche dell’EVM non può essere paragonata allo scrivere codice per puntare a un cloud o a un’onda dell'oceano, ma _esiste_ come entità singola gestita da migliaia di computer collegati, che eseguono un client Ethereum.

Il protocollo Ethereum stesso esiste unicamente allo scopo di garantire un funzionamento continuo, ininterrotto e immutabile di questa speciale macchina a stati. È l'ambiente in cui sono presenti tutti gli account Ethereum e gli Smart Contract. In qualsiasi blocco della catena, Ethereum ha uno, e solo uno, stato "canonico", e la EVM è ciò che definisce le regole per calcolare un nuovo stato valido da blocco a blocco.

## Prerequisiti {#prerequisites}

Per comprendere l'EVM, è richiesta una conoscenza di base dei termini comuni dell'informatica, come ad esempio [byte](https://wikipedia.org/wiki/Byte), [memoria](https://wikipedia.org/wiki/Computer_memory) e [stack](<https://wikipedia.org/wiki/Stack_(abstract_data_type)>). Sarebbe anche utile conoscere i concetti di crittografia/blockchain, quali le [funzioni hash](https://wikipedia.org/wiki/Cryptographic_hash_function), il [proof-of-work](https://wikipedia.org/wiki/Proof_of_work) e l'[albero di Merkle](https://wikipedia.org/wiki/Merkle_tree).

## Dal libro mastro alla macchina a stati {#from-ledger-to-state-machine}

Per descrivere blockchain come Bitcoin, viene spesso utilizzata l'analogia con un "libro mastro distribuito", che permette l'esistenza di una valuta decentralizzata utilizzando strumenti base della crittografia. Una criptovaluta si comporta come una "normale" valuta per via delle regole che decidono cosa si può e cosa non si può fare per modificare il libro mastro. Ad esempio, un indirizzo Bitcoin non può spendere più Bitcoin di quanti ne abbia ricevuti in precedenza. Queste regole sono alla base di tutte le transazioni su Bitcoin e di molte altre blockchain.

Ethereum ha la sua valuta nativa (Ether), che segue quasi esattamente le stesse regole intuitive, ma consente anche una funzione molto più potente: [gli smart contract](/developers/docs/smart-contracts/). Per questa caratteristica più complessa, è necessaria un'analogia più complessa. Invece di essere un libro mastro distribuito, Ethereum è una [macchina di stato distribuita](https://wikipedia.org/wiki/Finite-state_machine). Lo stato di Ethereum è una grande enorme struttura di dati che contiene non solo tutti gli account e i saldi, ma una _macchina a stati_, che puiò cambiare da blocco a blocco in base a un set predefinito di regole, e che può eseguire codice macchina arbitrario. Le regole specifiche di cambio stato da blocco a blocco sono definite dall'EVM.

![Ddiagramma che mostra la composizione dell'EVM](./evm.png) _Diagramma adattato da [Ethereum EVM illustrated](https://takenobu-hs.github.io/downloads/ethereum_evm_illustrated.pdf)_

## La funzione di transizione di stato di Ethereum {#the-ethereum-state-transition-function}

L'EVM si comporta come una funzione matematica: dato un input, produce un output deterministico. Quindi è più utile descrivere formalmente Ethereum come avente una **funzione di transizione di stato**:

```
Y(S, T)= S'
```

Dato un vecchio stato valido `(S)` e un nuovo set di transazioni valide `(T)`, la funzione di transizione di stato di Ethereum `Y(S, T)` produce un nuovo stato di output valido `S'`

### Stato {#state}

Nell'ambito di Ethereum, lo stato è un'enorme struttura di dati chiamata [albero di Merkle Patricia modificato](/developers/docs/data-structures-and-encoding/patricia-merkle-trie/), che tiene tutti gli [account](/developers/docs/accounts/) collegati tramite hash e riducibili a un singolo hash radice memorizzato sulla blockchain.

### Transazioni {#transactions}

Le transazioni sono istruzioni provenienti dagli account firmate crittograficamente. Esistono due tipi di transazioni: quelle che danno luogo a chiamate di messaggio e quelle che invece danno luogo alla creazione di contratti.

La creazione di contratti porta alla creazione di nuovo account contratto contenente bytecode di [Smart Contract](/developers/docs/smart-contracts/anatomy/) compilato. Quando un altro account fa una chiamata di messaggio a questo contratto, esegue il suo bytecode.

## Istruzioni dell'EVM {#evm-instructions}

L'EVM viene eseguita come una [macchina a stack](https://wikipedia.org/wiki/Stack_machine) con una profondità di 1024 elementi. Ogni elemento è una parola di 256 bit, scelta per la facilità d'uso con la crittografia a 256 bit (come gli hash Keccak-256 o le firme secp256k1).

Durante l'esecuzione, l'EVM mantiene una _memoria_ transitoria (sotto forma di array di byte con indirizzamento a parola), che non rimane persistente tra le transazioni.

I contratti, invece, contengono un trie di _memorizzazione_ di Merkle Patricia (sotto forma di array di parole con indirizzamento a parola), associato all'account in questione e parte dello stato globale.

Il bytecode compilato dello smart contract compilato viene eseguito come numero di [opcode](/developers/docs/evm/opcodes) dell'EVM, che eseguono operazioni stack standard come `XOR`, `AND`, `ADD`, `SUB`, ecc. L'EVM implementa anche una serie di operazioni di stack specifiche della blockchain, come `INDIRIZZO`, `SALDO`, `BLOCKHASH`, etc.

![Diagramma che mostra dove occorre carburante nelle operazioni dell'EVM](../gas/gas.png) _Diagramma adattato da [Ethereum EVM illustrated](https://takenobu-hs.github.io/downloads/ethereum_evm_illustrated.pdf)_

## Implementazioni dell'EVM {#evm-implementations}

Tutte le implementazioni dell'EVM devono rispettare le specifiche descritte nello Yellowpaper di Ethereum.

Nei 7 anni di storia di Ethereum, l'EVM ha subito diverse revisioni, ed esistono diverse implementazioni dell'EVM in vari linguaggi di programmazione.

Tutti i [client Ethereum](/developers/docs/nodes-and-clients/#execution-clients) includono un'implementazione dell'EVM. Inoltre, esistono diverse implementazioni standalone, tra cui:

- [Py-EVM](https://github.com/ethereum/py-evm) - _Python_
- [evmone](https://github.com/ethereum/evmone) - _C++_
- [ethereumjs-vm](https://github.com/ethereumjs/ethereumjs-vm) - _JavaScript_
- [eEVM](https://github.com/microsoft/eevm) - _C++_

## Letture consigliate {#further-reading}

- [Ethereum Yellowpaper](https://ethereum.github.io/yellowpaper/paper.pdf)
- [Jellopaper o KEVM: Semantica di EVM in K](https://jellopaper.org/)
- [The Beigepaper](https://github.com/chronaeon/beigepaper)
- [Ethereum Virtual Machine Opcodes](https://www.ethervm.io/)
- [Una breve introduzione alla documentazione di Solidity](https://docs.soliditylang.org/en/latest/introduction-to-smart-contracts.html#index-6)

## Argomenti correlati {#related-topics}

- [Carburante](/developers/docs/gas/)
