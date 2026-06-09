# woof 🐕

A self-custodial bitcoin wallet on [Ark](https://second.tech), in a single HTML file.

**Use it:** download [`index.html`](index.html) (or the repo ZIP) and open it in a modern browser. That's the whole install.

- Runs entirely in your browser — keys are generated locally and never leave it
- Bitcoin **mainnet** by default, signet toggle in the header
- Send and receive over Ark, Lightning, and on-chain; unified payment QR
- Optional password encrypts your recovery phrase at rest
- Built on [`@secondts/bark`](https://www.npmjs.com/package/@secondts/bark), Second's official WASM SDK

⚠️ Beta software handling real bitcoin — keep amounts small. Your wallet lives in this browser profile; the 12-word recovery phrase is the only backup.
