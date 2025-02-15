---
title: Heatmap - Vergleich von Erreichbarkeit und Bevölkerungsdichte
permalink: de/docs/walkability population heatmap/
lang: de
sections:
- technical
weight: 70
---

Zusätzlich zur [Lokalen Erreichbarkeits Heatmap](../heatmap/) ermöglicht GOAT die Visualisierung einer weiteren Heatmap, genannt "Vergleich von Erreichbarkeit und Bevölkerungsdichte". Diese Heatmap ermöglicht ein besseres Verständnis der Erreichbarkeit in einem bestimmten Gebiet oder in einer bestimmten Nachbarschaft unter Berücksichtigung der Bevölkerungsdichten. Die Heatmap kann zur Beantwortung vieler Planungsfragen verwendet werden, wie zum Beispiel:
- Wo herrscht in der untersuchten Nachbarschaft ein Erreichbarkeitssüberschuss?
- Wo herrscht in der untersuchten Nachbarschaft ein Dichteüberschuss?
- Wo ist Potenzial für (Nach-)Verdichtung? 
- Wo ist eine Verbesserung der Erreichbarkeit zu bestimmten Einrichtungen oder ÖV Haltestellen notwendig?

![](/images/docs/technical_documentation/walkability_population_index/walkability_population_map.png)

#### 1. Berechnung
Die Vergleichs-Heatmap von Erreichbarkeit und Bevölkerungsdichte ergibt sich aus der Schnittmenge der beiden Heatmaps "Lokale Erreichbarkeit" und "Bevölkerungsdichte".
![](/images/docs/technical_documentation/walkability_population_index/intersection_2_layers.png)

#### 2. Klassifizierung
Zur Klassifizierung der Erreichbarkeitswerte, die für jedes Hexagon berechnet wurden, wird eine Einteilung basierend auf Perzentilen verwendet. Die folgende Tabelle zeigt examplarisch, wie sich die Erreichbarkeitswerte zusammensetzen.
![](/images/docs/technical_documentation/walkability_population_index/percentile.png)

Die Vergleichs-Heatmap wird wie folgt berechnet:

<b> Erreichbarkeit - Bevölkerungs - Index = Bevölkerungsdichte – Erreichbarkeitswert </b>

und zeigt folgendes Ergebnis:


![](/images/docs/technical_documentation/walkability_population_index/calculated_index.png)



