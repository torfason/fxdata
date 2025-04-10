<!-- ====================================================== -->
<!-- Generated from .../fxconvert/build/document_fxdata.Rmd -->
<!-- Please edit that file to update documentation          -->
<!-- ====================================================== -->

This repository contains historical foreign exchange rate data in
parquet format. The data is in all cases retreived from official central
bank sources. Information about available date ranges is provided in
`<bank>_meta.json`.

## Central bank data sources

Central banks that make their data available in a format suitable for
automatic updating and are used as sources for this data set include:

- `ecb`: European Central Bank, retrieved from:
  - <https://www.ecb.europa.eu/stats/eurofxref/eurofxref-hist.zip>
- `cbi`: Central Bank of Iceland, retrieved from:
  - <https://sedlabanki.is/gagnatorg/xml-gogn/>
- `fed`: Federal Reserve Bank of St. Louis, retrieved from:
  - <https://fred.stlouisfed.org/searchresults/?st=spot%20exchange%20rates>

## Availability

This table shows the availability of different currencies from the
various central bank sources. The table values refer to the first and
last availabilities from each source, but currencies may have gaps
within these periods for one or more sources due to temporary currency
restrictions or other reasons.

| Symbol | Name                        |    ECB    |    CBI    |    FED    |
|:-------|:----------------------------|:---------:|:---------:|:---------:|
| EUR    | Euro                        | 1999-2025 | 1999-2025 | 1999-2025 |
| USD    | US Dollar                   | 1999-2025 | 1981-2025 | 1971-2025 |
| CAD    | Canadian Dollar             | 1999-2025 | 1981-2025 | 1971-2025 |
| CHF    | Swiss Franc                 | 1999-2025 | 1981-2025 | 1971-2025 |
| DKK    | Danish Krone                | 1999-2025 | 1981-2025 | 1971-2025 |
| GBP    | Pound Sterling              | 1999-2025 | 1981-2025 | 1971-2025 |
| JPY    | Japanese Yen                | 1999-2025 | 1981-2025 | 1971-2025 |
| NOK    | Norwegian Krone             | 1999-2025 | 1981-2025 | 1971-2025 |
| SEK    | Swedish Krona               | 1999-2025 | 1981-2025 | 1981-2025 |
| AUD    | Australian Dollar           | 1999-2025 | 2006-2025 | 1971-2025 |
| NZD    | New Zealand Dollar          | 1999-2025 | 2006-2025 | 1971-2025 |
| SGD    | Singapore Dollar            | 1999-2025 | 2006-2025 | 1971-2025 |
| ZAR    | South African Rand          | 1999-2025 | 2006-2025 | 1980-2025 |
| HKD    | Hong Kong Dollar            | 1999-2025 | 2006-2025 | 1981-2025 |
| KRW    | South Korean Won            | 1999-2025 | 2006-2025 | 1981-2025 |
| CNY    | Yuan Renminbi               | 2005-2025 | 2006-2025 | 1981-2025 |
| THB    | Thai Baht                   | 2005-2025 | 2008-2025 | 1981-2025 |
| MXN    | Mexican Peso                | 2008-2025 | 2006-2025 | 1993-2025 |
| BRL    | Brazilian Real              | 2008-2025 | 2006-2025 | 1995-2025 |
| INR    | Indian Rupee                | 2009-2025 | 2006-2025 | 1973-2025 |
| ISK    | Icelandic Króna             | 1999-2025 | 1981-2025 |     .     |
| MTL    | Maltese Lira                | 1999-2007 | 2006-2007 |     .     |
| EEK    | Estonian Kroon              | 1999-2010 | 2006-2010 |     .     |
| LVL    | Latvian Lats                | 1999-2013 | 2006-2013 |     .     |
| LTL    | Lithuanian Litas            | 1999-2014 | 2006-2014 |     .     |
| CZK    | Czech Koruna                | 1999-2025 | 2006-2025 |     .     |
| HUF    | Hungarian Forint            | 1999-2025 | 2006-2025 |     .     |
| PLN    | Polish Zloty                | 1999-2025 | 2006-2025 |     .     |
| BGN    | Bulgarian Lev               | 2000-2025 | 2006-2025 |     .     |
| HRK    | Croatian Kuna               | 2005-2022 | 2006-2022 |     .     |
| RUB    | Russian Ruble               | 2005-2022 | 2006-2022 |     .     |
| TRY    | Turkish Lira                | 2005-2025 | 2006-2025 |     .     |
| ILS    | New Israeli Shekel          | 2011-2025 | 2006-2025 |     .     |
| MYR    | Malaysian Ringgit           | 2005-2025 |     .     | 1971-2025 |
| TRL    | Turkish Lira (old)          | 1999-2004 |     .     |     .     |
| ROL    | Romanian Leu (old)          | 1999-2005 |     .     |     .     |
| SIT    | Slovenian Tolar             | 1999-2006 |     .     |     .     |
| CYP    | Cypriot Pound               | 1999-2007 |     .     |     .     |
| SKK    | Slovak Koruna               | 1999-2008 |     .     |     .     |
| IDR    | Rupiah                      | 2005-2025 |     .     |     .     |
| PHP    | Philippine Peso             | 2005-2025 |     .     |     .     |
| RON    | Romanian Leu                | 2005-2025 |     .     |     .     |
| TWD    | New Taiwan Dollar           |     .     | 2006-2025 | 1983-2025 |
| ATS    | Austrian Schilling          |     .     | 1981-2002 |     .     |
| DEM    | Deutsche Mark               |     .     | 1981-2002 |     .     |
| ESP    | Spanish Peseta              |     .     | 1981-2002 |     .     |
| FIM    | Finnish Markka              |     .     | 1981-2002 |     .     |
| FRF    | French Franc                |     .     | 1981-2002 |     .     |
| IEP    | Irish Pound                 |     .     | 1981-2002 |     .     |
| ITL    | Italian Lira                |     .     | 1981-2002 |     .     |
| NLG    | Dutch Guilder               |     .     | 1981-2002 |     .     |
| PTE    | Portuguese Escudo           |     .     | 1981-2002 |     .     |
| XDR    | Special Drawing Rights      |     .     | 1981-2025 |     .     |
| BEF    | Belgian Franc               |     .     | 1990-2002 |     .     |
| GRD    | Greek Drachma               |     .     | 1991-2002 |     .     |
| NGN    | Nigerian Naira              |     .     | 2006-2025 |     .     |
| SRD    | Surinamese Dollar           |     .     | 2006-2025 |     .     |
| JMD    | Jamaican Dollar             |     .     | 2010-2025 |     .     |
| VEF    | Venezuelan Bolívar (old)    |     .     | 2013-2018 |     .     |
| SAR    | Saudi Riyal                 |     .     | 2013-2025 |     .     |
| KWD    | Kuwaiti Dinar               |     .     | 2025-2025 |     .     |
| LKR    | Sri Lankan Rupee            |     .     |     .     | 1973-2025 |
| VES    | Venezuelan Bolívar Soberano |     .     |     .     | 1995-2025 |

## Note on quotation methods

Many central banks, such as the European Central Bank (ECB), use an
indirect quotation approach, listing exchange rates as foreign currency
per 1 EUR (e.g., 1 EUR = 1.20 USD). Other banks, such as the Central
Bank of Iceland (CBI), use a direct quotation, expressing rates as ISK
per 1 unit of foreign currency (e.g., 1 USD = 130 ISK). When handling
exchange rate data, it’s important to standardize or document these
differing conventions to ensure accuracy.

The metadata (`<bank>_meta.json`) for each bank includes the
`quotation_method` that each bank uses, (either `indirect` or `direct`).
The Federal Reserve Bank of St. Louis (FED) publishes rates in a mix of
direct an indirect quotations, they quotes must be converted to a common
method before inclusion. The indirect approach is used for the main data
set (`fed`), but a data set with the direct approach is available as
well (`xfed`).
