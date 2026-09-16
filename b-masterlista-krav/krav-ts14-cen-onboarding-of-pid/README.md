# Krav - TS14 CEN Onboarding of PID

## Mål

<span style="color:var(--ds-text,#172b4d);"><span style="color:var(--ds-text,#172b4d);">Målet är att skapa och underhålla master-dokumentation över krav som ska vara spårbara ur</span> </span><span style="color:var(--ds-text,#172b4d);">TS14 CEN onboarding of PID.</span>

## Bakgrund

N/A

## Antagande

N/A

## Krav

<span style="color:var(--ds-text,#172b4d);">Här är en summering av krav från</span><span style="color:var(--ds-text,#172b4d);"> </span>**<span style="color:var(--ds-text,#172b4d);">TS14 CEN onboarding of PID.</span>**

<span style="color:var(--ds-text,#172b4d);">OBS! TS14 har bytts ut till att handla om </span>Specification for the implementation of Zero-Knowledge Proofs based on multi-message signatures in the EUDI Wallet. Krav nedan finns det inte längre någon TS som hanterar och måste antas inte längre gälla.

| Krav_ID  | Källans index | Sektion        | Beskrivning 1                                                                                                                                                                                                                                                  | Beskrivning 2                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  | Digg kommentar                                   | Ej infört krav/orsak |     |
|----------|---------------|----------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|--------------------------------------------------|----------------------|-----|
| REQ_1203 |               | prCEN/TS 18098 | The User should be enforced to set the Wallet Unit authentication factor(s) (knowledge-based, possession-based or inherent)                                                                                                                                    |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |                                                  |                      |     |
| REQ_1204 |               | prCEN/TS 18098 | The Wallet Unit shall inform the User about all possibilities for the storage of the PID allowed by the Wallet Solution for the used device. In addition the Wallet Unit shall allow the User to select the options he wants to be applied by the Wallet Unit. | NOTE 1 With this requirement, the User can decide - if the Wallet Unit supports several possibilities for the PID storage (local, remote, in the WSCD, encrypted in the device, etc.), which one the User wants to use.NOTE 2 Nevertheless, the choice made by the User could be not compliant with the PID Provider policy. Therefore, it could lead either the PID Provider to abort the on-boarding or the User to reconsider his choice to fit the PID Provider policy.NOTE 3 In case the User’s device does not fulfil the requirement for local storage of the PID, but the Wallet Provider offers the possibility to store them in e.g. a cloud or remote server endowed with Hardware Security Module (HSM), the Wallet Unit will not work in an offline scenario, where the system has no connectivity to the cloud or remote server. | No support for this requirement is found in ARF. |                      |     |
| REQ_1205 |               | prCEN/TS 18098 | The Wallet Provider shall ensure that the Wallet Unit carries out all operations of the on-boarding process in a manner ensuring end to end communication with data protected in integrity, authenticity and confidentiality,                                  | NOTE 1 This requirement implies establishment of secure communication on top of TLS.NOTE 2 The encryption is performed independently of the operating system. This requirement addresses compromised devices where even the HTTPS stack on rooted devices cannot be trusted.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |                                                  |                      |     |

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
<td>1</td>
<td></td>
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
