# -showing-the-BDD-Scenario-for-Searching-a-Product-based-on-Name
Scenario: Searching a product by name
  Given the following products
    | name   | category | available |
    | ToyCar | Toys     | true      |
  When I search for the product with name "ToyCar"
  Then I should see the product with name "ToyCar"
