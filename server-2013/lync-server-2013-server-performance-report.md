﻿---
title: 'Lync Server 2013: Rapporto prestazioni dei server'
TOCTitle: Rapporto prestazioni dei server
ms:assetid: 942bb39a-1790-498e-9d99-8f6ce2d155c3
ms:mtpsurl: https://technet.microsoft.com/it-it/library/Gg615018(v=OCS.15)
ms:contentKeyID: 49301357
ms.date: 08/24/2015
mtps_version: v=OCS.15
ms.translationtype: HT
---

# Rapporto prestazioni dei server in Lync Server 2013

 

_**Ultima modifica dell'argomento:** 2015-03-09_

Il Rapporto prestazioni dei server offre un elenco di server Microsoft Lync Server 2013 in cui è stata riscontrata una percentuale più elevata di chiamate di livello insufficiente. Nel rapporto i server sono suddivisi in base al tipo in modo da riportare statistiche distinte per quelli seguenti:

  - Mediation Server

  - A/V Conferencing Server

  - A/V Edge Server

  - Gateway (Mediation Server)

  - Gateway (bypass a Mediation Server)

  - Video (incluse le metriche video per A/V Conferencing Server e A/V Edge Server)

  - Condivisione applicazioni (incluse le metriche di condivisione applicazioni per A/V Conferencing Server e A/V Edge Server)

È importante notare che le classificazioni illustrate in questo rapporto sono relative. Supponiamo ad esempio che il server con le prestazioni peggiori presenti una chiamata di livello insufficiente su 1.000 chiamate effettuate. Si tratta della più che accettabile percentuale dello 0,1%. Se questo è il server con le prestazioni peggiori (ovvero se tutti gli altri server presentano percentuali di chiamate di livello insufficiente inferiori a 0,1%), tale server verrà comunque incluso nel Rapporto prestazioni dei server.

## Accesso al Rapporto prestazioni dei server

Il Rapporto prestazioni dei server è accessibile dalla home page Rapporti di monitoraggio. È possibile eseguire il drill-down al [Rapporto Elenco chiamate in Lync Server 2013](lync-server-2013-call-list-report.md) facendo clic sulle metriche seguenti:

  - Volume chiamata

  - Percentuale chiamate di livello insufficiente

È inoltre possibile eseguire il drill-down al Rapporto tendenze qualità multimediale server facendo clic sulla metrica seguente:

  - Tendenza

## Uso ottimale del Rapporto prestazioni dei server

Il Rapporto prestazioni dei server offre diversi modi per filtrare i dati; ad esempio è possibile filtrare per tipo di rete (chiamate effettuate da una connessione cablata rispetto a quelle effettuate da una connessione wireless) e tipo di accesso (chiamate effettuate dall'interno del firewall rispetto a quelle effettuate dall'esterno del firewall). Quando si esamina il rapporto sulle prestazioni dei server, è consigliabile fare uso di questi filtri. Si supponga ad esempio di disporre di un Mediation Server con una percentuale di chiamate di livello insufficiente del 3,24%. Se si osservano esclusivamente le chiamate wireless, lo stesso server presenta una percentuale di chiamate di livello insufficiente prossimo al 20%. Ciò significa che il server presenta difficoltà con le chiamate wireless, problema parzialmente nascosto dal fatto che il server non presenta problemi con le chiamate cablate.

## Filtri

I filtri consentono di ottenere un set di dati più specifico o di visualizzare in modo diverso i dati restituiti. Ad esempio, il Rapporto prestazioni dei server consente di filtrare i dati restituiti in base al tipo di server o al tipo di rete (cablata o wireless). È inoltre possibile scegliere la modalità di raggruppamento dei dati. In questo caso i dati sono raggruppabili per ora, giorno, settimana o mese.

Nella tabella seguente sono elencati i filtri applicabili al Rapporto prestazioni dei server.

