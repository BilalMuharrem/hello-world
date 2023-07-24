resources = {
    "water": 300,
    "milk": 200,
    "coffee": 100,
}

water = 300
milk = 200
coffee = 100
money = 0
should_end = False

while not should_end:
    choice = input("What would you like? (espresso/latte/cappuccino): ")
    print("Please insert coins")
    quarters = int(input("How many quarters?: "))
    dimes = int(input("How many dimes?: "))
    nickles = int(input("How many nickles?: "))
    pennies = int(input("How many pennies?: "))

    def profit(money_in, quarters_in, dimes_in, nickles_in, pennies_in):
        money_in += (quarters_in * 0.25)
        money_in += (dimes_in * 0.1)
        money_in += (nickles_in * 0.05)
        money_in += (pennies_in * 0.01)
        return money_in

    a = profit(money_in=money, quarters_in=quarters, dimes_in=dimes, nickles_in=nickles, pennies_in=pennies)

    if choice == "espresso":
        if a >= 1.5:
            money += 1.5
            a -= 1.5
            print(f"Here is ${a} dollars in change.")
        else:
            print("Sorry that's not enough money. Money refunded.")
    elif choice == "latte":
        if a >= 2.5:
            money += 2.5
            a -= 2.5
            print(f"Here is ${a} dollars in change.")
        else:
            print("Sorry that's not enough money. Money refunded.")
    elif choice == "cappuccino":
        if a >= 3.0:
            money += 3.0
            a -= 3.0
            print(f"Here is ${a} dollars in change.")
        else:
            print("Sorry that's not enough money. Money refunded.")

    def calculation(choice_in, water_in, milk_in, coffee_in):
        if choice_in == "espresso" and water_in >= 50 and coffee_in >= 18:
            water_in -= 50
            coffee_in -= 18
            print("You can take your espresso")
        elif choice_in == "latte" and water_in >= 200 and milk_in >= 150 and coffee_in >= 24:
            water_in -= 200
            milk_in -= 150
            coffee_in -= 24
            print("You can take your latte")

        elif choice_in == "cappuccino" and water_in >= 250 and milk_in >= 100 and coffee_in >= 18:
            water_in -= 250
            milk_in -= 100
            coffee_in -= 24
            print("You can take your cappuccino")
        else:
            print("There is not enough sources")


        #print(water_in, milk_in, coffee_in)

    calculation(choice_in=choice, water_in=water, milk_in=milk, coffee_in=coffee)
