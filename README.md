# Compliant-Mechanism

A mechanism is a mechanical device which used to transfer or transform motion, force or energy. Traditional mechanisms are mostly rigid link mechanisms whereas the name suggests the links are rigid. On the Contrary compliant mechanisms are also used to perform the same task but unlike the former they rely on the flexibility of the members, eg: - Compliant Crimping mechanism. The biggest advantage of Compliant Mechanism over Rigid link mechanisms is the reduction in the number of moving parts. These advantages make compliant mechanisms ideally suited for space or aerospace applications, where low weight and no lubrication are essential.

Inspite of Compliant mechanisms having numerous advantages, the biggest difficulty lies in the design and analysis of them. Despite the advancement in the theory relating to Compliant Mechanisms, typically analysis and design of compliant mechanisms is tougher than for a rigid link mechanism. For Compliant Mechanism, link geometry, material properties and loading all become important considerations. As most of the deflections which are involved are often large hence it rules out linear deflection equations.

 # Material Consideration for Compliant Mechanism

### Ratio of Strength to Young’s Modulus
As flexibility is desirable in complaint mechanism, therefore members having low Young’s Modulus should be preferred but apart from Flexibility, Strength of a material also plays a vital role. If you view the formulae for the maximum deflection of cantilever beam with a load applied to its edge.
δ_max=  (2*S_y*L^2)/(3*E*h)
You can see that the maximum deflection is proportional to the ratio of S_y/E.   
The material with the highest strength to modulus ratio will allow large deflection before failure, which is often the deciding criterion for selecting material in a Complaint Mechanism.
Material	E[GPa]	S_y[MPa]	S_y⁄E
Spring Steel	206	1158	177.89
Titanium	108	883	122.31
Aluminum (Al 6061)	68.67	241	284.93
Beryllium Copper	132.43	1000.62	132.43

### Pseudo Rigid Body Model
The Pseudo Rigid Body Model is used to model the deflection of model the deflection of flexible members using rigid body components that have equivalent Force - displacement relationship. The method is particularly very helpful in the design of compliant mechanism as it provides a simple method of analysing systems that undergo large, nonlinear deflections.
Here is the brief discussion about the segments and their equivalent model which has been used in the given project:
2.1.1. Small Length Flexural Pivots
 
Figure 3. Small Length Flexural Pivot
The beam has two segments, one is the short and flexible and the other is long and rigid. If the small segment is significantly shorter than the longer segment then that is called a small length flexural pivot.
The small segment is flexible, and we find deflection in the Pseudo rigid Body Model using it. 
K=〖(EI)〗_l/l
 
Figure 4. Pseudo Rigid Body Model

2.1.2. Living Hinges
When the small segment in the small-length flexural pivots is extremely short and thin then it is called a living hinge. The pseudo rigid body model of it is a revolute joint as it Torsional stiffness is very low and hence offers no resistance to rotation.
 
Figure 5. An example of Living Hinge


2.1.3. Cantilever beam with a force at the free end
 
Figure 6. Cantilever Beam
The PRBM for this segment was proposed by Howell and Midha[], and consists of two body links with one torsional spring placed at the characteristic pivot.  The length of the rigid links is calculated using γ (characteristic radius), which is a function of n or the Load factor. Load factor is the ratio of the axial force (nP) and the transverse force (P). The spring stiffness of the torsional spring k is a function of characteristic radius factor γ and the 45 beam stiffness coefficient KΘ. The beam end angle is represented by θ_o, and pseudorigid-body angle by Θ. The beam end angle and pseudo-rigid-body angle are related with the parametric angle coefficient cθ.
 
Figure 7. Pseudo Rigid Body Model

	
The characteristic radius factor γ is given by:
	γ = 0.912364 + 0.0145928 n			(for − 5 <n ≤ −1.8316)
γ = 0.852144 − 0.0182867 n			(for − 1.8316 <n ≤−0.5)
γ = 0.841655 − 0.0067807 n + 0.000438n^2		(for − 0.5 <n ≤ 10)

As a rule of thumb, as an approximation γ_avg can be taken as 0.85.
To define the torsional stiffness constant of the spring we define a stiffness coefficient,K_Θ . The stiffness coefficient is also a function of the load factor, hence depends on the orientation of the non - follower force. 
For a rough estimate we can take K_Θavg = 2.65.
Torsional Spring constant is given by 
K=γK_Θ  EI/l
Where E is the Young’s Modulus, I is Area Moment of Inertia, l is the length of the beam.