### Filtri del Rapporto prestazioni dei server

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
<p>7/7/2012 1:00 PM</p>
<p>Se non si specifica l'ora di inizio, il rapporto inizia automaticamente alla mezzanotte del giorno specificato. Per visualizzare i dati in base al giorno, immettere solo la data:</p>
<p>7/7/2012</p>
<p>Per visualizzare i dati in base alla settimana o al mese, immettere una data che rientra nella settimana o nel mese in base a cui deve essere effettuata la visualizzazione. Non è necessario immettere il primo giorno della settimana o del mese:</p>
<p>7/3/2012</p>
<p>Le settimane vengono calcolate sempre dal lunedì alla domenica.</p></td>
</tr>
<tr class="even">
<td><p><strong>A</strong></p></td>
<td><p>Data/ora di fine dell'intervallo di tempo. Per visualizzare i dati in base all'ora, immettere sia la data che l'ora di fine come indicato di seguito:</p>
<p>7/7/2012 1:00 PM</p>
<p>Se non si specifica l'ora di fine, il rapporto termina automaticamente alla mezzanotte del giorno specificato. Per visualizzare i dati in base al giorno, immettere solo la data:</p>
<p>7/7/2012</p>
<p>Per visualizzare i dati in base alla settimana o al mese, immettere una data che rientra nella settimana o nel mese in base a cui deve essere effettuata la visualizzazione. Non è necessario immettere il primo giorno della settimana o del mese:</p>
<p>7/3/2012</p>
<p>Le settimane vengono calcolate sempre dal lunedì alla domenica.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Tipo di server</strong></p></td>
<td><p>Indica il tipo di server di cui eseguire il rapporto sulle prestazioni. Selezionare uno dei seguenti:</p>
<ol>
<li><p>[Tutto]</p></li>
<li><p>Mediation Server</p></li>
<li><p>A/V Conferencing Server</p></li>
<li><p>A/V Edge Server</p></li>
</ol></td>
</tr>
<tr class="even">
<td><p><strong>Primi N elementi</strong></p></td>
<td><p>Indica il numero di server, in base alla percentuale di chiamate di livello insufficiente, da visualizzare in ogni categoria. Se ad esempio si seleziona <strong>5</strong> verranno visualizzati i cinque server con le prestazioni peggiori. Selezionare uno dei seguenti:</p>
<ol>
<li><p>[Tutto]</p></li>
<li><p>5</p></li>
<li><p>10</p></li>
</ol></td>
</tr>
<tr class="odd">
<td><p><strong>Tipo di accesso</strong></p></td>
<td><p>Indica se al momento dell'esecuzione della chiamata il client era connesso alla rete interna o alla rete esterna. Selezionare una delle opzioni seguenti:</p>
<ol>
<li><p>[Tutto]</p></li>
<li><p>Interna</p></li>
<li><p>Esterna</p></li>
</ol></td>
</tr>
<tr class="even">
<td><p><strong>Tipo di rete</strong></p></td>
<td><p>Indica il tipo di rete a cui il client era connesso quando è stata effettuata la chiamata. Selezionare una delle opzioni seguenti:</p>
<ol>
<li><p>[Tutto]</p></li>
<li><p>Cablata</p></li>
<li><p>Wireless</p></li>
</ol></td>
</tr>
<tr class="odd">
<td><p><strong>VPN</strong></p></td>
<td><p>Indica se un client esterno utilizzava una connessione di rete privata virtuale (VPN) quando è stata effettuata la chiamata. Selezionare una delle opzioni seguenti:</p>
<ol>
<li><p>[Tutto]</p></li>
<li><p>VPN</p></li>
<li><p>Non VPN</p></li>
</ol></td>
</tr>
</tbody>
</table>


## Metriche

La tabella seguente elenca le informazioni disponibili nel Rapporto prestazioni dei server.

