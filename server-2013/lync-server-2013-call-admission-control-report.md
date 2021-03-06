﻿---
title: 'Lync Server 2013: Rapporto controllo di ammissione di chiamata'
TOCTitle: Rapporto controllo di ammissione di chiamata
ms:assetid: ea4b0c9f-7f93-4b8a-b901-01e1636c44fb
ms:mtpsurl: https://technet.microsoft.com/it-it/library/Gg615043(v=OCS.15)
ms:contentKeyID: 49302368
ms.date: 08/24/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Rapporto controllo di ammissione di chiamata in Lync Server 2013

 

_**Ultima modifica dell'argomento:** 2015-03-09_

Il Rapporto controllo di ammissione di chiamata fornisce informazioni sulle sessioni peer-to-peer e di conferenza sottoposte alle limitazioni imposte dal servizio Controllo di ammissione di chiamata. Il servizio Controllo di ammissione di chiamata, introdotto in Microsoft Lync Server 2010, permette agli amministratori di consentire o negare le sessioni di comunicazione in base a vincoli di larghezza di banda. Gli amministratori possono ad esempio creare criteri che limitano la larghezza di banda disponibile per le chiamate vocali e video. Se il limite di larghezza di banda viene raggiunto, non è possibile avviare ulteriori chiamate vocali o video se prima non termina una delle chiamate in corso liberando le risorse di rete necessarie.

## Accesso al Rapporto controllo di ammissione di chiamata

È possibile accedere al Rapporto controllo di ammissione di chiamata dalla home page di Relazioni monitoraggio. Dal Rapporto controllo di ammissione di chiamata è possibile eseguire il drill-down nei report seguenti:

  - Rapporto Dettagli conferenza - Per accedere a questo rapporto, fare clic sulla metrica Dettagli in una sessione di conferenza.

  - Rapporto Dettagli sessione peer-to-peer - Per accedere a questo rapporto, fare clic sulla metrica Dettagli in una sessione peer-to-peer.

## Utilizzare al meglio il Rapporto controllo di ammissione di chiamata

Per visualizzare un elenco delle chiamate non riuscite per larghezza di banda insufficiente, selezionare Chiamate rifiutate a causa del controllo di ammissione di chiamata dall'elenco a discesa Categoria chiamata. La maggior parte delle chiamate restituite avrà probabilmente l'ID diagnostica 5:

Larghezza di banda insufficiente per stabilire la sessione. Tentare il reindirizzamento PSTN.

Questo indica che le limitazioni imposte dal servizio Controllo di ammissione di chiamata hanno impedito l'esecuzione della chiamata nella rete VoIP.

## Filtri

I filtri consentono di ottenere un set di dati più specifico o di visualizzare in modo diverso i dati restituiti. Ad esempio, il Rapporto controllo di ammissione di chiamata consente di filtrare le chiamate in base all'utente che le ha avviate o all'utente chiamato. È inoltre possibile scegliere la modalità di raggruppamento dei dati. In questo caso le chiamate sono raggruppabili per ora, giorno, settimana o mese.

Nella tabella seguente sono elencati i filtri applicabili al Rapporto controllo di ammissione di chiamata.

