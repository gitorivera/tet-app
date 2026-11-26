# TET App — Temporal Experience Tracing (compiled build)

🇬🇧 English · [🇪🇸 Español](README.es.md)

**Live apps: <https://gitorivera.github.io/tet-app/>**

- **TET-Kid** (with video): <https://gitorivera.github.io/tet-app/kid/>
- **TET** (whole session, no video): <https://gitorivera.github.io/tet-app/tet/>

This repository only hosts the **compiled builds** of the TET tracing apps, served through GitHub Pages. It contains no source code and is overwritten on every release. The source lives in a separate private research repository.

## What is it?

Two Progressive Web Apps used in a doctoral study (Universidad Tecnológica de Pereira, Colombia) comparing children's engagement in a cognitive-rehabilitation game played in mixed reality (Meta Quest) versus on a tablet. After playing, the child traces how they felt over time, one dimension at a time (Temporal Experience Tracing, adapted from [Jachs et al., 2022](https://doi.org/10.1101/2022.03.04.482237)). **TET-Kid** plays back the recording of their game and the child traces while watching it; **TET** shows the whole session on a single time axis and the curve is drawn in one go. The resulting traces are aligned with EEG recorded through Lab Streaming Layer.

## Using it

1. Open the app's link above in Chrome on an Android tablet (or any modern browser).
2. Install it: browser menu → **Install app** / **Add to Home screen**. Each app installs separately, with its own icon. After the first load it works **without an internet connection**.
3. As the researcher, set up the session and hand the tablet to the child. In **TET-Kid** you fill in the participant code and the dimensions and load the game video and the events CSV. In **TET** there is nothing to type: you load the **configuration file** (a JSON holding the participant, the session length, the axis markers, the dimensions and the LSL times) prepared beforehand on the recording computer.
4. At the end, download the CSV/JSON files or share them from the tablet.

## Privacy

Everything runs in the browser. Videos, traces and session data stay **on the device** (IndexedDB / local storage) and are never uploaded to any server.

## Updating

Installed copies update themselves the next time the app is opened with a connection. If a stale version appears, close and reopen the app.

## License

[MIT](LICENSE) © 2026 Jorge Rivera.
