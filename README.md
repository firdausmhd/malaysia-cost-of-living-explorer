# Malaysia Cost-of-Living Explorer

An interactive report on Malaysian inflation from 2021 to September 2026, built from open data published by the Department of Statistics Malaysia (DOSM).

**Live report:** https://firdausmhd.github.io/malaysia-cost-of-living-explorer/

## Problem

Inflation headlines say prices are "easing", but they do not show where the pressure sits or what it adds up to over several years.

## What it shows

- Headline and core inflation, 2021 to 2025
- The cumulative rise in the cost of a basket of goods since 2021 (about 9%)
- Inflation by spending category, with a switch between 2024, 2025 and the change between them
- Urban and rural inflation
- Selected states against the national rate in 2025
- Malaysia against other ASEAN countries in 2025

## Findings

- Annual inflation has fallen every year since 2022: 3.3%, 2.5%, 1.8%, then 1.4% in 2025. Monthly readings in 2026 have stayed near 1.8% to 1.9%.
- Slower inflation does not mean lower prices. The price index rose from 123.1 in 2021 to 134.6 in 2025, so the same basket costs about 9.3% more.
- In 2025, personal care, insurance and financial services, and restaurants rose fastest. Information and communication was the main category getting cheaper.

## Data and method

- Source: DOSM annual Consumer Price Index analyses, 2022 to 2025, published on [OpenDOSM](https://open.dosm.gov.my/data-catalogue/cpi_annual_inflation) under CC BY 4.0.
- Figures were keyed in from those releases and the index changes were checked against the stated percentages.
- The +9.3% cumulative rise is calculated from the annual price index (134.6 / 123.1).
- Category comparisons cover 2024 and 2025 only, because DOSM changed its category classification in 2024.
- 2026 monthly readings are year-on-year rates reported in the press, so they are not directly comparable with annual averages.

## Limitations

- Core inflation for 2025 and urban/rural inflation for 2021 were not in the releases used, so those points are missing.
- State figures cover only the states named in DOSM's 2025 analysis.
- To refresh or extend the data, pull the `cpi_annual_inflation` dataset from OpenDOSM.

## Tech

Single-file HTML, CSS and JavaScript with hand-drawn SVG charts. No build step and no dependencies apart from the IBM Plex fonts loaded from Google Fonts. Supports light and dark mode.

## Run it locally

Open `index.html` in a browser.
