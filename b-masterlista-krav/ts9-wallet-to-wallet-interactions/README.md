# TS9 Wallet to Wallet interactions

## Mål

<span style="color:var(--ds-text,#172b4d);"><span style="color:var(--ds-text,#172b4d);">Målet är att skapa och underhålla master-dokumentation över krav som ska vara spårbara ur</span> </span>TS9 Wallet to Wallet interactions.

## Bakgrund

N/A

## Antagande

- N/A

## Krav

<span style="color:var(--ds-text,#172b4d);">Här är en summering av krav från</span><span style="color:var(--ds-text,#172b4d);"> </span>**S9 Wallet to Wallet interactions V1.1**.

<table style="width:100%;" xmlns:ac="http://www.atlassian.com/schema/confluence/4/ac/">
<colgroup>
<col style="width: 14%" />
<col style="width: 14%" />
<col style="width: 14%" />
<col style="width: 14%" />
<col style="width: 14%" />
<col style="width: 14%" />
<col style="width: 14%" />
</colgroup>
<thead>
<tr class="header">
<th>Krav_ID</th>
<th>Källans index</th>
<th>Sektion</th>
<th>Beskrivning 1</th>
<th>Beskrivning 2</th>
<th>Digg comment</th>
<th>Ej infört krav/orsak</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td>REQ_1166</td>
<td></td>
<td></td>
<td>At a high-level, W2W interactions SHALL be performed following the ISO/IEC 18013-5 device retrieval method. The Holder's Wallet Unit SHALL act as a mdoc (cf. ISO/IEC 18013-5) and the Verifier's Wallet Unit SHALL act as an mdoc Reader (cf. ISO/IEC 18013-5). The <code>Device Engagement</code> structure of ISO/IEC 18013-5 will be extended to also optionally include the Holder's presentation offer. The presentation offer SHALL be a <code>NameSpaces</code> structure cf. ISO/IEC 18013-5:2021 p. 30. If present, a presentation offer will impose restrictions on the Verifier's <code>mdoc request</code>, such that the <code>DataElements</code> in such subsequent mdoc request SHALL be a subset of the <code>DataElements</code> in the received presentation offer.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1167</td>
<td>STS9_01</td>
<td></td>
<td>Wallet Units SHALL offer the user an option to activate W2W and proceed to Device Engagement.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1168</td>
<td>STS9_02</td>
<td></td>
<td>Wallet Units SHALL notify the User that W2W functionality should only be used with natural person they trust, before the W2W mode is activated.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1169</td>
<td>STS9_03</td>
<td></td>
<td>A Wallet Unit SHALL NOT send or accept a Device Engagement structure containing a presentation offer before the User has activated the W2W mode.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1170</td>
<td>STS9_04</td>
<td></td>
<td>When entering W2W mode, a Wallet Unit SHALL allow the User to choose a role of either Holder or Verifier.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1171</td>
<td>STS9_05</td>
<td></td>
<td>Device engagement for Wallet Units to do W2W interactions SHALL follow ISO/IEC 18013-5 with the extensions and restrictions described in this section.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1172</td>
<td>STS9_06</td>
<td></td>
<td>The Holder's Wallet Unit SHALL take the role of a mdoc and the Verifier's Wallet Unit SHALL take the role of a mdoc reader.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1173</td>
<td>STS9_07</td>
<td></td>
<td>A Wallet Unit SHALL support QR codes for engaging as a Holder in a W2W interaction, meaning it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc regarding the use of QR codes for device engagement.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1174</td>
<td>STS9_08</td>
<td></td>
<td>A Wallet Unit SHALL support QR codes for engaging as a Verifier in a W2W interaction, meaning it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc reader regarding the use of QR codes for device engagement.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1175</td>
<td>STS9_10</td>
<td></td>
<td>A Wallet Unit MAY support NFC for engaging as a Holder in a W2W interaction. If it does, it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc regarding the use of NFC for device engagement.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1176</td>
<td>STS9_11</td>
<td></td>
<td>A Wallet Unit MAY support NFC for engaging as a Verifier in a W2W interaction. If it does, it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc reader regarding the use of NFC for device engagement.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1177</td>
<td>STS9_12</td>
<td></td>
<td>The Holder's Wallet Unit SHOULD allow the Holder to select a set of attributes available in their already issued attestations.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1178</td>
<td>STS9_13</td>
<td></td>
<td>The Wallet Unit SHALL authenticate the Holder before presenting the Holder with the available attributes when enabling the Holder to make such a selection.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1179</td>
<td>STS9_14</td>
<td></td>
<td>If the User makes such a selection, the Holder's Wallet Unit SHALL include them in a <code>PresentationOffer</code> under the key <code>-1</code> in the <code>DeviceEngagement</code> structure.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1180</td>
<td>STS9_15</td>
<td></td>
<td>The DeviceEngagement structure used for W2W interactions SHALL follow the structure below:DeviceEngagement = {        0: tstr, ; Version        1: Security,        ? 2: DeviceRetrievalMethods, ; Is absent if NFC is used for device engagement        ? 3: ServerRetrievalMethods,        ? 4: ProtocolInfo,        ? -1: PresentationOffer        * int =&gt; any}</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1181</td>
<td>STS9_16</td>
<td></td>
<td>The optional ServerRetrievalMethods SHALL be absent.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1182</td>
<td>STS9_17</td>
<td></td>
<td>All key-value pairs SHALL comply with applicable requirements in ISO/IEC 18013-5, except PresentationOffer, which SHALL be defined as:PresentationOffer = {0: tstr, ; Version1: [+ DocOffer]; Documents offered}DocOffer = {0: DocType ; Document type offered 1: NameSpacesOffer ; Namespaces offered}NameSpacesOffer : = {+ NameSpace =&gt; [ + DataElementIdentifier] ; Data elements offered for each namespace}</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1183</td>
<td>STS9_18</td>
<td></td>
<td>The key <code>0</code> of the <code>Presentation Offer</code> contains a version number that in the current version of this document SHALL be "1.0".<code>DocOffer</code> contains the document type as a <code>DocType</code> and the offered namespaces in <code>NameSpacesOffer</code>.<code>DocType</code> follows the ISO/IEC 18013-5:2021 definition for mdoc requests (p. 29).<code>NameSpacesOffer</code> is a CBOR map containing NameSpaces of type <code>NameSpace</code>, and for each <code>NameSpace</code> an array of data element identifiers with type <code>DataElementIdentifier</code>.<code>NameSpace</code> and <code>DataElementIdentifier</code> follow the ISO/IEC 18013-5:2021 definition for mdoc requests (p. 29).
<blockquote>
Note: Rather than letting the <code>PresentationOffer</code> mirror the <code>DeviceRequest</code> structure of ISO/IEC 18013-5:2021, it has been changed to minimize the size of the structure, since it must be transferred using QR codes.
</blockquote>
Below is an example of a presentation offer using CBOR Diagnostic Notation (CDN
<pre><code>{
    0: &quot;1.0&quot;,
    1: [
        {
            0: &quot;org.iso.18013.5.1.mDL&quot;,
            1: {
                &quot;org.iso.18013.5.1&quot;: [
                        &quot;family_name&quot;,
                        &quot;document_number&quot;,
                        &quot;driving_privileges&quot;,
                        &quot;issue_date&quot;,
                        &quot;expiry_date&quot;,
                        &quot;portrait&quot;,
                        ]
            }
        }
    ]
}</code></pre></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1184</td>
<td>STS9_19</td>
<td></td>
<td>Data retrieval for Wallet Units to do W2W interactions SHALL follow ISO/IEC 18013-5 with the extensions and restrictions described in this section.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1185</td>
<td>STS9_20</td>
<td></td>
<td>Wallet Units SHALL support device retrieval.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1186</td>
<td>STS9_21</td>
<td></td>
<td>Wallet Units SHALL NOT support server retrieval.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1187</td>
<td>STS9_22</td>
<td></td>
<td>A Wallet Unit SHALL support BLE for data retrieval as a Holder in a W2W interaction, meaning it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc regarding the use of BLE for data retrieval.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1188</td>
<td>STS9_23</td>
<td></td>
<td>A Wallet Unit SHALL support BLE for data retrieval as a Verifier in a W2W interaction, meaning it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc reader regarding the use of BLE for data retrieval.Note that in ISO/IEC 18013-5, a mdoc must support either BLE or NFC, whereas mdoc readers must support both BLE and NFC. However, since NFC is not supported by all smartphones, it is necessary to mandate a data retrieval technology that works across all smartphones.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1189</td>
<td>STS9_24</td>
<td></td>
<td>A Wallet Unit MAY support NFC for data retrieval as a Holder in a W2W interaction. If it does, it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc regarding the use of NFC for data retrieval.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1190</td>
<td>STS9_25</td>
<td></td>
<td>A Wallet Unit MAY support NFC for data retrieval as a Verifier in a W2W interaction. If it does, it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc reader regarding the use of NFC for data retrieval.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1191</td>
<td>STS9_26</td>
<td></td>
<td>A Wallet Unit MAY support Wi-Fi Aware for data retrieval as a Holder in a W2W interaction. If it does, it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc regarding the use of Wi-Fi Aware for data retrieval.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1192</td>
<td>STS9_27</td>
<td></td>
<td>A Wallet Unit MAY support Wi-Fi Aware for data retrieval as a Verifier in a W2W interaction. If it does, it SHALL comply with all ISO/IEC 18013-5 requirements for a mdoc reader regarding the use of Wi-Fi Aware for data retrieval.Note that according to ISO/IEC 18013-5, an mdoc reader is recommended to (i.e., SHOULD) support Wi-Fi Aware for data retrieval.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1193</td>
<td>STS9_28</td>
<td></td>
<td>The Verifier Wallet Unit SHALL enable the Verifier to construct an mdoc request as follows:
<ul>
<li>If a presentation offer is present in the Device Engagement information received, then the Verifier SHALL be able to select a subset (including their respective document types and name spaces) of the <code>DataElementIdentifiers</code> to include in their mdoc request.</li>
<li>If a presentation offer is not present in the Device Engagement information received, then the Verifier SHALL be able to select a set of <code>DataElementIdentifiers</code> to include in their mdoc request without restrictions. The Wallet Provider SHALL decide which <code>DataElementIdentifiers</code> (including their respective document types and name spaces) the Verifier may select from to request in this case.</li>
</ul></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1194</td>
<td>STS9_29</td>
<td></td>
<td>All <code>IntentToRetain</code> flags SHALL be set to <code>false</code> in a mdoc request used in a W2W interaction.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1195</td>
<td>STS9_30</td>
<td></td>
<td>In a W2W interaction, the Verifier Wallet Unit SHALL be authenticated by the Holder Wallet Unit as a genuine, non-revoked EUDI Wallet Unit operated by a recognised Wallet Provider, within the protocol session in which the mdoc request is sent.Note: the technical mechanism by which this authentication is achieved is not yet determined.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1196</td>
<td>STS9_31</td>
<td></td>
<td>To prevent misuse of the W2W functionality, Wallet Providers SHALL implement rate limiting for the Verifier functionality of their Wallet Units.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1197</td>
<td>STS9_32</td>
<td></td>
<td>A Wallet Provider SHALL ensure that a Wallet Unit in Verifier Wallet Unit mode cannot send more than 5 presentation requests per hour, more than 20 per day, and more than 50 per week.
<blockquote>
Note that "hour", "day", and "week" in this requirement refer to sliding time periods, rather than calendar-aligned intervals. If this limit proves to be too restrictive for certain valid use cases, this limit will be revisited in future versions of this specification.
</blockquote></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1198</td>
<td>STS9_33</td>
<td></td>
<td>A Wallet Provider MAY use increasing backoff times between subsequent presentation requests, provided these limits are not exceeded.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1199</td>
<td>STS9_34</td>
<td></td>
<td>If a presentation offer was sent as part of the W2W interaction, then the Holder's Wallet Unit, after receiving an mdoc request, SHALL validate that the <code>DataElementIdentifiers</code> in the mdoc request are a subset of the <code>DataElementIdentifiers</code> (for their respective document types and name spaces) sent in the presentation offer and that all <code>IntentToRetain</code> flags are set <code>false</code>. If not, then the Holder's Wallet Unit SHALL abort the interaction by sending a <code>DeviceResponse</code> with the field <code>status</code> set to <code>10</code> and not including any values for the optional field <code>documents</code>. In addition, the Holder Wallet Unit SHALL inform its User that the interaction was aborted because the Verifier requested attributes that were not offered by the Holder.
<blockquote>
Implementation note: To prevent the Verifier from inducing information based upon the timing of the response, the time it takes for the wallet to send back this error must depend only on the data available in the <code>PresentationOffer</code> and the <code>DeviceRequest</code> (i.e., data that is already available to the Verifier's device).
</blockquote>
<blockquote>
Note: An alternative approach would have been to let the Holder Wallet Unit only return errors for the specific <code>DataElements</code> that were not part of the presentation offer (rather than not returning any attributes at all). However, to prevent disclosing too much information and since this will <strong>only</strong> happen in cases where the Verifier Wallet Unit is not conforming to this document, this specification has opted to let the Holder's Wallet Unit return no attributes at all.
</blockquote></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1200</td>
<td>STS9_35</td>
<td></td>
<td>When a Wallet Unit receives a mdoc response it SHALL comply with the requirements in ISO/IEC 18013-5 clause 8.3.2.1.2.1 regarding retaining data elements for which the IntentToRetain flag was set to <code>false</code>.
<blockquote>
Note that even though that the data itself shall not be persisted, metadata about the event must still be logged as described in HLR <em>DASH_03b</em> from <a href="https://github.com/eu-digital-identity-wallet/eudi-doc-architecture-and-reference-framework/blob/main/docs/annexes/annex-2/annex-2-high-level-requirements.md#hlrs--11">Annex 2 - ARF</a>.
</blockquote></td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="even">
<td>REQ_1201</td>
<td>STS9_36</td>
<td></td>
<td>Wallet Units SHOULD take measures to prevent users from taking screenshots of received presentations.</td>
<td></td>
<td></td>
<td></td>
</tr>
<tr class="odd">
<td>REQ_1202</td>
<td>STS9_37</td>
<td></td>
<td>A Verifier Wallet Unit SHALL NOT communicate any attribute values received from the Holder Wallet Unit to any other party inside or outside the EUDI Wallet ecosystem.</td>
<td></td>
<td></td>
<td></td>
</tr>
</tbody>
</table>



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
