y,x,h = map(int,input().split())

teigi_1,teigi_2,teigi_3,teigi_4,teigi_5 = map(int,input().split())
ryoukinn_1,ryoukinn_2,ryoukinn_3,ryoukinn_4,ryoukinn_5,ryoukinn_6 = map(int,input().split())

if h <= teigi_1:
    if y <= teigi_2 and x <= teigi_2:
        print(ryoukinn_1)
    elif y + x <= teigi_3:
        print(ryoukinn_2)
    else:
        print(ryoukinn_3)

elif y <= teigi_4 and x <= teigi_4 and h <= teigi_4:
    print(ryoukinn_4)

elif x + y + h <= teigi_5:
        print(ryoukinn_5)

else:
    print(ryoukinn_6 * y * x * h)