### Metriche del Rapporto prestazioni dei server: riepilogo delle chiamate audio

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th>Nome</th>
<th>Possibilità di ordinamento</th>
<th>Descrizione</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>Server</strong></p></td>
<td><p>No</p></td>
<td><p>Nome/indirizzo IP del server.</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume chiamata</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate effettuate.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Percentuale chiamate di livello insufficiente</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate classificate come di livello insufficiente. In una chiamata di livello insufficiente almeno una delle metriche misurate supera il valore consentito, ad esempio viene rilevato un livello di instabilità eccessivo.</p></td>
</tr>
<tr class="even">
<td><p><strong>Roundtrip (ms)</strong></p></td>
<td><p>Sì</p></td>
<td><p>Tempo medio di roundtrip (in millisecondi) richiesto per il viaggio di andata e ritorno di un pacchetto RTP (Real-Time Transport Protocol) verso e da un altro endpoint. I roundtrip che non superano i 100 millisecondi vengono considerati accettabili.</p>
<p>Valori di tempo di roundtrip elevati possono essere dovuti a routing delle chiamate internazionali, errata configurazione del routing o overload di un server di contenuti multimediali e comportano difficoltà nelle conversazioni audio bidirezionali in tempo reale.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Degradazione (MOS)</strong></p></td>
<td><p>Sì</p></td>
<td><p>Degradazione MOS (Mean Opinion Score) media sperimentata durante una chiamata. I valori di degradazione possono oscillare da un minimo di 0,0 a un massimo di 5,0. Un valore di 0,5 o inferiore rappresenta una degradazione accettabile. In passato questo valore veniva calcolato chiedendo agli utenti di valutare la qualità di una chiamata in una scala da 1 a 5. In Lync Server, il Monitoring Server utilizza un set di algoritmi per prevedere in che modo gli utenti avrebbero valutato la chiamata.</p>
<p>Valori di degradazione elevati possono essere causati da congestione, mancanza di larghezza di banda, interferenze o congestione della rete wireless o da un endpoint o un server di contenuti multimediali sovraccarico. Una degradazione elevata genera audio distorto o perdita di audio.</p></td>
</tr>
<tr class="even">
<td><p><strong>Perdita di pacchetti</strong></p></td>
<td><p>Sì</p></td>
<td><p>Frequenza media di perdita di pacchetti RTP (Real-Time Transport Protocol). La perdita di pacchetti si verifica quando i pacchetti RTP, un protocollo utilizzato per la trasmissione di audio e video su Internet, non raggiungono la destinazione. Valori alti di perdita sono in genere dovuti a congestione, superamento della larghezza di banda disponibile, congestione/interferenze wireless o sovraccarico del server dei contenuti multimediali con conseguente audio distorto o perdita di audio.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Instabilità (ms)</strong></p></td>
<td><p>Sì</p></td>
<td><p>Instabilità media rilevata tra gli arrivi dei pacchetti RTP (Real-Time Transport Protocol). L'instabilità è un indice della qualità di una chiamata. Valori di instabilità elevati sono generalmente dovuti a congestione o overload di un server di contenuti multimediali e comportano distorsione o perdita di audio.</p></td>
</tr>
<tr class="even">
<td><p><strong>Rapporto campioni nascosti utilità di ripristino</strong></p></td>
<td><p>Sì</p></td>
<td><p>Rapporto medio tra i campioni audio nascosti e il numero totale di campioni. Un campione audio nascosto è una tecnica utilizzata per mitigare le transazioni improvvise generalmente causate dall'eliminazione di pacchetti di rete. Valori elevati indicano l'applicazione di livelli significativi di soppressione della perdita applicata dovuti a perdita di pacchetti o instabilità, con conseguente audio distorto o perdita di audio.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Rapporto campioni estesi utilità di ripristino</strong></p></td>
<td><p>Sì</p></td>
<td><p>Rapporto medio tra i campioni audio estesi e il numero totale di campioni. Con audio esteso si intende l'audio che è stato espanso per garantire la qualità delle chiamate quando viene rilevato un pacchetto di rete eliminato. Valori elevati indicano livelli significativi di estensione dei campioni dovuti a instabilità, con conseguente riproduzione di audio robotico o distorto.</p></td>
</tr>
<tr class="even">
<td><p><strong>Rapporto campioni compressi utilità di ripristino</strong></p></td>
<td><p>Sì</p></td>
<td><p>Rapporto medio tra i campioni audio compressi e il numero totale di campioni. L'audio compresso è audio che è stato compresso per mantenere la qualità della chiamata quando è stato rilevato un pacchetto di rete eliminato. Valori alti indicano livelli significativi di compressione dei campioni dovuti a instabilità con conseguente riproduzione di audio accelerato o distorto.</p></td>
</tr>
</tbody>
</table>


