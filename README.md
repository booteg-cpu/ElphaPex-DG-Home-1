# ElphaPex DG Home 1

SD firmware based on the **original ElphaPex DG-Home1 V1.0.5**, with automatic return to the primary mining pool and original thermal protection.

[Download v14.0.0](https://github.com/booteg-cpu/ElphaPex-DG-Home-1/releases/tag/v14.0.0) · [Русский](RELEASE_NOTES_RU.txt) · [中文](RELEASE_NOTES_ZH.txt)

## Pool recovery

When mining on Pool 2 or Pool 3, the firmware returns to Pool 1 after three successful recovery checks. The switch briefly interrupts mining. Supports `stratum+tcp`; TLS pool compatibility is not confirmed.

## Installation

1. Download the release ZIP and verify the supplied SHA-256.
2. Extract `DGH_Home1_v14.0.0_SD_8GB.img` and write it with Rufus in DD mode.
3. Use a card with at least **8,053,063,680 bytes** of actual capacity and 512-byte logical sectors. Some nominal 8 GB cards are smaller. GPT is prepared for this size; compatibility with other capacities is not confirmed. Partitions do not expand automatically.
4. Power off the miner before inserting the SD card. Keep a working card for recovery.
5. Boot and enter your own pool and network settings.

This is an SD boot image, not an internal eMMC update. Pool and Wi-Fi settings are empty. Root account: `root` / `admin`; change the password immediately. The web interface may still display V1.0.5.

The image has been tested on an ASIC and is in long-term use.

## Donations

[![Sponsor](https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ea4aaa?logo=githubsponsors)](https://github.com/sponsors/booteg-cpu)

```text
TRX: TBhFJKbh7E7o2ezh3x8RwJiAoPVKF94aVw
Ethereum (ETH): 0x0cAd5052B15b06aF62140e329A6684FaC27fB4C0
BTC: bc1qprxtn8j6y7adjnc0vw2jgnyj48eg39y65phfr2
Solana (SOL): CCHEzR6hVU3JigCGUdB278gGc2L21Vu2smQZHiNoQuCY
```

Original firmware and bundled software retain their respective rights and licenses.
