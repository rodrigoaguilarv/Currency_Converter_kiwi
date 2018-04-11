# Currency_Converter_kiwi
-Currency converter CLI and Web API for Kiwi

-It use the rates from the European Central Bank. http://www.ecb.europa.eu/stats/policy_and_exchange_rates/euro_reference_exchange_rates/html/index.en.html 

## Note

- Currency symbols are not supported. It can be confusing for users 

## Example

### CLI
```
./currency_converter.py --amount 100.0 --input_currency EUR --output_currency CZK
{   
    "input": {
        "amount": 100.0,
        "currency": "EUR"
    },
    "output": {
        "CZK": 2707.36, 
```
### API
```
GET /currency_converter?amount=0.9&input_currency=EUR&output_currency=AUD HTTP/1.1
{   
    "input": {
        "amount": 0.9,
        "currency": "CNY"
    },
    "output": {
        "AUD": 0.20, 
    }
}
