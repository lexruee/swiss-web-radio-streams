# swiss-web-radio-streams

The json-ld file `streams.jsonld` contains a collection of swiss web streams
from NRJ Swiss.


__Example contents__:

```jsonld
{
    "@context": { 
        "schema": "http://schema.org",
        "streams": "schema:track",
        "stations": "schema:itemListElement",
        "title": "schema:title",
        "description": "schema:description",
        "contentUrl": "schema:contentUrl",
        "encodingFormat": "schema:encodingFormat",
        "addressCountry": "schema:adressCountry"
    },

    "@type": "schema:MusicPlaylist",
    "streams": {
        "@type": "schema:ItemList",
        "stations": [
            {
                "@type": "schema:AudioObject",
                "title": "Energy Bern",
                "description": "Energy Bern",
                "contentUrl": "http://energybern.ice.infomaniak.ch:80/energybern-high.mp3",
                "encodingFormat": "mp3",
                "addressCountry": "CH"
            },
            {
                "@type": "schema:AudioObject",
                "title": "Energy Zürich",
                "description": "Energy Zürich",
                "contentUrl": "http://energyzuerich.ice.infomaniak.ch/energyzuerich-high.mp3",
                "encodingFormat": "mp3",
                "addressCountry": "CH"
            },
            {
                "@type": "schema:AudioObject",
                "title": "Energy Basel",
                "description": "Energy Basel",
                "contentUrl": "http://energybasel.ice.infomaniak.ch/energybasel-high.mp3",
                "encodingFormat": "mp3",
                "addressCountry": "CH"
            },
            ...
        ]
    }
}
```
