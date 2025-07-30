This repository was created to investigate and organizae information and source code for open source digital wallets, include the EUDI wallet. 

# EUDI Wallet

* [Open-source code of the wallet now published](https://ec.europa.eu/digital-building-blocks/sites/display/EUDIGITALIDENTITYWALLET/Open-source+code+of+the+wallet+now+published)

## Self-Sovereign Ecosystem

<img width="786" height="330" alt="Image" src="https://github.com/user-attachments/assets/f2003d85-0023-478e-8e5c-b146c627445b" />

## EUDI Wallet Reference Implementation

EUDI 지갑 참조 구현은 다양한 비즈니스에서 재 사용할 수 있도록 컴포넌트로 구성된 모듈화된 구조를 따른다. 그러므로 점진적으로 진화 개발되어 여러 프로젝트에 재사용할 수 있다.
참조 구현은 다음과 같은 구성 요소를 제공힌다. 

### 프레임워크에 필요한 라이브러리 및 기타 소프트웨어 구성 요소

##### Coordinator Layer between the UI app and Wallet libraries
* Android: Wallet Core 
* iOS: Wallet Kit

##### Proximity Sharing Libraries
* mDoc Data Transfer
* mDoc Security
* mDoc Data Model

##### Remote Presentaion Libraries
* Presentaiton Exchange
* SOIPv2 & OpenID4VP prtocols
* SD-JWT

##### Issuing Libraries
* OpenID4VCI

##### Wallet Data Storage and Cryptographic Management Libraries
* mDoc Document Storage

##### Wallet UI and demo App

##### Verifier App and Services
* Web Verifier
* Restful API (web-services)

###### Issuing App and service
* OpenID4VCI Issuer(Python)
* OpenID4VCI Issuer (Kotrin)

###### Signing Apps and Services
* Trust Providr Signier




## Usecase of EUDI Wallet

<img width="658" height="384" alt="Image" src="https://github.com/user-attachments/assets/ab973f2a-2093-4f36-bae2-dba48bd2331c" />
