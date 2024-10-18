Q = float(input(“Enter the value of Load in kN: “)) * 1000 # converting kN to N

N = int(input(“Enter the number of data values of radial distance: “))

Z = float(input(“Enter the depth in meters: “)) # Depth is constant

R = []

# Getting radial distances

For I in range(1, N+1):

 Value_r = float(input(f”Enter radial distance {i} in meters: “))

 r.append(value_r)

# Calculate and display stress for each radial distance

For value_r in r:

 Stress = (3 * Q) / (2 * math.pi * Z**2) * ((1 / (1 + (value_r/Z)**2)) ** 2.5)

 Print(f”Radial distance: {value_r} m, Stress: {stress} N/m^2”)

OUTPUT:

Enter the value of Load in kN: 2500

Enter the number of data values of radial distance: 5

Enter the depth in meters: 6

Enter radial distance 1 in meters: 1

Enter radial distance 2 in meters: 2

Enter radial distance 3 in meters: 3

Enter radial distance 4 in meters: 4

Enter radial distance 5 in meters: 5

Radial distance: 1.0 m, Stress: 30962.1304453601 N/m^2

Radial distance: 2.0 m, Stress: 25479.163627896556 N/m^2

Radial distance: 3.0 m, Stress: 18980.334491124726 N/m^2
