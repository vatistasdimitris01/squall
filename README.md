# squall

a sketchy little weather tui

```
                         ~ squall ~
                         ◇ weather ◇

                   › search for a city...

               type · ↑↓ navigate · enter select
```

powered by [Open-Meteo](https://open-meteo.com/) — no API key, no signup.

## install

```bash
git clone https://github.com/vatistasdimitris01/squall.git
cd squall
npm install
npm run build
```

## run

```bash
npm start
```

or after building:

```bash
node dist/cli.mjs
```

## usage

| key | action |
|---|---|
| type | search for a city |
| `↑` `↓` | navigate results |
| `enter` | select city |
| `esc` | clear search |
| `b` / `q` | back / quit from weather |

## data

- search: Open-Meteo Geocoding API
- current: temperature, feels-like, humidity, wind, UV, pressure
- hourly: next 6 hours with precipitation
- daily: 7-day forecast with highs, lows, and precipitation
- sunrise & sunset times

## build

```bash
npm run build      # bundle with esbuild
npm run dev        # build + run
```

## license

MIT
