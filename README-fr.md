# L’application VérifOuverte 

Répertoire du code source libre pour l’application officielle de l’Ontario **(VérifOntario)** qui est utilisée pour vérifier les certificats de vaccination contre la COVID-19.
- [Aperçu](#aperçu)
- [Configuration locale](#configuration-locale)
- [Rules, Public keys and Minimum mandatory app version](#rules-public-keys-and-minimum-mandatory-app-version)
- [Vulnerability disclosure policy](#vulnerability-disclosure-policy)

## Aperçu
Il s’agit d’une application de technologie React Native conçue pour être compatible avec les appareils Android et iOS. 

VérifOuverte offre aux entreprises et aux organismes un moyen rapide, facile et fiable de numériser et de vérifier que les visiteurs sont entièrement vaccinés.

L’application numérise le code QR affiché sur un certificat de vaccination délivré par le gouvernement de l’Ontario.  

Après avoir numérisé un code QR, l’entreprise ou l’organisme verra : une coche verte indiquant qu’il répond aux exigences en matière de vaccination, un X rouge pour un certificat non valide, ou un avertissement jaune indiquant que le code QR ne peut être lu.

VérifOuverte numérise également la plupart des codes QR délivrés par les gouvernements de la Colombie-Britannique, du Québec et du Yukon. [Refer to our list of onboarded issuers and their associated public keys](https://files.ontario.ca/apps/verify/verifyRulesetON.json). Des fonctionnalités à l’échelle nationale sont en cours de développement et seront intégrées au fur et à mesure que les provinces délivreront des certificats de vaccination munis des codes QR de la carte santé SMART®.


## Configuration locale

#### 1. Clonez le repositoire

```bash
git clone https://github.com/ongov/OpenVerify
```

#### 2. Installez les dépendances

```bash
cd OpenVerify
yarn install
```

#### 3. Installez les modules

```bash
yarn run update:pods
```

#### 4. Configuration de l’environnement

```bash
cp .env.template .env
```
La variable d’environnement API_URL est dirigée vers l'URL hébergeant les règles et les clés publiques and minimum mandatory app version. Ajustez la valeur en conséquence

#### 5. Démarrer l’application (mode développement)

##### iOS

```bash
yarn run-ios
```
##### Android

```bash
yarn run-android
```

## Rules, Public keys and Minimum mandatory app version

These are the public access endpoints for:

[Rules](https://files.ontario.ca/apps/verify/verifyRulesetON.json)

[Public keys](https://files.ontario.ca/apps/verify/publicKeys.json)

[Minimum mandatory app version](https://files.ontario.ca/apps/verify/minimumVersion.json)

## Vulnerability disclosure policy

[Politique de divulgation des vulnérabilités de VérifOntario | COVID-19 (coronavirus) en Ontario ](https://covid-19.ontario.ca/fr/verif-divulgation-vulnerabilite)
