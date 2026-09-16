# UPI MDR Tracker

<p align="center">
  <strong>A native Android app that calculates and tracks UPI Merchant Discount Rate (MDR) charges under India's new NPCI framework, effective 15 October 2026.</strong>
</p>

<p align="center">
  <img alt="Kotlin" src="https://img.shields.io/badge/Kotlin-7F52FF?style=flat&logo=kotlin&logoColor=white">
  <img alt="Jetpack Compose" src="https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat&logo=jetpackcompose&logoColor=white">
  <img alt="Material 3" src="https://img.shields.io/badge/Material%203-757575?style=flat&logo=materialdesign&logoColor=white">
  <img alt="Platform" src="https://img.shields.io/badge/Platform-Android-3DDC84?style=flat&logo=android&logoColor=white">
  <img alt="License" src="https://img.shields.io/badge/License-MIT-blue.svg">
</p>

---

## Overview

On 15 October 2026, NPCI's revised UPI merchant charge framework goes live in India, introducing MDR (Merchant Discount Rate) fees on certain merchant transactions for the first time. Most small business owners have no easy way to know what they'll actually be charged, or whether they qualify for exemption.

**UPI MDR Tracker** solves that with two tools in one app: an instant calculator for any transaction, and a monthly tracker that watches cumulative receipts against the exemption threshold, so merchants never get an unexpected bill.

## Features

- **Instant Calculator** — enter an amount, transaction type, and category to see the exact MDR charge, rate applied, and the reason behind it.
- **Monthly Tracker** — logs transactions locally and visualizes progress toward the ₹1,00,000/month small-merchant exemption limit, with early warnings before it's lost.
- **Rules & Info** — a built-in reference screen covering every rule in the new framework.
- **Fully offline** — all data stored locally via Room; no account or internet connection required.

## MDR Rules (effective 15 Oct 2026)

| Transaction | Charge |
|---|---|
| P2P (person-to-person) | Always free |
| P2M up to ₹2,000 | Free |
| P2M above ₹2,000 (general merchants) | 0.4%, capped at ₹300 |
| Small merchant, ≤ ₹1,00,000/month via UPI QR | Fully exempt |
| Essential sectors — railways, telecom, insurance, fuel, electricity, water, gas | Flat ₹5 |
| Capital markets — mutual funds, securities, broking | 0.02%, capped at ₹300 |

> The merchant always bears the MDR — the customer is never charged extra.
>
> Source: PIB Press Release, PRID 2310586

## Tech Stack

| Layer | Technology |
|---|---|
| Language | Kotlin |
| UI | Jetpack Compose, Material 3 |
| Local storage | Room (Entity / DAO / Database / Repository) |
| Architecture | Repository pattern, unidirectional data flow |

## Download

Grab the latest debug build directly: app-debug.apk (in this repo)

Install steps:
1. Download the APK to your Android device.
2. When prompted, allow installation from this source.
3. Open and install.

## Building from Source

Open the project in Android Studio, let Gradle sync complete, then hit Run on an emulator or physical device.

## Roadmap

- Signed release build for Play Store distribution
- CSV export of monthly transaction history
- "Days remaining this month" pacing indicator
- Dark mode

## Related

Companion web app (React + Node/Express + MongoDB) implementing the same calculation engine.

## License

MIT
