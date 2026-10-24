# JIO-FARM — Security-safe GitHub Actions setup

This repository contains the original `jio_gemini_farm.py` source for code review and **safe GitHub Actions demonstrations**. The upstream project is [dlupo707-ship-it/jio-farm-action](https://github.com/dlupo707-ship-it/jio-farm-action).

## What works

- `.github/workflows/test.yml`: simple GitHub Actions test.
- `.github/workflows/farm.yml`: **SAFE DEMO ONLY**. Checks Python syntax and creates downloadable demo output files without fetching SMS, accessing Firebase panels, sending OTPs, logging in, or claiming any promotion.
- `jio_gemini_farm.py`: original source retained for static review. **The live farming code is not executed by these workflows.**

## Run the safe demo

1. Go to **Actions** in this repository.
2. Choose **Jio Farm - Safe Demo (No OTP)**.
3. Click **Run workflow**.
4. Open the completed run and download the `safe-demo-results-...` artifact.

The ZIP contains:

- `fresh_links.txt`: empty, because no real promotional links were requested or collected.
- `farm_results.csv`: a demo status row indicating zero links.
- `farm.log`: diagnostic information explaining what was tested.

**Important:** A green checkmark means GitHub Actions and the static checks work. It does **not** mean Google AI Pro links were generated or any real Jio account was tested.

## বাংলা

এই Workflow শুধু GitHub Actions পরীক্ষা করে ও ডেমো রিপোর্ট বানায়। এটি অন্য কারও SMS/OTP সংগ্রহ করে না, Firebase database পড়ে না এবং Jio account-এ লগইন করে না। মূল script আলাদা আছে, কিন্তু এই workflow সেটি live চালায় না।
