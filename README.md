# Ontario Verify App

Open source repository for Ontario's official app (Ontario Verify) that is used for verifying COVID-19 vaccine certificates.
- [Overview](#overview)
- [Local setup](#local-setup)
- [Contributing](#contributing)
- [License](#license)

## Overview
This is a React Native app and designed to work well on both Android and iOS devices. 

## Local setup
#### 1. Clone the repository
```bash
git clone https://github.com/ongov/OntarioVerify
```

#### 2. Install dependencies
```bash
cd OntarioVerify
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
yarn run-android
```
##### android
```bash
yarn run-android
```

##  Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.

##  License