### Filtri del Rapporto controllo di ammissione di chiamata

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Da</strong></p></td>
<td><p>Data/ora di inizio dell'intervallo di tempo. Per visualizzare i dati in base all'ora, immettere sia la data che l'ora di inizio come indicato di seguito:</p>
<p>17/07/2012 13.00</p>
<p>Se non si specifica l'ora di inizio, il rapporto inizia automaticamente alla mezzanotte del giorno specificato. Per visualizzare i dati in base al giorno, immettere solo la data:</p>
<p>17/07/2012</p>
<p>Per visualizzare i dati in base alla settimana o al mese, immettere una data che rientra nella settimana o nel mese in base a cui deve essere effettuata la visualizzazione. Non è necessario immettere il primo giorno della settimana o del mese:</p>
<p>13/07/2012</p>
<p>Le settimane vengono calcolate sempre dal lunedì alla domenica.</p></td>
</tr>
<tr class="even">
<td><p><strong>A</strong></p></td>
<td><p>Data/ora di fine dell'intervallo di tempo. Per visualizzare i dati in base all'ora, immettere sia la data che l'ora di fine come indicato di seguito:</p>
<p>17/07/2012 13.00</p>
<p>Se non si specifica l'ora di fine, il rapporto termina automaticamente alla mezzanotte del giorno specificato. Per visualizzare i dati in base al giorno, immettere solo la data:</p>
<p>17/07/2012</p>
<p>Per visualizzare i dati in base alla settimana o al mese, immettere una data che rientra nella settimana o nel mese in base a cui deve essere effettuata la visualizzazione. Non è necessario immettere il primo giorno della settimana o del mese:</p>
<p>13/07/2012</p>
<p>Le settimane vengono calcolate sempre dal lunedì alla domenica.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Pool</strong></p></td>
<td><p>Nome di dominio completo (FQDN) del pool di registrazione o del server perimetrale. È possibile selezionare un singolo pool o fare clic su <strong>[Tutti]</strong> per visualizzare dati per tutti i pool. Questo elenco a discesa viene popolato automaticamente in base ai record del database.</p></td>
</tr>
<tr class="even">
<td><p><strong>Tipo di attività</strong></p></td>
<td><p>Selezionare una delle attività seguenti:</p>
<ul>
<li><p>[Tutto]</p></li>
<li><p>Peer-to-peer</p></li>
<li><p>Conferenza</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p><strong>Categoria chiamata</strong></p></td>
<td><p>Indica il motivo per cui è stato utilizzato il controllo di ammissione chiamata. Selezionare una delle opzioni seguenti:</p>
<ul>
<li><p>[Tutto]</p></li>
<li><p>Chiamate rifiutate a causa del controllo di ammissione di chiamata</p></li>
<li><p>Chiamate reinstradate tramite PSTN a causa del controllo di ammissione di chiamata</p></li>
</ul></td>
</tr>
</tbody>
</table>


## Metriche per le sessioni peer-to-peer

Nella tabella seguente sono elencate le informazioni riportate nel Rapporto controllo di ammissione di chiamata per le sessioni peer-to-peer, ovvero che coinvolgono solo due partecipanti.

### Metriche per le sessioni peer-to-peer

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Elemento utilizzabile per eseguire l'ordinamento?</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Dettagli</strong></p></td>
<td><p>No</p></td>
<td><p>Se si fa clic su questa opzione, nel rapporto viene visualizzato un rapporto dettagliato sulla sessione peer-to-peer specificata.</p></td>
</tr>
<tr class="even">
<td><p><strong>Da utente</strong></p></td>
<td><p>Sì</p></td>
<td><p>Indirizzo SIP dell'utente che ha avviato la sessione.</p></td>
</tr>
<tr class="odd">
<td><p><strong>A utente</strong></p></td>
<td><p>Sì</p></td>
<td><p>Indirizzo SIP dell'utente che è stato invitato a partecipare alla sessione.</p></td>
</tr>
<tr class="even">
<td><p><strong>Modalità</strong></p></td>
<td><p>Sì</p></td>
<td><p>Modalità di comunicazione, ad esempio audio e video, utilizzate durante la sessione.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Ora invito</strong></p></td>
<td><p>Sì</p></td>
<td><p>Date e ora in cui è stato inviato l'invito iniziale alla sessione alla persona indicata in Da utente.</p></td>
</tr>
<tr class="even">
<td><p><strong>Ora risposta</strong></p></td>
<td><p>Sì</p></td>
<td><p>Data e ora in cui è stata ricevuta l'informazione che l'invito è stato accettato.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Ora fine</strong></p></td>
<td><p>Sì</p></td>
<td><p>Data e ora di fine della sessione.</p></td>
</tr>
<tr class="even">
<td><p><strong>ID diagnostica</strong></p></td>
<td><p>Sì</p></td>
<td><p>Identificatore univoco nel formato di un'intestazione ms-diagnostics associato a un messaggio SIP in cui spesso vengono fornite informazioni utili per la risoluzione dei problemi. Le intestazioni di diagnostica sono facoltative (è possibile che in alcune sessioni SIP non siano incluse queste intestazioni) e gli ID diagnostica sono spesso indicati solo per sessioni in cui si sono verificati problemi di un determinato tipo.</p></td>
</tr>
</tbody>
</table>


