# Availability of QTSP services relating to PSD2 eIDAS certificates
Public repo for sharing information about availability of QTSP services relating to PSD2 eIDAS certificates.

## Disclaimer

This repo can be updated by any GitHub user, and therefore the information on this page can change at any time without notice. Any participant who edits this repo must act in good faith and only provide information that is accurate to the best of their knowledge. Open Banking Limited (OBIE) is making this repo available to help the ecosystem to share general information. OBIE is not responsible for ensuring the accuracy of any information or contents contained on this repo. It is not intended to amount to advice. OBIE does not endorse or recommended any service listed in this repo. OBIE does not take any liability for any loss any direct or indirect or consequential loss, any loss of goodwill, reputation or opportunity, any loss of profits or revenue  whether direct or indirect as a result or attributed to information or content on this repo.

## Official list of QTSPs

Please also refer to [https://webgate.ec.europa.eu/tl-browser/](https://webgate.ec.europa.eu/tl-browser/)

## List of QTSP services

| QTSP Name | Country | Website | Other Contact Details | Test QWAC | Prod QWAC | Test QsealC | Prod QsealC | Process to obtain | HSM requirements / support | Notes |
|--------------|-----------------|-----------------------------------------------|------------------------|--------------------------------|------------------------|--------------------------------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------|------------------------------------------|-|
| Aruba Posta Elettronica Certificata S.p.A. | Italy |||||||||||
| Bank-Verlag | Germany |||||||||||
| Bundesdruckerei GmbH (D-Trust GmbH) | Germany |||||||||||
| Buypass AS | Norway | [https://www.buypass.com/products/eseal--and-enterprise-certificate/eidas-qualified-certificates](https://www.buypass.com/products/eseal--and-enterprise-certificate/eidas-qualified-certificates) | support@buypass.com | Y | Aiming to begin issuing in May/June 2019 | Y | Aiming to begin issuing in May/June 2019 | *Test*: Fill in a form, generate a CSR and return. Certs delivered by email. *Production*: Fill form, generate CSR, and verify identity. In the Nordics the delivery and ID check are done by the national post. Working on similar solutions for other parts of Europe.  By the end of this year hope to have a certified video solution for the ID check. | QSealC does not require a HSM/SmartCard.  You are free to use AWS or any other cloud services.   | |
| CERTSIGN S.A. | Romania |||||||||||
| Evrotrust Technologies JSC | Bulgaria |||||||||||
| FINA - Financijska agencija | Croatia |||||||||||
| First certification authority, a.s. | Czech Republic |||||||||||
| InfoCert S.p.A. | Italy |||||||||||
| Krajowa Izba Rozliczeniowa S.A. | Poland |||||||||||
| LuxTrust S.A. | Luxembourg |||||||||||
| Microsec Micro Software Engineering & Consulting Private Company Limited by Shares | Hungary |||||||||||
| MULTICERT - Serviços de Certificação Electrónica S.A. | Portugal ||psd2@multicert.com|Y|Pending update of ETSI TS 119 495|Y|Pending update of ETSI TS 119 495|Options for F2F validation: (1) in person; (2) notarized with Hague Apostille; (3) “home delivery” at request; (4) “PSD2 workshops”|HSMs are not required. QSealC is issued without QcSSCD QcStatement.|Test certificates include OCSP and CRL services.||
| NETLOCK Informatics and Network Privacy services Limited Company | Hungary |||||||||||





## Data dictionary

| Field | Description |
| ----- | ----------- |
| QTSP Name | Full legal name of QTSP as per official list |
| Country | Country where QTSP is located |
| Website | Direct link to QTSP's PSD2 eIDAS services page |
| Other Contact Details | e.g. email, phone |
| Test QWAC | availability, e.g. Y, N or planned date |
| Prod QWAC | availability, e.g. Y, N or planned date |
| Test QsealC | availability, e.g. Y, N or planned date |
| Prod QsealC | availability, e.g. Y, N or planned date) |
| Process to obtain | e.g. can these certificates be procured online, or does this have to be in person | 
| HSM requirements / support | e.g. are HSMs required, and if so, which cloud HSMs are supported |
| Notes | any other notes |

## How to contribute

Any person with a GitHub account can contribute to this repo at [https://github.com/OpenBankingUK/QTSP-Services/](https://github.com/OpenBankingUK/QTSP-Services/) via a pull request. Before submitting your pull requests, make sure you follow these steps:

* Create a pull request, see `contributing via pull request guide`.
* Check that your changes are consistent with the current `.md` style. For example, using the correct headings depths.
* Ensure you have read the Contributor agreement below.

## Contributing via pull request guide

* Create a personal fork of this repository by clicking on the fork button on the top of this page. This will create a copy of this repository in your account.
* Clone the fork on your local machine `git clone "url you just copied"`.
* If you created your fork a while ago be sure to pull upstream changes into your local repository.
* Branch from master and create a new branch to work on using `hotfix/` or `feature/` as the prefix `git checkout -b "feature/<add-your-new-branch-name>"`
* Make necessary changes and commit those changes as needed.
* Push your branch to your own fork on Github, the remote origin.
* From your fork open a pull request in the correct branch and target `master`.

Once the pull request is approved and merged by OBIE you can pull the changes from upstream to your local repo and delete your extra branch(es) if required.

## Contributor agreement

By submitting a pull request you agree that contributions to the project are governed by the [MIT License and copyright statement](https://www.openbanking.org.uk/open-licence/). You also acknowledge that OBIE are under no obligation to use or incorporate your contributions into this project.
