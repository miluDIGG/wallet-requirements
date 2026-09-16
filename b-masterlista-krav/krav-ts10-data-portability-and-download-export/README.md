# Krav - TS10 Data Portability and Download (Export)

## Mål

<span style="color:var(--ds-text,#172b4d);"><span style="color:var(--ds-text,#172b4d);">Målet är att skapa och underhålla master-dokumentation över krav som ska vara spårbara ur</span> </span>TS10 Data Portability and Download (Export).

## Bakgrund

<span style="color:var(--ds-text,#333333);">The TS10 document specifies the common format and data set for the transaction log and the Migration Object, as well as protocols related to exporting those objects from a Wallet Unit and importing to another one in a backup, recovery and migration scenarios, as required by the </span><a href="https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=celex%3A32024R1183" style="text-decoration: underline;" rel="nofollow">European Digital Identity Regulation (EU 2024/1183)</a><span style="color:var(--ds-text,#333333);"> and </span><a href="https://eur-lex.europa.eu/eli/reg_impl/2024/2979/oj/eng" style="text-decoration: underline;" rel="nofollow">CIR 2024/2979</a><span style="color:var(--ds-text,#333333);">.</span>

<span style="color:var(--ds-text,#333333);">In TS10 includes specifications of data class objects, thus not spcifying many requirements. Related requirements can be found in ARF,  article 5a(4)(f) and (g) of the \[European Digital Identity Regulation\] and Article 9 and 13 of the \[CIR on Integrity and Core Functionalities\].</span>

## Antagande

- N/A

## Krav

<span style="color:var(--ds-text,#172b4d);">Här är en summering av krav från</span><span style="color:var(--ds-text,#172b4d);"> </span>**TS10 Data Portability and Download (Export) V1.0**

OBS! Senaste versionen är V1.2. Där finns hela datamodellen för transaktions logg och migreringsobjekt specificerad. Det bör diskuteras hur kraven lämpligast preciceras. Kanske är det här bättre hänvisa till lämplig nivå inom **TS10 Data Portability and Download (Export).**

| Krav_ID | Källans index | Sektion | Beskrivning 1                                                                                                                                                                                                                                                                                                                                                                                                                                                    | Beskrivning 2 | Digg kommentar | Ej infört krav/orsak |
|---------|---------------|---------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|----------------|----------------------|
| Tbd     |               |         | The `TransactionLogObject` object shall be in \[JWE\] format; the corresponding \[JWE\] ciphertext object shall be encoded as a \[JSON\] object.                                                                                                                                                                                                                                                                                                                 |               |                |                      |
| Tbd     |               |         | The `MigrationObject` object shall be in \[JWE\] format; the corresponding \[JWE\] ciphertext is composed of the `TransactionLog` and `ListOfCredential` objects, both encoded as \[JSON\] objects.                                                                                                                                                                                                                                                              |               |                |                      |
| Tbd     |               |         | För definition av objekt och attribut se källan - Technical Specification 10, Data Portability and Download (Export)The following algorithms are mandatory for \[JWE\] objects encryption:PBES2-HS256+A128KW, as specified in \[JWA\] and \[PKCS#5\] - to derive the key encryption key from the User's password/passphrase and encrypt the content encryption key,A128GCM, as specified in \[JWA\] - for the content encryption with the content encryption key |               |                |                      |



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
