# HowToBeAHero-WikiToPdf

This tool uses [Request](https://github.com/request/request) on [Parasoid](https://www.mediawiki.org/wiki/Parsoid) to fetch specific pages of the [How to be a Hero](https://howtobeahero.de/index.php?title=Hauptseite) Wiki, put them in a nice HTML-template and generate a PDF via [html-pdf](https://www.npmjs.com/package/html-pdf) for a printable version.

## Installing the project ##

Run in project root
```
npm install
```

___Copy over the `config.yaml` from project root to `.\node_modules\parsoid`___

Running the Node.js Express server which will request HTML from the Parsoid server and handle the HTML-Template creation:
```
node index.js
```

Requesting HTML of Wiki Page Titled "Kategorie:Begabungsgruppen" with Express via Browser (both servers (Parsoid/Express) need to be running for that):
```
http://localhost:3000/?title=Kategorie:Begabungsgruppen
```