### Metriche del Rapporto prestazioni dei server: riepilogo delle videochiamate

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
<td><p><strong>Tipo di chiamata/Tipo di endpoint</strong></p></td>
<td><p>No</p></td>
<td><p>Facendo clic su questo elemento è possibile visualizzare informazioni dettagliate sulle chiamate in base al tipo. I tipi di chiamata includono:</p>
<ul>
<li><p>Chiamate peer-to-peer UC</p></li>
<li><p>Sessioni conferenza UC</p></li>
<li><p>Sessioni conferenza PSTN</p></li>
<li><p>Chiamate PSTN: bypass multimediale</p></li>
<li><p>Chiamate PSTN (senza bypass): coda UC</p></li>
<li><p>Chiamate PSTN (senza bypass): coda gateway</p></li>
<li><p>Altri tipi di chiamata</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Volume chiamata</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate per ciascun tipo.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Percentuale chiamate di livello insufficiente</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate classificate come di livello insufficiente. In una chiamata di livello insufficiente almeno una delle metriche misurate supera il valore consentito, ad esempio viene rilevato un livello di instabilità eccessivo.</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume chiamata (chiamata wireless)</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate eseguite tramite una connessione wireless.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Volume chiamata (chiamata VPN)</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate eseguite tramite una connessione VPN.</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume chiamata (chiamata esterna)</strong></p></td>
<td><p>No</p></td>
<td><p>Numero di chiamate eseguite tramite una connessione esterna, ovvero un collegamento fuori dalla rete interna.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Velocità media in bit (Kbit/s)</strong></p></td>
<td><p>No</p></td>
<td><p>Velocità in bit video media (in kilobit al secondo).</p></td>
</tr>
<tr class="even">
<td><p><strong>Bassa velocità in bit (%)</strong></p></td>
<td><p>No</p></td>
<td><p>Percentuale della chiamata con velocità in bit bassa.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Perdita di pacchetti in uscita</strong></p></td>
<td><p>No</p></td>
<td><p>Perdita di pacchetti RTP (Real-Time Transport Protocol) in uscita. La perdita di pacchetti si verifica quando i pacchetti RTP, un protocollo utilizzato per la trasmissione di audio e video su Internet, non raggiungono la destinazione. Valori alti di perdita sono in genere dovuti a congestione, superamento della larghezza di banda disponibile, congestione/interferenze wireless o sovraccarico del server dei contenuti multimediali con conseguente audio distorto o perdita di audio.</p></td>
</tr>
<tr class="even">
<td><p><strong>% fotogrammi bloccati</strong></p></td>
<td><p>No</p></td>
<td><p>Percentuale di fotogrammi “bloccati”. In un fotogramma bloccato, il video smette di avanzare mentre la parte audio della chiamata prosegue.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Frequenza media dei fotogrammi in uscita</strong></p></td>
<td><p>No</p></td>
<td><p>Frequenza media dei fotogrammi per le trasmissioni in uscita durante la chiamata.</p></td>
</tr>
<tr class="even">
<td><p><strong>Frequenza media dei fotogrammi in ingresso</strong></p></td>
<td><p>No</p></td>
<td><p>Frequenza media dei fotogrammi per le trasmissioni in arrivo durante la chiamata.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Bassa frequenza dei fotogrammi in ingresso (%)</strong></p></td>
<td><p>No</p></td>
<td><p>Percentuale della chiamata con velocità in bit bassa per il video in arrivo.</p></td>
</tr>
<tr class="even">
<td><p><strong>Integrità client (%)</strong></p></td>
<td><p></p></td>
<td><p>Indica l'integrità relativa del dispositivo client durante la chiamata.</p></td>
</tr>
</tbody>
</table>


