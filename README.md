<div align="center">

# 💳 UPI MDR Tracker

### Know exactly what UPI transactions cost you, before the new rules hit.

A native Android app that calculates and tracks UPI Merchant Discount Rate (MDR) charges under India's revised NPCI framework, effective **15 October 2026**.

<img alt="Kotlin" src="https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white">
<img alt="Jetpack Compose" src="https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=for-the-badge&logo=jetpackcompose&logoColor=white">
<img alt="Material 3" src="https://img.shields.io/badge/Material%203-757575?style=for-the-badge&logo=materialdesign&logoColor=white">
<img alt="Platform" src="https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white">

<br>

<img alt="License" src="https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square">
<img alt="Status" src="https://img.shields.io/badge/status-active-brightgreen.svg?style=flat-square">
<img alt="Offline" src="https://img.shields.io/badge/works-offline-orange.svg?style=flat-square">

</div>

<br>

## The problem

On 15 October 2026, NPCI's revised UPI framework introduces merchant fees for the first time in India's UPI history. Millions of small merchants now need to know, per transaction, whether they'll be charged, how much, and whether they still qualify for the small-merchant exemption. Most have no simple way to check.

## The solution

**UPI MDR Tracker** puts the entire rulebook in a merchant's pocket — a fast, offline-first calculator paired with a running monthly tracker, so nobody gets billed by surprise.

<br>

## ✦ Features

| | |
|---|---|
| **Instant Calculator** | Enter an amount, transaction type, and category — get the exact charge, rate, and reasoning in real time. |
| **Monthly Tracker** | Logs every transaction locally and shows live progress toward the ₹1,00,000/month exemption threshold. |
| **Early Warnings** | Flags when a merchant is about to lose small-merchant exempt status, before it happens. |
| **Rules & Info** | A built-in reference screen covering every case in the new framework — no need to hunt through a PDF. |
| **Fully Offline** | Everything runs and stores locally via Room. No account, no server, no signal required. |

<br>

## ✦ MDR Rules at a Glance

*Effective 15 October 2026*

| Transaction Type | Charge |
|---|---|
| P2P (person-to-person) | **Free**, always |
| P2M up to ₹2,000 | **Free** |
| P2M above ₹2,000 (general merchant) | **0.4%**, capped at ₹300 |
| Small merchant, ≤ ₹1,00,000/month via UPI QR | **Fully exempt** |
| Essential sectors — railways, telecom, insurance, fuel, electricity, water, gas | **Flat ₹5** |
| Capital markets — mutual funds, securities, broking | **0.02%**, capped at ₹300 |

> The merchant always bears the MDR — the customer is never charged extra.
> Source: [PIB Press Release, PRID 2310586](https://www.pib.gov.in/PressReleaseDetail.aspx?PRID=2310586)

<br>

## ✦ Screenshots

<div align="center">
<em>Calculator · Monthly Tracker · Rules & Info</em>
<br><br>
<!-- Add screenshots here: drag images into this repo and reference them like below -->
<!-- <img src="screenshots/calculator.png" width="240"> <img src="screenshots/tracker.png" width="240"> <img src="screenshots/rules.png" width="240"> -->
</div>

<br>

## ✦ Tech Stack

```
Language        Kotlin
UI              Jetpack Compose · Material 3
Local Storage   Room (Entity → DAO → Database → Repository)
Architecture    Repository pattern · unidirectional data flow
```

<br>

## ✦ Get the App

**[⬇ Download app-debug.apk](./app-debug.apk)**

1. Download the APK to your Android device.
2. When prompted, allow installation from this source.
3. Open and install — no Play Store required.

<br>

## ✦ Run it yourself

```bash
git clone https://github.com/manishkshtriya/upi-mdr-tracker-android.git
```

Open in Android Studio → let Gradle sync → hit **Run** on an emulator or device.

<br>

## ✦ Roadmap

- [ ] Signed release build for Play Store distribution
- [ ] CSV export of monthly transaction history
- [ ] "Days remaining this month" pacing indicator
- [ ] Dark mode

<br>

## ✦ Related Project

A companion web app (React + Node/Express + MongoDB) implementing the same calculation engine for desktop/browser use.

<br>

---

<div align="center">

**Built by [Manish Kshtriya](https://github.com/manishkshtriya)**

If this project is useful to you, consider giving it a ⭐

</div>
