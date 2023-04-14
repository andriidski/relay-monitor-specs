# Relay Monitor API Specifications

![ci][ci]

Relay Monitor API is an interface for a MEV-Boost PBS [relay][relay-specs] monitoring service based on a [design][relay-monitor-design-doc] for a behavior and performance monitoring service. This interface enables interested parties such as validators running MEV-boost software to get insight into the operation of the relays that they connect to.

The Relay Monitor API consists of several groups of endpoints:

* Transcripts
* Relay Faults
* Relay Scores
* Relay Monitor Metrics

## Contributing

The API specification is checked for lint errors before merging pull requests.

To run the linter locally, install it with:
```console
npm install -g @redocly/cli
```
and then run it:
```console
redocly lint rm-oapi.yaml
```

### Render API Specification

To render spec in browser, you will simply need an HTTP server to load the
`index.html` file in root of the repo.

For example:
```console
python -m http.server 8080
```

The spec will render at [http://localhost:8080](http://localhost:8080).

[ci]: https://github.com/andriidski/relay-monitor-specs/workflows/CI/badge.svg
[relay-specs]: https://github.com/flashbots/relay-specs
[relay-monitor-design-doc]: https://hackmd.io/A2uex3QFSfiaJJ9BKxw-XA