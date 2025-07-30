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
  - Trust Provider Signer는 서버 측 컴포넌트롤 EUDI Wallet 생태계에서 Trust List 및 관련 객체에 대한 서명 역할을 수행
  - 주요 기능
    * Trust List에 대한 디지털 서명 생성
      - EU 내 각 Member State 또는 신뢰 가능한 기관이 제공하는 Trust List(e.g. trusted issuers, verifier lists 등)를 전자적으로 서명
      - EUDI Wallet이나 다른 서비스가 해당 리소스의 무결성과 출처 신뢰성을 검증할 수 있도록 보장
    * Trust Anchor에 대한 서명 발행
      - Trust Provider가 인증한 Trust Anchor (예: 인증된 Issuer의 공개 키 등)에 대해 서명
      - 이 Anchor가 공식적이고 검증된 신뢰 주체임을 증명
    * API 제공
      - 외부에서 신뢰할 수 있는 객체를 등록하거나, 서명 요청을 전송할 수 있도록 RESTful API 제공
    * 서명 프로파일 및 키 관리
      - 서명을 위한 키는 내부적으로 PKCS#11 (HSM) 또는 파일 기반 Keystore를 통해 관리
      - 서명 알고리즘: ECDSA, RSA, 등 유럽 eIDAS 프로파일에 부합하는 형식 사용
  

## Usecase of EUDI Wallet

<img width="658" height="384" alt="Image" src="https://github.com/user-attachments/assets/ab973f2a-2093-4f36-bae2-dba48bd2331c" />
