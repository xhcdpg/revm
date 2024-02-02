# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.2.1](https://github.com/xhcdpg/revm/compare/revme-v0.2.0...revme-v0.2.1) - 2024-02-02

### Added
- *(revme)* make it runnable by goevmlab ([#990](https://github.com/xhcdpg/revm/pull/990))
- EvmBuilder and External Contexts ([#888](https://github.com/xhcdpg/revm/pull/888))
- Loop call stack ([#851](https://github.com/xhcdpg/revm/pull/851))
- *(revme)* format kzg setup ([#818](https://github.com/xhcdpg/revm/pull/818))
- *(interpreter)* add more helper methods to memory ([#794](https://github.com/xhcdpg/revm/pull/794))
- derive more traits ([#745](https://github.com/xhcdpg/revm/pull/745))
- Alloy primitives ([#724](https://github.com/xhcdpg/revm/pull/724))
- implement EIP-4844 ([#668](https://github.com/xhcdpg/revm/pull/668))
- *(StateBuilder)* switch builder option from without_bundle to with_bundle ([#688](https://github.com/xhcdpg/revm/pull/688))
- alloy migration ([#535](https://github.com/xhcdpg/revm/pull/535))
- State with account status ([#499](https://github.com/xhcdpg/revm/pull/499))
- *(cancun)* EIP-5656: MCOPY - Memory copying instruction ([#528](https://github.com/xhcdpg/revm/pull/528))
- json opcode traces EIP-3155 ([#356](https://github.com/xhcdpg/revm/pull/356))
- *(Shanghai)* All EIPs: push0, warm coinbase, limit/measure initcode ([#376](https://github.com/xhcdpg/revm/pull/376))
- revm-interpreter created ([#320](https://github.com/xhcdpg/revm/pull/320))
- Export CustomPrinter insector from revm ([#300](https://github.com/xhcdpg/revm/pull/300))
- substitute web3db to ethersdb ([#293](https://github.com/xhcdpg/revm/pull/293))
- *(interpreter)* Unify instruction fn signature ([#283](https://github.com/xhcdpg/revm/pull/283))
- *(revm)* Add prevrandao field to EnvBlock ([#271](https://github.com/xhcdpg/revm/pull/271))
- Migrate `primitive_types::U256` to `ruint::Uint<256, 4>` ([#239](https://github.com/xhcdpg/revm/pull/239))
- *(revm, revme)* gas inspector ([#222](https://github.com/xhcdpg/revm/pull/222))

### Fixed
- *(eip4844)* Pass eth tests, additional conditions added. ([#735](https://github.com/xhcdpg/revm/pull/735))
- *(test)* Check expect exception and revm error ([#734](https://github.com/xhcdpg/revm/pull/734))
- k256 compile error ([#451](https://github.com/xhcdpg/revm/pull/451))

### Other
- *(Interpreter)* Split calls to separate functions ([#1005](https://github.com/xhcdpg/revm/pull/1005))
- *(revme)* EmptyDb Blockhash string, json-outcome flag, set prevrandao in statetest ([#994](https://github.com/xhcdpg/revm/pull/994))
- *(revme)* add recovery of address from secret key ([#992](https://github.com/xhcdpg/revm/pull/992))
- *(log)* use alloy_primitives::Log ([#975](https://github.com/xhcdpg/revm/pull/975))
- *(docs)* revme readme update ([#898](https://github.com/xhcdpg/revm/pull/898))
- simplify use statements ([#864](https://github.com/xhcdpg/revm/pull/864))
- decode KZG points directly into the buffers ([#840](https://github.com/xhcdpg/revm/pull/840))
- bump v26 revm v3.5.0 ([#765](https://github.com/xhcdpg/revm/pull/765))
- tag v25, revm v3.4.0 ([#755](https://github.com/xhcdpg/revm/pull/755))
- BLOBBASEFEE opcode ([#721](https://github.com/xhcdpg/revm/pull/721))
- Never inline the prepare functions ([#712](https://github.com/xhcdpg/revm/pull/712))
- *(deps)* bump bytes from 1.4.0 to 1.5.0 ([#707](https://github.com/xhcdpg/revm/pull/707))
- make `impl Default for StateBuilder` generic ([#690](https://github.com/xhcdpg/revm/pull/690))
- *(deps)* bump walkdir from 2.3.3 to 2.4.0 ([#692](https://github.com/xhcdpg/revm/pull/692))
- *(cfg)* convert chain_id from u256 to u64 ([#693](https://github.com/xhcdpg/revm/pull/693))
- Revert "feat: alloy migration ([#535](https://github.com/xhcdpg/revm/pull/535))" ([#616](https://github.com/xhcdpg/revm/pull/616))
- spell check ([#615](https://github.com/xhcdpg/revm/pull/615))
- avoid unnecessary allocations ([#581](https://github.com/xhcdpg/revm/pull/581))
- clippy and fmt ([#568](https://github.com/xhcdpg/revm/pull/568))
- optimize stack usage for recursive `call` and `create` programs ([#522](https://github.com/xhcdpg/revm/pull/522))
- *(deps)* bump hashbrown from 0.13.2 to 0.14.0 ([#519](https://github.com/xhcdpg/revm/pull/519))
- Bump v24, revm v3.3.0 ([#476](https://github.com/xhcdpg/revm/pull/476))
- *(deps)* bump ruint from 1.7.0 to 1.8.0 ([#465](https://github.com/xhcdpg/revm/pull/465))
- Release v23, revm v3.2.0 ([#464](https://github.com/xhcdpg/revm/pull/464))
- Release v22, revm v3.1.1 ([#460](https://github.com/xhcdpg/revm/pull/460))
- v21, revm v3.1.0 ([#444](https://github.com/xhcdpg/revm/pull/444))
- bump all
- remove gas blocks ([#391](https://github.com/xhcdpg/revm/pull/391))
- *(deps)* bump bytes from 1.3.0 to 1.4.0 ([#355](https://github.com/xhcdpg/revm/pull/355))
- Bump v20, changelog ([#350](https://github.com/xhcdpg/revm/pull/350))
- Cleanup imports ([#348](https://github.com/xhcdpg/revm/pull/348))
- includes to libs ([#338](https://github.com/xhcdpg/revm/pull/338))
- Creating revm-primitives, revm better errors and db components  ([#334](https://github.com/xhcdpg/revm/pull/334))
- Correct typo ([#282](https://github.com/xhcdpg/revm/pull/282))
- Integer overflow while calculating the remaining gas in GasInspector ([#287](https://github.com/xhcdpg/revm/pull/287))
- native bits ([#278](https://github.com/xhcdpg/revm/pull/278))
- *(release)* Bump revm and precompiles versions
- Bump primitive_types. Add statetest spec
- Bump revm to v2.3.0
- typos ([#263](https://github.com/xhcdpg/revm/pull/263))
- *(eth/test)* Added OEF spec for tests. Skip HighGasPrice ([#261](https://github.com/xhcdpg/revm/pull/261))
- Bump revm v2.1.0 ([#224](https://github.com/xhcdpg/revm/pull/224))
# v0.1.0
date: 18.12.2021

Initial release. statetest are done, other things I have just started working on.