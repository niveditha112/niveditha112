
tshirts = float(input("Enter tshirt Quantity :"))
jacket	= float(input("Enter jacket Quantity :"))
cap = float(input("Enter cap Quantity :"))
notebook = float(input("Enter notebook Quantity :"))
pens = float(input("Enter pens Quantity :"))
markers = float(input("Enter marker Quantity :"))
trate = 1000.0
jrate = 2000.0
crate = 500.0
nrate = 200.0
prate = 300.0
mrate = 500.0

tamount = trate*tshirts
jamount = jrate*jacket
camount = crate*cap
namount = nrate*notebook
pamount = prate*pens
mamount = mrate*markers
amount = tamount+jamount+camount+namount+pamount+mamount
print("Amount = ",amount)

if(amount >= 1000):
    discount = 10
elif(amount>=3000 and amount<=99999):
   discount = 15
else:
   discount = 0

discountAmount = (amount*discount)/100
netAmt = amount - discountAmount

if(amount >= 100):
    netAmt = amount + 10

print("Discount = %d%% and Discount Amount = %.2f"%(discount,discountAmount))
print("tshirt = %.2f , jacket = %.2f , cap = %.2f , notebook = %.2f , pens = %.2f , markers = %.2f"%(tshirts,jacket,cap,notebook,pens,markers))

print("Net Amount = ",netAmt)
