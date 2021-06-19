# currency_final_project
# Sayed Sadat
#CNE330-final
#06/18/2021
# https://thecleverprogrammer.com/2021/01/27/real-time-currency-converter-with-python/



from forex_python.converter import CurrencyRates
c = CurrencyRates()
amount = int(input("Enter the amount: "))
from_currency = input("From Currency: ").upper()
to_currency = input("To Currency: ").upper()
print(from_currency, " To ", to_currency, amount)
result = c.convert(from_currency, to_currency, amount)
print(round(result,2))
