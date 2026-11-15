# btc-cent-forecast-01

[![make.fun · btc-cent-forecast-01](https://make.fun/badge/btc-cent-forecast-01.svg)](https://make.fun/bounty/btc-cent-forecast-01?utm_source=github&utm_medium=readme&utm_campaign=btc-cent-forecast-01)

Forecasts Bitcoin's USDC price 240 minutes (4 hours) ahead from 72 hours of
minute closes, for make.fun's forecasting bounty.

Method: a fixed blend of 35% persistence (the checkpoint close) and 65% the
mean of exponential moving averages with spans 60, 180, 360, 720 and 1440
minutes. The spans and weight were chosen once on the kit's practice cases;
the program fits nothing at run time and is fully deterministic.

Entry point: main.py (Python 3.13, standard library only). Reads every
/input/<id>.in and writes /output/<id>.out.

## License

MIT
