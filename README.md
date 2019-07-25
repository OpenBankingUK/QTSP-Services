# Availability of QTSP services relating to PSD2 eIDAS certificates
Public repo for sharing information about availability of QTSP services relating to PSD2 eIDAS certificates.

## Disclaimer

This repo can be updated by any GitHub user, and therefore the information on this page can change at any time without notice. Any participant who edits this repo must act in good faith and only provide information that is accurate to the best of their knowledge. Open Banking Limited (OBIE) is making this repo available to help the ecosystem to share general information. OBIE is not responsible for ensuring the accuracy of any information or contents contained on this repo. It is not intended to amount to advice. OBIE does not endorse or recommended any service listed in this repo. OBIE does not take any liability for any loss any direct or indirect or consequential loss, any loss of goodwill, reputation or opportunity, any loss of profits or revenue  whether direct or indirect as a result or attributed to information or content on this repo.

## Official list of QTSPs

Please also refer to [https://webgate.ec.europa.eu/tl-browser/](https://webgate.ec.europa.eu/tl-browser/)

## List of QTSP services

| QTSP Name | Country | Website | Other Contact Details | Test QWAC | Prod QWAC | Test QsealC | Prod QsealC | Process to obtain | HSM requirements / support | Notes |
|--------------|-----------------|-----------------------------------------------|------------------------|--------------------------------|------------------------|--------------------------------|-----------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------|------------------------------------------|-|
| Actalis S.p.A. | Italy | https://www.actalis.it | info@actalis.it | Y | Y | Y | Y | Test: fill a form, generate CSR(s) and send to CA, certificate(s) delivered via email. Production: fill a form and sign it digitally or have it authenticated by a notary (further options available), generate CSR(s) and send to CA along with CSR(s). For QWACs, prove control of domains by the usual methods used for plain SSL Server certificates. Wait for CA to carry out all checks, including those on claimed PSD2 authorization and roles. Certificate(s) delivered via email. Detailed procedure delivered to applicants on request. | N ||||| 
| Aruba Posta Elettronica Certificata S.p.A. | Italy | https://www.pec.it ||||||||||
| Bank-Verlag | Germany |||||||||||
| Bundesdruckerei GmbH (D-Trust GmbH) | Germany | https://www.bdr.de/psd2 | psd2@bdr.de | Y | Y | Y | Y | Test: fill a form, generate CSR (for QWAC and QSealC as soft token) and send to CA.  QWAC and QSealC as soft token delivered via email, seal card sent per post. Production: fill a form,  generate CSR (for QWAC and QSealC as soft token), sign an order and have requester be identified by a notary or German embassy (further options available). For QWACs, prove control of domains by the usual methods used for plain SSL Server certificates. Wait for CA to carry out all checks, including those on claimed PSD2 authorization and roles. QWAC delivered via email, seal card sent per post. | No. QWAC and QSealC on smart card available on May 16th. QSealC as soft token (without QcSSCD QcStatement) scheduled for June 2019. |||
| Buypass AS | Norway | [https://www.buypass.com/products/eseal--and-enterprise-certificate/eidas-qualified-certificates](https://www.buypass.com/products/eseal--and-enterprise-certificate/eidas-qualified-certificates) | support@buypass.com | Y | Aiming to begin issuing in May/June 2019 | Y | Aiming to begin issuing in May/June 2019 | *Test*: Fill in a form, generate a CSR and return. Certs delivered by email. *Production*: Fill form, generate CSR, and verify identity. In the Nordics the delivery and ID check are done by the national post. Working on similar solutions for other parts of Europe.  By the end of this year hope to have a certified video solution for the ID check. | QSealC does not require a HSM/SmartCard.  You are free to use AWS or any other cloud services.   | |
| CERTSIGN S.A. | Romania |||||||||||
| Evrotrust Technologies JSC | Bulgaria |||||||||||
| FINA - Financijska agencija | Croatia |||||||||||
| First certification authority, a.s. | Czech Republic |||||||||||
| HARICA | Greece | [https://www.harica.gr](https://www.harica.gr) | support@harica.gr | Y | May 2019 | Y | May 2019 | **Test**: Simulate the production process but without validation of Legal representative. Just submit a request form. PSD2 certificate will be delivered by email. **Production**: Submit a request form, generate CSR, verify identity of Applicant, PSD2 roles and Authorization ID. | No Qualified Signature/Seal Creation Device (QSCD) is required for Qualified Certificate for **Advanced** electronic seal. QSCD ***is required*** only for Qualified Certificate for ***Qualified*** electronic seal. | |
| InfoCert S.p.A. | Italy |||||||||||
| Krajowa Izba Rozliczeniowa S.A. | Poland |||||||||||
| LuxTrust S.A. | Luxembourg |||||||||||
| **Microsec** Micro Software Engineering & Consulting Private Company Limited by Shares | Hungary | https://e-szigno.hu/en/pki-services/psd2-specific-solutions.html | sales@microsec.hu | Y <br /> (since Mar 2018) | Y <br /> (since Dec 2018) | Y <br /> (since Mar 2018) | Y <br /> (since Dec 2018) | **Test**: submit request [form](https://srv.e-szigno.hu/psd2_test), await email from Microsec for unlimited testing access. <br /> <br /> **Production**: generate CSRs, submit request [form](https://srv.e-szigno.hu/ssl_ev_psd_eng), await email from Microsec with further instructions for identity verification. | HSM or QSCD is **not required**. | Certificates conform to ETSI TS 119495. <br /> <br /> **Test** access includes unlimited number of test certificates with customizable content, test CRL and test OCSP services. <br /> <br /> **Production** certs identity validation options: face-to-face, qualified e-signature, public notary, mobile RA (for travel fee). |
| MULTICERT - Serviços de Certificação Electrónica S.A. | Portugal |https://www.multicert.com/en/products/advanced-solutions/psd2-certificates/ <br />Online request form: https://www.multicert.com/3ws/psd2?execution=e1s1&lang=en_US|psd2@multicert.com English, Portuguese, Spanish, French|Y|Y|Y|Y|Options for F2F validation: (1) in person; (2) notarized with Hague Apostille; (3) “home delivery” at request; (4) “PSD2 workshops”|HSMs are not required. QSealC is issued without QcSSCD QcStatement.|Test certificates include OCSP and CRL services.||
| NETLOCK Informatics and Network Privacy services Limited Company | Hungary |||||||||||
| První certifikační autorita, a.s. | Czech Republic | https://www.ica.cz/Whitelist-en | sales@ica.cz | Y | Y | Y | Y | Test certificates can be issued online. Prod certificates can be issued online based on the required documents, or  based on a personal visit. | No | OB are aware of a European TPP that has acquired a Prod eIDAS cert from this QTSP, and has passported into the UK||



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
