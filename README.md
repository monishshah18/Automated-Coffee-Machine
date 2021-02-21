# Automated-Coffee-Machine
----------------

A Simple Coffee Machine that dispenses drinks. It has the following properties:

### Properties
1. It will be serving some beverages.
2. Each beverage will be made using some ingredients.
3. Assume time to prepare a beverage is the same for all cases.
4. The quantity of ingredients used for each beverage can vary. Also, the same ingredient (ex:water) can be used for multiple beverages.
5. There would be ​N​​( N is an integer )​ outlet from which beverages can be served.For N = 2 [ 2 outlets in a machine ]For N = 3 [ 3 outlets in a machine ]
6. Maximum ​N​ beverages can be served in ​parallel​.
7. Any beverage can be served only if all the ingredients are available in terms of quantity.
8. There would be an indicator that would show which all ingredients are running low. There should be some methods to refill them.
9. Tests have been added as part of unit test to validate the source code. Also these tests have been integrated with Github Actions so as to validate each and every code changes.

### Usage
* The input will be taken from `resources/input.json`.
* While being in the project root, run `python3 main.py` to dispense drinks.
NOTE: Required python is 3.7 and above
* This Machine is flexible to handle different items, user needs to modify `resources/input.json` according to his/her needs.

### Output
* Display result to stdout. Following is the example output.
```
hot_coffee is prepared
hot_tea is prepared
black_tea cannot be prepared because hot_water, sugar_syrup are not available
green_tea cannot be prepared because sugar_syrup, green_mixture are not available
```
### Run tests
While being in the project root run following commands:

```
cd tests
pytest --verbose
```