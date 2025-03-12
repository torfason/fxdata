This repository contains historical foreign exchange rate data in parquet format. The data is in all cases retreived from official central bank sources. Information about available date ranges is provided in `<bank>_meta.json`.

## Central bank data sources

Central banks that make their data available in a format suitable for automatic updating and are used as sources for this data set include:

- `ecb`: European Central Bank, retrieved from:
  - https://www.ecb.europa.eu/stats/eurofxref/eurofxref-hist.zip

## Note on quotation methods

Many central banks, such as the European Central Bank (ECB), use an indirect quotation approach, listing exchange rates as foreign currency per 1 EUR (e.g., 1 EUR = 1.20 USD). Other banks, such as the Central Bank of Iceland (CBI), use a direct quotation, expressing rates as ISK per 1 unit of foreign currency (e.g., 1 USD = 130 ISK). When handling exchange rate data, it's important to standardize or document these differing conventions to ensure accuracy. 

The metadata (`<bank>_meta.json`) for each bank includes  the `quotation_method` that each bank uses, (either `indirect` or `direct`).
