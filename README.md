# lynx-ccc

[Lynx](https://github.com/lynx-chess/Lynx) configuration files for [Computer Chess Championship (CCC)](https://www.chess.com/computer-chess-championship)
<sub>even if Lynx hasn't participated in CCC yet 😄</sub>

## Handy docker commands

Building and running Lynx:

```bash
docker run --rm -it $(docker build -q -f lynx.Dockerfile .)
```

Building and running Lynx, extracting its logs to `lynx-logs` dir:

```bash
docker run --rm -it -v ${PWD}/lynx-logs:/lynx/artifacts/Lynx/logs $(docker build -q -f lynx.Dockerfile .)
```

Inspecting container:

```bash
docker run --rm -it --entrypoint bash $(docker build -q -f lynx.Dockerfile .)
```