## Metriche per le sessioni di conferenza

Nella tabella seguente sono elencate le informazioni riportate nel Rapporto di controllo di ammissione di chiamata per le sessioni di conferenza, ovvero che coinvolgono almeno tre partecipanti.

### Metriche per le sessioni di conferenza

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Elemento utilizzabile per eseguire l'ordinamento?</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>URI conferenza</strong></p></td>
<td><p>Sì</p></td>
<td><p>Identificatore univoco della conferenza. Se si fa clic su questa opzione, nel rapporto vengono visualizzati i singoli partecipanti alla conferenza.</p></td>
</tr>
<tr class="even">
<td><p><strong>Organizzatore</strong></p></td>
<td><p>Sì</p></td>
<td><p>Indirizzo SIP dell'utente che ha organizzato la conferenza.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Pool</strong></p></td>
<td><p>Sì</p></td>
<td><p>Server perimetrale utilizzato nella conferenza.</p></td>
</tr>
<tr class="even">
<td><p><strong>Ora inizio</strong></p></td>
<td><p>Sì</p></td>
<td><p>Data e ora di inizio della conferenza.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Ora fine</strong></p></td>
<td><p>Sì</p></td>
<td><p>Data e ora di fine della conferenza.</p></td>
</tr>
</tbody>
</table>


## Metriche per i singoli partecipanti alla conferenza

Nella tabella seguente sono elencate le informazioni riportate nel Rapporto di controllo di ammissione di chiamata per i singoli partecipanti alla conferenza.

### Metriche per i singoli partecipanti alla conferenza

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Elemento utilizzabile per eseguire l'ordinamento?</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Ruolo</strong></p></td>
<td><p>No</p></td>
<td><p>Ruolo, ad esempio Relatore, ricoperto dal partecipante alla conferenza.</p></td>
</tr>
<tr class="even">
<td><p><strong>Partecipante</strong></p></td>
<td><p>No</p></td>
<td><p>Indirizzo SIP del partecipante alla conferenza.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Connettività</strong></p></td>
<td><p>No</p></td>
<td><p>Connettività di rete, solitamente Dall'interno o Dall'esterno, per il partecipante.</p></td>
</tr>
<tr class="even">
<td><p><strong>Modalità</strong></p></td>
<td><p>No</p></td>
<td><p>Tipo di conferenza, ad esempio audio/video.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Ora partecipazione</strong></p></td>
<td><p>No</p></td>
<td><p>Data e ora in cui il partecipante si è unito alla conferenza.</p></td>
</tr>
<tr class="even">
<td><p><strong>Ora uscita</strong></p></td>
<td><p>No</p></td>
<td><p>Data e ora in cui il partecipante è uscito dalla conferenza.</p></td>
</tr>
<tr class="odd">
<td><p><strong>ID diagnostica</strong></p></td>
<td><p>No</p></td>
<td><p>Identificatore univoco nel formato di un'intestazione ms-diagnostics associato a un messaggio SIP in cui spesso vengono fornite informazioni utili per la risoluzione dei problemi. Le intestazioni di diagnostica sono facoltative (è possibile che in alcune sessioni SIP non siano incluse queste intestazioni) e gli ID diagnostica sono spesso indicati solo per sessioni in cui si sono verificati problemi di un determinato tipo.</p></td>
</tr>
</tbody>
</table>

