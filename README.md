# Open Verify App 

Open source repository for Ontario's official app **(Ontario Verify)** that is used for verifying COVID-19 vaccine certificates.
- [Overview](#overview)
- [Local setup](#local-setup)

## Overview
This is a React Native app and designed to work well on both Android and iOS devices. 

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
