# Open Verify App 

Open source repository for Ontario's official app **(Verify Ontario)** that is used for verifying COVID-19 vaccine certificates.
- [Overview](#overview)
- [Local setup](#local-setup)
- [Rules, Public keys and Minimum mandatory app verion](#Rules, Public keys and Minimum mandatory version)
- [Vulnerability disclosure policy](#vulnerability-disclosure-policy)

## Overview
This is a React Native app and designed to work well on both Android and iOS devices. 

Verify Ontario gives businesses and organizations a quick, easy and trusted way to scan and confirm that visitors are fully vaccinated. 

The app scans the QR code on an Ontario government-issued vaccine certificate.  

After scanning a QR code, the business or organization will see: a green checkmark indicating that it meets vaccine requirements, a red X for an invalid certificate, or a yellow warning indicating that the QR code cannot be read. 

Verify Ontario also scans most government issued QR codes from British Columbia and Québec. Nation-wide capabilities are in development and will be added as provinces issue proof of vaccination with SMART® Health Card QR codes. 


## Local setup

#### 1. Clone the repository

```bash
git clone https://github.com/ongov/OpenVerify
```

#### 2. Install dependencies

```bash
cd OpenVerify
yarn install
```

#### 3. Install pods

```bash
yarn run update:pods
```

#### 4. Environment config

```bash
cp .env.template .env
```
API_URL env variable points to the URL hosting the rules and public keys. Adjust the value accordingly.

#### 5. Launch app (development mode)

##### iOS

```bash
yarn run-ios
```
##### Android

```bash
yarn run-android
```

## Rules, Public keys and Minimum mandatory version

These are the public access endpoints for:

#### [Rules and Public keys](https://files.ontario.ca/apps/verify/verifyRulesetON.json)


#### [Minimum mandatory version] (https://files.ontario.ca/apps/verify/minimumVersion.json)

## Vulnerability disclosure policy

https://covid-19.ontario.ca/verify-vulnerability-disclosure
