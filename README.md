# Introduction
This design is a 2 bike hitch rack that can carry up to 100lbs. we chose this type of rack because we wanted to create an affordable (most hitch racks can reach up to $200) and reliable component.  
Hitch rack designs can carry bikes and can be adapted to carry skis, snowboards, cargo holders. 

## Initial Concept
![image](https://github.com/fsalaita/Portfolio/assets/146680465/5c9f5a28-5823-422e-a872-3cb45426731a)
![image](https://github.com/fsalaita/Portfolio/assets/146680465/56e037c2-1e2b-4cef-8974-5a531caf7e5a)

## Final Design
![image](https://github.com/fsalaita/Portfolio/assets/146680465/6dde412f-ad9b-4f33-bc7b-eece75740845)
![image](https://github.com/fsalaita/Portfolio/assets/146680465/aa538a57-e97c-4495-883d-dde91190440e)
![image](https://github.com/fsalaita/Portfolio/assets/146680465/211adbc2-1306-4603-ae42-d49a084ff1b8)

## Walkthrough
**Material selection**

Initial considerations where Aluminum and Steel, due to their relative properties. Aluminum is typically not as strong as steel, but it is also almost one-third of the weight. 

**Design**

Dimensions and overall design were based of initial concepts.

Sketches were made 3D using Autodesk Inventor.

**Calculations**

Equations, concepts, and constants were taken from notes and Shigley's Mechanical Engineering Design 10th Edition.

![image](https://github.com/fsalaita/Portfolio/assets/146680465/a13fe782-0df4-40c6-95d1-c2da2843338a)

## Buckling Analysis
For Al 6061:
	E = 10.4 Mpsi = 10.4E6 psi
	σ allow = 40,000 psi
With the vertical beam:
	Area Moment of Inertia, I = 0.057 in4
	Area, A = 4*0.125 = 0.5 in2
	Distance to neutral axis, c = 0.5 in
	Length of beam, L = 36 in
	Eccentricity of load, e = 11.25 in
Critical Load, Pcr = π2EI/L2 = (π2 * 10.4E6 * 0.057)/(36)2 =4,514.4 lb.
Using non-dimensional eccentric buckling chart: P/Pcr = 0.1
	P= 0.1*4,514.4 = 451.4 lb.
With Safety Factor of 4 for Dynamic Loading: Pallow = 451.4/3.0 = 115 lb. 
![image](https://github.com/fsalaita/Portfolio/assets/146680465/806f9f3f-90bb-429f-b057-2113468998a6)

## Shear Analysis on Bolts
Shear, σ = F/(n*A)
	n = number of bolts in vertical alignment
	A = t*d,
		t = sum of thickness of walls
		d = diameter of bolts
Shear stress on bolts in top bracket: 
	σ=100lb/(2*.5*.375) = 266.67psi/bolt
Shear stress on bolts in bottom bracket:
	σ= (100+2.43)/(3*.5*.375) = 182.1psi/bolt 
![image](https://github.com/fsalaita/Portfolio/assets/146680465/a1ca33f9-9483-44af-b232-fa26785fc43e)

## Fatigue Analysis
Number of loads allowable before failure:
N = [(S’f/σ’f)(1/b)]/2 , where:
	S’f = fatigue strength = 40,000 psi
	σ’f = fatigue strength coefficient =  90,000 psi
	b = -[log(σ’f)/(S’e)]
		S’e = 0.5*S’f = 0.05*40,000 = 2000 psi
N = [(40,000/90,000)(1/(-.02))]/2 = 1.6E14 = 160,000,000,000,000 cycles
![image](https://github.com/fsalaita/Portfolio/assets/146680465/e6c66923-6108-4cda-b44d-ad2ffceb6b43)

## Stress Analysis
Bending stress: My/I 
	Y=Centroid
	 I=Moment of inertia
	Y=(18*2*1)+(13*2*35)+(32+*2*18)/(18*2+13*32*2)=16.65in
	Ixx’=bh^3/12 + b2h2^3/12 + A1y1^2 + b3h3^3/12 + A2y2^2= 1082.5 in^4

Bending stress=10lbs/in^2
![image](https://github.com/fsalaita/Portfolio/assets/146680465/da872974-3347-4a66-9f14-d4028dbf4d6c)

## Future-proofing
* A folding carry arm design allows the rack's arms to drop out of the way when not in use.
* A system that secures and protects bikes for safer travel.
* Extendable components to allow easy loading, unloading, and overall management of bikes.

## Contributors
* **Fares Salaita** - [fsalaita] (github.com/fsalaita/)
* **Eric Baldwin**
* **Austin Bray**





