# Introduction
This design is a 2 bike hitch rack that can carry up to 100lbs. My team and I chose this type of rack because we wanted to create an affordable (most hitch racks can reach up to $200) and reliable component.  
Hitch rack designs can carry bikes and can be adapted to carry skis, snowboards, cargo holders. 

## Initial Concept
![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/f37ffa47-123f-4526-8422-485f8ce099a3)
![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/7c0743a0-e5b0-4460-b748-b9033b2d833e)


## Final Design
![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/3b3aa662-f5c7-4ecc-af1e-153b8ddccfa8)
![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/f2877eaf-781a-4a96-90f7-a5d793447e5c)
![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/fbc243dd-cb31-4c33-adad-5c1d6414c4e6)

## Walkthrough
**Material selection**

Initial considerations where Aluminum and Steel, due to their relative properties. Aluminum is typically not as strong as steel, but it is also almost one-third of the weight. 

**Design**

Dimensions and overall design were based of initial concepts.

Sketches were made 3D using Autodesk Inventor.

**Calculations**

Equations, concepts, and constants were taken from notes and Shigley's Mechanical Engineering Design 10th Edition.

![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/f7bd4b27-d297-42cd-b6db-3b62003d25b1)


## Buckling Analysis

For Al 6061:

	E = 10.4 Mpsi = 10.4E6 psi__
 
	σ allow = 40,000 psi__
 
With the vertical beam:

	Area Moment of Inertia, I = 0.057 in4__
 
	Area, A = 4*0.125 = 0.5 in2__
 
	Distance to neutral axis, c = 0.5 in__
 
	Length of beam, L = 36 in__
 
	Eccentricity of load, e = 11.25 in__
 
Critical Load, Pcr = π ^2^ EI/L ^2^  = (π ^2^ * 10.4E6 * 0.057)/(36) ^2^ =4,514.4 lb.

Using non-dimensional eccentric buckling chart: P/P~cr~ = 0.1

	P= 0.1*4,514.4 = 451.4 lb.__
 
With Safety Factor of 4 for Dynamic Loading: P~allow~ = 451.4/3.0 = 115 lb.



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
![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/13952fed-b828-45be-a9c0-7fa1eb733bfe)


## Fatigue Analysis
Number of loads allowable before failure:
N = [(S’f/σ’f)(1/b)]/2 , where:
	S’f = fatigue strength = 40,000 psi
	σ’f = fatigue strength coefficient =  90,000 psi
	b = -[log(σ’f)/(S’e)]
		S’e = 0.5*S’f = 0.05*40,000 = 2000 psi
N = [(40,000/90,000)(1/(-.02))]/2 = 1.6E14 = 160,000,000,000,000 cycles
![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/721e8165-cbba-4fbd-9663-080cda799699)


## Stress Analysis
Bending stress: My/I 
	Y=Centroid
	 I=Moment of inertia
	Y=(18*2*1)+(13*2*35)+(32+*2*18)/(18*2+13*32*2)=16.65in
	Ixx’=bh^3/12 + b2h2^3/12 + A1y1^2 + b3h3^3/12 + A2y2^2= 1082.5 in^4

Bending stress=10lbs/in^2
![image](https://github.com/fsalaita/HitchBikeRackDesign/assets/146680465/ecbeb7fb-1401-4bf9-9f4b-68eafff4e2f2)


## Future-proofing
* A folding carry arm design allows the rack's arms to drop out of the way when not in use.
* A system that secures and protects bikes for safer travel.
* Extendable components to allow easy loading, unloading, and overall management of bikes.

## Contributors
* **Fares Salaita**
* **Eric Baldwin**
* **Austin Bray**





