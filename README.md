# Relay Monitor API Specifications

![CI][ci]

## 🚧 WIP 🚧

The Relay Monitor API consists of several groups of endpoints:

* Relay Faults
* Relay Scores
* Relay Monitor Metrics

### Render API Specification

To render spec in browser, you will simply need an HTTP server to load the
`index.html` file in root of the repo.

For example:
```console
python -m http.server 8080
```

The spec will render at [http://localhost:8080](http://localhost:8080).
