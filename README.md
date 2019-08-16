# design

## Klonen
Dieses Repo benutzt [Git Submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules). Um das Repo mit all seinen Inhalten zu klonen, muss folgendes gemacht werden.

```git
git clone git@github.com:foss-ag/design.git
git submodule init
git submodule update
```

Die Submodule beinhalten spezifische (Druck-)Produkte. 

## Repo-Strukur
Das Repo beinhaltet sowohl unspezifische Source-Dateien, z.B. im `.svg` Format: rundes Logo, eckiges Logo, Logo mit Text, als auch spezifische (Druck-)Produkte, z.B. ein T-Shirt oder Sticker. Aus den Source-Dateien generierte Ausgangsformate (`.png`, `.pdf`, etc.) sind in verschiedenen Ausführungen unter den [GitHub Releases](https://github.com/foss-ag/design/releases) auffindbar.

### Unspezifische Source-Dateien
Diese Dateien gehören allesamt zum Corporate-Identity der FOSS-AG. Sie sind generisch genug, um für neue Zwecke (etwa neue Druckprodukte) verwendet zu werden. Du findest sie im Ordner `src`.

Um neue Formen der Corporate-Identity zu erstellen, lege sie entsprechend der Struktur im `src` Ordner an. TODO: siehe das Issue [#17](https://github.com/foss-ag/design/issues/17)

### Spezifische (Druck-)Produkte
Da spezifische Druckprodukte häufig in leicht abgewandelter Form die Corporate-Identity enthalten bzw. zusätzliche Designmerkmale und -elemente beinhalten, werden diese als Submodul hinzugefügt d.h. als eigenes Repo.

```git
git submodule add <repo-url> <path>
```

`<repo-url>`: URL des Repos, welches eingebunden werden soll.  
`<path>`: Ordnername und -pfad unterhalb des Design-Repos, in den das Submodul eingebunden werden soll.

### Releases
Um die Corporate Identity besser nutzen zu können, sollten von jeder Source-Datei Releases erstellt werden, in Ausgangsformate wie `.png` und `.pdf`.
