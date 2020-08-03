# openlp-custom-stages
 
Custom screens for OpenLP 2.x implemented as additional foldback (stage) views.  Each view is fully contained as three files (stage.html, stage.js, and stage.css) within a single directory.  Currently, two views are available:

* `foldback` - useful for projecting lyrics and other content onto a rear projector or stage-side monitor
* `obs` - outputs white text on a blue-gradient overlay over a transparent background, for use in Open Broadcasting Software (OBS)

## Installation

### Windows

Copy the contents of this repository into `%APPDATA%\Roaming\openlp\data\stages`.

## Usage

Output is via web browser at `http://localhost:4316/stage/obs` or `http://localhost:4316/stage/foldback`.

## Limitations

The OpenLP 2.x API does not expose copyright information for songs in its database.  One workaround is to create an "Other" verse for the song in OpenLP named "O1" (important!) with the song title on the first line and any additional information on the next 2-3 lines.  The `obs` view looks for "O1" slides and will style it differently.
