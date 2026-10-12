# trading-dashboard-data

Data files behind the JR Market Sentiment module on jrgthecpa.com.

Two files, written automatically every NYSE trading day after the close by a GitHub Action that runs in a private repository:

- `sentiment/latest.json`: the current reading. A 0 to 100 risk-appetite score, its zone, five weighted factors with their drivers, confidence and input coverage, and the as-of date.
- `sentiment/history.json`: one row per trading day, oldest first.

Everything here is derived: a rules-based composite computed from end-of-day prices. No raw market data, no trades, no account information.

Context, not a signal. It does not drive any trading rule and never places a trade. Past readings are not predictive on their own. A personal project, shared for transparency; not investment advice and not a service of the firm.
