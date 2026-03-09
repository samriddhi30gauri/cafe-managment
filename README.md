# cafe-managment
menu={
    'Pizza':40,
    'Pasta':50,
    'Burger':60,
    'Salad':70,
    'Coffee':80,

}

##Greet
print("welcome to Python Restaurant ")
print("Pizza:Rs40\nPasta: Rs 50\nBurger: Rs60\nSalad:Rs60\n:Rs70\nC0offee:Rs80")

order_total=0
item_1=input("Enter the name of item you want to order=")
if item_1 in menu:
    order_total+=[item_1]
    print(f"Your item {item_1} has been added to your order")

else:
    print("Please order something else we can serve you")
    another_order=input("Do youn want to add another item(Yes/No)")
    if another_order=="Yes":
        item_2=input("Enter the name of second item=")
        if item_2 in menu:
            order_total +=menu[item_2]
    else:
        print(f"Ordered item {item_2} is not available!")

    print(f"the total amount of item is {order_total}")
