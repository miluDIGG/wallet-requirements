# TS8 Common Interface for reporting of Relying Parties to Data Protection Authorities

## Mål

<span style="color:var(--ds-text,#172b4d);"><span style="color:var(--ds-text,#172b4d);">Målet är att skapa och underhålla master-dokumentation över krav som ska vara spårbara ur</span> </span>TS8 Common Interface for reporting of Relying Parties to Data Protection Authorities.

## Bakgrund

N/A

## Antagande

- N/A

## Krav

<span style="color:var(--ds-text,#172b4d);">Här är en summering av krav från</span><span style="color:var(--ds-text,#172b4d);"> </span>**TS8 - Common Interface for reporting of Relying Parties to Data Protection Authorities V0.11**.



| Krav_ID  | Källans index | Sektion                   | Beskrivning 1                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Beskrivning 2 | Digg kommentar | Ej infört krav/orsak |
|----------|---------------|---------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------|----------------------|
| REQ_1156 |               | EUDIW WRP Interfaces TS08 | Article 5a (5) of the regulation (EU) No 910/2014 requires thatEuropean Digital Identity Wallets shall, in particular:(a) support common protocols and interfaces:\[...\](x) for reporting a relying party to the competent national data protection authority where an allegedly unlawful or suspicious request for data is received.                                                                                                                                                                                                                                                                                                                                                                         |               |                |                      |
| REQ_1157 |               | EUDIW WRP Interfaces TS08 | Article 7 of (EU) 2024/2982 stipulates the following:1. Wallet providers shall ensure that wallet units allow wallet users to easily report wallet-relying parties to supervisory authorities established under Article 51 of Regulation (EU) 2016/679.2. Wallet providers shall implement the protocols and interfaces for reporting wallet-relying parties in compliance with national procedural laws of the Member States.3. Wallet providers shall ensure that wallet units allow wallet users to substantiate the reports, including by attaching relevant information to identify the wallet-relying parties, and the wallet users’ claims in machine-readable format.                                  |               |                |                      |
| REQ_1158 | RPT_DPA_01    | EUDIW WRP Interfaces TS08 | When prompted by the User, a Wallet Unit SHALL provide the contact details of the DPA, which supervises the Relying Party, if available, and SHALL make it easy for the User to send a report of allegedly unlawful or suspicious Relying Party presentation requests to this DPA. If these are not available, the Wallet Unit SHALL provide the contact details of the DPA of the region in which the Wallet Provider is residing. In addition, the Wallet Unit MAY also provide contact details of other DPAs taken from the "European Data Protection Board" website (<https://www.edpb.europa.eu/about-edpb/about-edpb/members_en>), and allow the User to choose a DPA to continue the reporting process. |               |                |                      |
| REQ_1159 | RPT_DPA_02    | EUDIW WRP Interfaces TS08 | The User interface enabling a User to start the process of reporting a Wallet-relying Party to a DPA SHALL be accessible via the log provided by the Wallet Unit.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |               |                |                      |
| REQ_1160 | RPT_DPA_04    | EUDIW WRP Interfaces TS08 | Wallet providers SHALL ensure that wallet units allow wallet users to substantiate the reports, including by attaching relevant information to identify the wallet-relying parties, and the wallet users’ claims in machine-readable format.Note: The log kept by the Wallet Unit is machine-readible and specified in [TS10](https://github.com/eu-digital-identity-wallet/eudi-doc-standards-and-technical-specifications/blob/main/docs/technical-specifications/ts10-data-portability-and-download-(export).md) in order to enable data portability. An excerpt from this log therefore can be used to substantiate the report.                                                                            |               |                |                      |
| REQ_1161 | RPT_DPA_05    | EUDIW WRP Interfaces TS08 | A Wallet Unit SHALL log the initiation of a report sent to the DPA in a log file so that it can be presented to the User in the dashboard (as specified in [Topic 19](https://github.com/eu-digital-identity-wallet/eudi-doc-standards-and-technical-specifications/blob/main/docs/technical-specifications/ts8-common-interface-for-reporting-of-wrp-to-dpa.md#a2319-topic-19---user-navigation-requirements-dashboard-logs-for-transparency) and [TS10](https://github.com/eu-digital-identity-wallet/eudi-doc-standards-and-technical-specifications/blob/main/docs/technical-specifications/ts10-data-portability-and-download-(export).md)).                                                              |               |                |                      |
| REQ_1162 | RPT_DPA_06    | EUDIW WRP Interfaces TS08 | The Wallet Unit SHALL take the contact details of the DPA, which supervises the Relying Party, either (in this order) from a) included in the RPRC in the log entry, b) included in the RPAC in the log entry, c) looked up by the Wallet Unit from the RP Registry, based on the Subject of the RPAC in the log entry. The contact information includes at least one of email address, phone number, or a URL of a webform.                                                                                                                                                                                                                                                                                   |               |                |                      |
| REQ_1163 | RPT_DPA_07    | EUDIW WRP Interfaces TS08 | The text in the `subject` of the mail prepared by the Wallet Unit according to `RPT_DPA_06` SHALL clearly indicate that the purpose of the mail is to report a WRP to the DPA and state that an allegedly unlawful or suspicious request for data has been received.                                                                                                                                                                                                                                                                                                                                                                                                                                           |               |                |                      |
| REQ_1164 | RPT_DPA_08    | EUDIW WRP Interfaces TS08 | The text in the `subject` of the mail prepared by the Wallet Unit according to `RPT_DPA_06` SHOULD indicate the identity of the WRP and also an involved intermediary, if applicable, which sent the allegedly unlawful or suspicious request.                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |               |                |                      |
| REQ_1165 | RPT_DPA_09    | EUDIW WRP Interfaces TS08 | The text in the `body` of the mail prepared by the Wallet Unit according to `RPT_DPA_06` SHALL contain the necessary information to identify the WRP and also an involved intermediary, if applicable, and allows that the request can be handled by the DPA in an efficient manner.                                                                                                                                                                                                                                                                                                                                                                                                                           |               |                |                      |

<table xmlns:ac="http://www.atlassian.com/schema/confluence/4/ac/">
<colgroup>
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
<col style="width: 20%" />
</colgroup>
<thead>
<tr class="header">
<th>#</th>
<th>Titel</th>
<th>Användarberättelse</th>
<th>Betydelse</th>
<th>Anteckningar</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>1.0</td>
<td>Kort identifierare för berättelsen</td>
<td>Beskriv användaren och vad de försöker uppnå</td>
<td>Måsten</td>
<td><ul>
<li>Ytterligare hänsynstaganden eller anmärkningsvärda referenser (länkar, ärenden)</li>
</ul></td>
</tr>
<tr class="even">
<td>2</td>
<td></td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>

## Användarinteraktion och design

Inkludera eventuella modeller, diagram eller visuella ritningar som relaterar till dessa krav.

## Frågor

Nedan finns en lista över frågor att ta itu med som resultat av detta kravdokument:

| Fråga                                                             | Resultat                         |
|-------------------------------------------------------------------|----------------------------------|
| (T.ex. Hur kan vi göra användare mer medvetna om denna funktion?) | Kommunicera det fattade beslutet |

## Gör inte

- Lista diskuterade funktioner som är utanför tillämpningsområdet eller som kan återupptas till i en senare utgåva.
