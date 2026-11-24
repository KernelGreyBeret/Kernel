The file `neon-grid/upload/README.md` marks this folder as the one-shot upload inbox for your MIDI ZIP archives.

On your phone: open this folder in GitHub, choose Add file → Upload files, and upload a MIDI .zip file (for example midi-archive.zip).

The Neon Grid MIDI ingest GitHub Action, when enabled, unpacks valid MIDI scores under `neon-grid/tracks/`, updates `neon-grid/library.json`, and removes the uploaded ZIP from the repository.

Do not upload player HTML to this repository folder. The music library remains the only published asset here.
