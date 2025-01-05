# Auction-Project

auc=False
auction={}
while not auc:
    c=input("Do you want to bet(yes or no): ")
    if c == "yes":
        a=input("Enter the name: ")
        b=int(input("Enter the amount: "))
        auction[a]=b
    else:
        auc=True

if auction:
    winner = max(auction,key=auction.get)
    result = auction[winner]
    print (f"The winner is: {winner} {result}")
