def Bisection(f, a , b ):
    f_of_a = f(a)
    f_of_b = f(b)

    if f_of_a * f_of_b > 0:
        print("there is no root between a and b")
        return None

    for _ in range(50):
        midPoint = (a + b) / 2
        f_of_midPoint = f(midPoint)

        if f_of_midPoint == 0:
            return midPoint
        if f_of_a * f_of_midPoint > 0:
            a = midPoint
            f_of_a = f_of_midPoint
        if f_of_b * f_of_midPoint > 0:
            b = midPoint
            f_of_b = f_of_midPoint

    return midPoint


f = lambda x: x**3 - 2 * x - 3

a=1
b=2
print(f"Interval {a,b}")
x = Bisection(f, a, b)
print("last midPoint-point is :")
print(x)
