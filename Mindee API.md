
# Mindee API 

the Mindee node returns a subset of the fields returned from the Mindee API.  

## Expense Receipt  

The Mindee node returns a JSON object with the following fields for a receipt prediction:  

| Field                      | Description                                                                                                  | Notes         |
|:---------------------------|:-------------------------------------------------------------------------------------------------------------|:--------------|
| id: string                 | UUID for the API request.                                                                                    |               |
| name: string               | Document name.                                                                                               |               |
| number_of_pages: number    | If using a PDF document with multiple pages, returns the number of pages processed by the Mindee API.        | Single images will return a value of 1 for this field.    |
| category: string           | The receipt category among 8 predefined classes.                                                             | toll, food, parking, transport, accommodation, gasoline, telecom, miscellaneous. The class 'telecom' will only be supported in the future.    |
| date: string               | Purchase date on the receipt given as an ISO date yyyy-mm-dd. Works for both European and US date formats.   |               |
| currency: string           | ISO 4217 code among 44 predefined currencies.                                                                | AED, ARS, AUD, BRL, CAD, CHF, CLP, CNY, COP, CZK, DKK, DZD, EUR, GBP, HKD, HUF, IDR, ILS, INR, JPY, KRW, MAD, MXN, MYR, NOK, OMR, PHP, PLN, QAR, RON, RUB, SAR, SEK, SGD, THB, TND, TRY, TWD, USD, VND, XAF, XOF, XPF, ZAR    |
| locale: string             | Two-letter language code (ISO 639-1) followed by two-letter country code (ISO 3166-1 alpha-2).               |               |
| supplier: string           | Name of the receipt supplier.                                                                                |               |
| taxes: object              |                                                                                                              |               |
| rate: number               | The tax rate in percentage.                                                                                  | 12% tax rate is given as a value of 12, not 0.12    |
| time: string               | Time of purchase with 24 hour formatting (hh:mm).                                                            |               |
| total_incl: number         | The total amount paid including taxes, discounts, fees, tips and gratuity.                                   |               |

## Invoice  

The Mindee node returns a JSON object with the following fields for an invoice prediction:  

| Field                      | Description                                                                                                  | Notes         |
|:---------------------------|:-------------------------------------------------------------------------------------------------------------|:--------------|
| id: string                 | UUID for the API request.                                                                                    |               |
| name: string               | Document name.                                                                                               |               |
| number_of_pages: number    | If using a PDF document with multiple pages, returns the number of pages processed by the Mindee API.        | Single images will return a value of 1 for this field.    |
| category: string           | Name of customer.                                                                                            |               |
| date: string               | Purchase date on the receipt given as an ISO date yyyy-mm-dd. Works for both European and US date formats.   |               |
| document_type: string      | Type of document.                                                                                            | Beta field, currently only returns either 'INVOICE' or 'CREDIT NOTE'.    |
| due_date: string           | Due date given as an ISO date yyyy-mm-dd. Works for both European and US date formats.                       |               |
| invoice_number: string     | Name of the receipt supplier.                                                                                |               |
| taxes: object              | Invoice number.                                                                                              |               |
| currency: string           | ISO 4217 code among 22 predefined currencies.                                                                | ISO 4217 code among 22 predefined currencies.    |
| supplier: string           | Name of  supplier.                                                                                           |               |
| taxes: object              |                                                                                                              |               |
| rate: number               | The tax rate in percentage.                                                                                  | 12% tax rate is given as a value of 12, not 0.12    |
| total_excl: number         | The total amount to be paid without taxes.                                                                   |               |
| total_incl: number         | The total amount to be paid.                                                                                 |               |
