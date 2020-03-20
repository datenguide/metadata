# Datenguide metadata

This repo holds manually curated metadata about German public statistics for use by the [Datenguide](https://datengui.de) project. It includes metadata about the following entities:

## Regions

German regions, NUTS level 1-3 (Bundesländer, Regierungsbezirke, Statistische Regionen, Landkreise, Kreisstädte, etc.) and LAU (Gemeinden). Regions are managed in `/regions.json` using the following structure:

```js
{
    "08425": {
        "id": "08425", // AGS for the region
        "name": "Alb-Donau-Kreis", // Nicely formated name of the region
        "type": "Landkreis", // Type of region (e.g. Kreisfreie Stadt, Regierungsbezirk)
        "level": 3, // NUTS level (1-3), LAU (4)
        "duration": { 
            "from": "2012-01-01", // ISO dates for earliest available statistical measure  
            "until": "2019-12-31"  // ISO dates for latest available statistical measure  
        }
    },
}
```

## Statistics and measures

Metadata about regions are managed in Markdown files using the following structure:

[to be defined]

## License

The metadata in this repository was derived from data originally published by the German Federal Statistics Offices, [Statistische Ämter des Bundes und der Länder](https://www.statistikportal.de/de/statistische-aemter), under the [Data licence Germany – attribution – version 2.0](https://www.govdata.de/dl-de/by-2-0).
