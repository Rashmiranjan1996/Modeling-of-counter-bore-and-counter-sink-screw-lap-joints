# Modeling-of-counter-bore-and-counter-sink-screw-lap-joints
In this work we predict the mechanical behavior (load-deformation) of various screw lap joints using a spring-mass model based approach. 
## Abstract
This paper presents an analytical approach to predict the mechanical behavior of different types of screw lap shear joints using a spring-mass model. The spring-mass model captures the axial, bending, bearing, and shear stiffnesses of the components and their masses at the joint. The springs in the model represent the stiffness arising from each of these modes of deformation. We derive the expressions of the individual stiffnesses analytically and use the spring-mass model to obtain the overall joint stiffness. We show that this joint stiffness accurately predicts the experimentally observed mechanics of counter-bore and countersink screw lap joints. The experimental validation is carried out in nine different joint configurations. The analytical model is also validated with the aid of linear finite element analysis. Furthermore, the influence of individual stiffness components on the overall joint behavior is studied by varying the thickness and width of the plates.

## Analytical-model
| <img src="https://user-images.githubusercontent.com/110676380/183095488-1deb9c29-25f6-4b7f-98b6-c7fb479e9dfb.jpg" width="450"> | <img src="https://user-images.githubusercontent.com/110676380/183095492-fe4d8bd9-5e3b-4834-b0c6-8c1e9e2a69e7.jpg" width="450"> |
|:--:| :--:|
|*Schematic Counter-bore screw lap joint.*|*Schematic Countersink screw lap joint.*|

Here we intended to obtain an analytical expression for the total deformation in the joint when an axial load P is applied at one end of a screw lap joint, presented in Figure 1. When the joint is under external loading as shown in Figure 3, the plates experience tensile and bearing load. At the same time, the screw resists the combined effect of shear, bearing, and bending loads. The total deformation in the joint is contributed by each of these loads experienced by the plates and the screw. Thus, the complex deformation at the joint can be simplified and represented using a lumped spring model (Figure 3), where there is a spring to account for every mode of deformation in the plates and the screw.

<p align="center">
  <img src="https://user-images.githubusercontent.com/110676380/183098955-24e81b34-5582-4333-b733-320699db05bb.jpg" width="450">
  
  <em>Forces developed in a screw lap joint with an axial load, P [Note: The arrows indicate the region in which the forces
are developed].</em>
</p>

Employing classical mechanics theories such as Timoshenko beammodel, Castiglianlo's theorem, each deformation component are evalutaed.

<p align="center">
  <img src="https://user-images.githubusercontent.com/110676380/183100379-92596333-d0d0-4288-99eb-4a7b0eb905e9.jpg" width="550">
  
  <em>Mass-spring model representation of screw lap joint.</em>
</p>

Subsequently, the above spring-mass model was solved to get the load-deformation behavior of the joints. Which was later verified with experimental results and FE models.

## FE models
FEA studies were conducted with the aid of ABAQUS software (Version-2018). The constructed FE models are presented in
Figure 4. Here, both the plates and screw were modeled using eight-node linear brick elements (C3D8R). In total 45278 elements are used to develop the entire joint assembly while ensuring a finer mesh near the joint area.

<p align="center">
  <img src="https://user-images.githubusercontent.com/110676380/183102385-715837e3-8d1b-4396-b75b-eb1c2ef0ff5c.png" width="550">
  
  <em>3D Finite element model of joint configuration and counter-bore and countersink screws .</em>
</p>

## Results-1: Comparison between analytical, FEA and experimental results 
The load-deformation curves obtained from analytical, FEA, and experimental results of two
types of lap joint configurations (viz. counter-bore and countersink) are shown in Figures 5. These graphs show very good agreement between the present analytical model with FEA and experimental results and thereby validating the accuracy of the proposed analytical model.

| <img src="https://user-images.githubusercontent.com/110676380/183103803-24421c20-f92a-4ba1-a62a-43dac8b2fe69.jpg" width="400"> | <img src="https://user-images.githubusercontent.com/110676380/183103895-4b8ab952-a351-4008-86c2-5d1fb0adc97d.jpg" width="400"> |
|:--:| :--:|
|*Counter-bore screw lap joint behavior.*|*Counter-bore screw lap joint behavior.*|

## Results-2: Effect of individual component stiffness 
Figure 6 represents individual component stiffness's effect on global joint stiffness. There we can observe that the screw bending stiffness governs the overall joint behavior for thicker plates, whereas, for thinner plates, this is done by plates' axial stiffness. But the variation in plate width (Fig. 6b) doesn't change individual componet's effect as significant as change in plate thickness. 

| <img src="https://user-images.githubusercontent.com/110676380/183122734-fff9dd38-cf07-4c9a-a7df-13b898bbb26b.jpg" width="400"> | <img src="https://user-images.githubusercontent.com/110676380/183122736-d13d8c06-d972-49f1-be3e-838a4e7b8c78.jpg" width="400"> |
|:--:| :--:|
|*Influence of individual component stiffness with variation in plate thickness. *|*variation in plate thicknes plate width.*|

## Conclusion
1. In this paper, we presented a theoretical model to predict the joint stiffness of three different types of screw lap joints where the use of correction factors for stiffness estimation as adopted in existing literature are completely removed.
2. Also, the influence of the plate thickness and plate width on the overall joint stiffness was analyzed. We found that plate stiffness has more influence on overall joint stiffness in thin plate joints, whereas in joints with thicker plates, screw stiffness (bending stiffness) dominates the overall joint stiffness.










