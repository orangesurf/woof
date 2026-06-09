# woof 🐕

A self-custodial bitcoin wallet on [Ark](https://second.tech), in a single HTML file.

**Use it:** download [`index.html`](index.html) (or the repo ZIP) and open it in a modern browser. That's the whole install.

- Runs entirely in your browser — keys are generated locally and never leave it
- Bitcoin **mainnet** by default, signet toggle in the header
- Send and receive over Ark, Lightning, and on-chain; unified payment QR
- Optional password encrypts your recovery phrase at rest
- **Encrypted wallet backup**: one click downloads a backup file encrypted with a key derived from your recovery phrase (useless without the words). On Chrome/Brave/Edge, pick a file once and the wallet silently keeps it current. Restore = seed words + backup file.
- **Unilateral exit**: reclaim your funds on-chain with no cooperation from the Ark server (Settings → Unilateral exit). The wallet progresses the exit automatically in the background and lets you claim matured funds to any bitcoin address.
- Built on [`@secondts/bark`](https://www.npmjs.com/package/@secondts/bark), Second's official WASM SDK

⚠️ Beta software handling real bitcoin — keep amounts small. While Bark is in beta, the 12 words alone recover unspent incoming Ark payments only — funds from Lightning receives, boards, and change need the backup file too. Keep both: write down the words, keep the backup file current (the wallet shows a "backup needed" badge when it's stale).

## No warranty, no liability

This software is provided **as-is, without warranty of any kind**, express or implied. In no event shall the authors be liable for any claim, damages, or other liability — including loss of funds — arising from its use. You are solely responsible for your keys, your backups, and your bitcoin. See [LICENSE](LICENSE).
