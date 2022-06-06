---
title: 'Ny version af Costa - version 1.6.0'
layout: post
categories:
  - Costa
---
Så blev det den tid igen. Jeg har i dag udgivet en ny version af Costa, version 1.6.0, efter næsten 6 måneders ventetid siden sidste version. Costa er kort fortalt mit lille hobbyprojekt, hvor jeg siden 2004 har udviklet på en grafisk brugerflade til MS-DOS og kompatible systemer.

Den største nyhed i denne version er understøttelse af EGA-grafik. Indtil nu har Costa kun understøttet VGA grafik, men der er en række ulemper ved dette. Den måde hvorpå VGA håndterer grafik, inddelt i fire hukommelsesområder, giver VGA en forholdsvis dårlig ydeevne. Derudover er der ingen hukommelse tilovers til en grafik buffer, hvilket vil sige at jeg ikke har mulighed for at tegne ting i baggrunden, og derefter vise dem på skærmen. Alt skal tegnes direkte på skærmen.

Ved at implementere EGA understøttelse løses begge disse problemer. Som en ekstra bonus gør det også Costa i stand til at køre på ældre computere end hidtil - i teorien helt ned til en computer med en Intel 80286 CPU, mindst 250 kilobyte RAM og et EGA-grafikkort med mindst 64 kilobyte grafik RAM. Ulempen er, at Costa i EGA-tilstand har en lavere skærmopløsning. I VGA-tilstand benyttes skærmopløsningen 640x480, hvorimod der i EGA-tilstand benyttes 640x350. Altså 130 færre pixels lodret.

For at tilgodese alle brugere, kan der skiftes frit imellem EGA- og VGA-tilstand, uden at det er nødvendigt at lukke Costa.

Visuelt er der også en del ændringer. Stort set alle ikoner er blevet lavet om, da mange af dem var "lånt" fra Windows og andet software, og jeg ikke ønsker at have indhold i Costa som ikke enten er lavet af mig selv, eller sendt til mig af andre som selv har lavet det. Alle er i øvrigt velkomne til at sende mig ikoner og temaer til Costa, som kan blive en del af kommende versioner.

Standard temaet er også blevet ændret. Jeg eksperimenterede lidt med farverne til jeg fandt en sammensætning jeg synes godt om. Efterfølgende har jeg så konstateret at temaet minder om [OS/2](https://en.wikipedia.org/wiki/OS/2) 2.0, hvilket ikke var noget jeg sigtede efter, men lad os kalde det en hyldest til OS/2.

![The Costa GUI version 1.6.0]({{site.url}}/assets/img/160.png)

Mere information, og links til download, kan findes på <https://costa.jacobpalm.dk>.

For dem der har interesse i udviklingen og den bagvedliggende kode, indeholder [Costas GitHub repository](https://github.com/jacobpalm/costa) alt dette.