### Metriche del Rapporto prestazioni dei server: riepilogo delle chiamate di condivisione applicazioni

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
<td><p><strong>Tipo di chiamata/Tipo di endpoint</strong></p></td>
<td><p>No</p></td>
<td><p>Facendo clic su questo elemento è possibile visualizzare informazioni dettagliate sulle chiamate in base al tipo. I tipi di chiamata includono:</p>
<ul>
<li><p>Chiamate peer-to-peer UC</p></li>
<li><p>Sessioni conferenza UC</p></li>
<li><p>Sessioni conferenza PSTN</p></li>
<li><p>Chiamate PSTN: bypass multimediale</p></li>
<li><p>Chiamate PSTN (senza bypass): coda UC</p></li>
<li><p>Chiamate PSTN (senza bypass): coda gateway</p></li>
<li><p>Altri tipi di chiamata</p></li>
</ul></td>
</tr>
<tr class="even">
<td><p><strong>Volume chiamata</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate per ciascun tipo.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Percentuale chiamate di livello insufficiente</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate classificate come di livello insufficiente. In una chiamata di livello insufficiente almeno una delle metriche misurate supera il valore consentito, ad esempio viene rilevato un livello di instabilità eccessivo.</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume chiamata (chiamata wireless)</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate eseguite tramite una connessione wireless.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Volume chiamata (chiamata VPN)</strong></p></td>
<td><p>No</p></td>
<td><p>Numero totale di chiamate eseguite tramite una connessione VPN.</p></td>
</tr>
<tr class="even">
<td><p><strong>Volume chiamata (chiamata esterna)</strong></p></td>
<td><p>No</p></td>
<td><p>Numero di chiamate eseguite tramite una connessione esterna, ovvero un collegamento fuori dalla rete interna.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Instabilità (ms)</strong></p></td>
<td><p>No</p></td>
<td><p>Instabilità media rilevata tra gli arrivi dei pacchetti RTP (Real-Time Transport Protocol). L'instabilità è un indice della qualità di una chiamata. Valori di instabilità elevati sono generalmente dovuti a congestione o overload di un server di contenuti multimediali e comportano distorsione o perdita di audio.</p></td>
</tr>
<tr class="even">
<td><p><strong>Media unidirezionale relativa</strong></p></td>
<td><p>No</p></td>
<td><p>Media unidirezionale relativa tra due endpoint multimediali. Si tratta di una misurazione della latenza a singolo hop.</p></td>
</tr>
<tr class="odd">
<td><p><strong>Latenza media elaborazione sezioni RDP</strong></p></td>
<td><p>No</p></td>
<td><p>Latenza media dell'elaborazione delle sezioni RDP in AS Conferencing Server per la durata della sessione di visualizzazione. Questa metrica non copre la latenza di rete. Una media elevata riflette ritardi maggiori nell'esperienza di visualizzazione. In un server per conferenze sovraccaricato possono verificarsi ritardi medi maggiori.</p></td>
</tr>
<tr class="even">
<td><p><strong>% totale sezioni danneggiate</strong></p></td>
<td><p>No</p></td>
<td><p>Percentuale totale di sezioni RDP danneggiate.</p></td>
</tr>
</tbody>
</table>

