# Portfolio Visualiser and Optimiser

A Python-based tool that visualizes security price forecasts, optimizes portfolios for maximum Sharpe ratio, and integrates sentiment analysis to generate trading signals.

[![Watch the video](https://img.shields.io/badge/YouTube-Project%20Demo-red)](https://youtu.be/wpi0ueHl9Fg)

---

## Table of Contents

1. [Overview](#overview)  
2. [Features](#features)  
3. [Project Structure](#project-structure)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [License](#license)

---

## Overview

This project combines multiple financial modeling techniques:
- **Geometric Brownian Motion** and **Monte Carlo simulations** to forecast security prices.
- **Portfolio Optimization** aimed at maximizing the Sharpe ratio for specified target returns.
- **Bollinger Bands** over projected price paths to identify potential trade entries and exits.
- **Sentiment Analysis** on textual data (including Elon Musk’s tweets) to derive buy, sell, or hold signals.

The result is a **dynamic portfolio visualizer** that can help investors, data scientists, and quants better understand and manage their investments.

---

## Features

1. **Algorithm for Security Price Forecasting**  
   - Utilizes Geometric Brownian Motion and Monte Carlo simulations for more accurate short- to medium-term price predictions.

2. **Asset Allocation & Sharpe Ratio Optimization**  
   - Implements a model to optimize asset weights while respecting user-defined return targets.

3. **Bollinger Bands Application**  
   - Overlays Bollinger Bands on projected security price paths, providing crucial insights for trade timing.

4. **Sentiment Analysis Model**  
   - Scrapes web data (e.g., news, social media) to produce a quantitative sentiment score, which translates into buy, sell, or hold signals.

5. **Elon Musk’s Tweets Analysis**  
   - Conducts sentiment analysis on Elon Musk’s historical tweets, potentially detecting influences on specific stock movements.

---

## Project Structure

Below is an overview of the key files included. Click any of the links to view detailed information:

- **[understand.md](./understand.md)** – Additional project background and context.
- **[tp3final(112).md](./tp3final(112).md)** – Main script or notes explaining the core functionalities.
- **[bands_gbm.md](./bands_gbm.md)** – Detailed explanation and usage of Bollinger Bands with Geometric Brownian Motion.
- **[sentimentanalysis.md](./sentimentanalysis.md)** – Outline of the sentiment analysis pipeline.
- **[optimise.md](./optimise.md)** – Sharpe ratio optimization and portfolio allocation methodologies.
- **[elon.md](./elon.md)** – Details on the Elon Musk tweets dataset and its analysis.
- **[brownianmotion.md](./brownianmotion.md)** – Mathematical background on Geometric Brownian Motion.
- **[simulate.md](./simulate.md)** – Explanation of the Monte Carlo simulation process.
- **[cmu_112_graphics.md](./cmu_112_graphics.md)** – Visualization and UI notes (if relevant).

### Data Files
- **[TweetsElonMusk.csv](./TweetsElonMusk.csv)** – Dataset containing Elon Musk's tweets for sentiment analysis.

### Images
![Homepage](https://user-images.githubusercontent.com/118176527/206685708-daf513a4-5071-4cfc-b749-d9553bf101c8.jpg)  
![Resize Final](https://user-images.githubusercontent.com/118176527/206685691-5184cc4c-f8c3-4325-80e8-e296027afc3f.jpg)

Feel free to customize any directories and filenames according to your local project structure.

---

## Installation

1. **Clone this repository**:
   ```bash
   git clone https://github.com/yourusername/yourrepository.git
   cd yourrepository

