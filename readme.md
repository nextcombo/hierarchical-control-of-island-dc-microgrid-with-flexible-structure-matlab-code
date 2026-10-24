# Hierarchical Control of Island DC Microgrid with Flexible Structure (Matlab Code Implementation)

​  
1. Overview of Microgrids (mG) are small-scale power grids composed of distributed generation units (DGU) and various loads. In addition to numerous advantages such as renewable energy integration, improved power quality, reduced transmission losses, and the capability to operate in both grid-connected and islanded modes, mGs are also compatible with AC and DC operating standards [1, 2, 3]. Notably, DC microgrids (DCmGs) have recently gained attention. Their increasing popularity can be attributed to the development of efficient converters, their natural interface with many renewable sources (such as photovoltaic modules), batteries, and a wide range of electronic loads (including various appliances, LEDs, electric vehicles, computers, etc.), essentially being DC [4, 5]. The stable operation of islanded DC microgrids (DCmG) is a multi-objective problem. Therefore, it requires a control entity to appropriately regulate internal voltage and effectively coordinate DGU operations while considering the non-deterministic absorption/production of load and renewable energy. For this purpose, a hierarchical architecture that spans across different control stages, time scales, and physical layers is typically adopted.
Editor
Figure 1: DC microgrid hierarchical control scheme
The hierarchical architecture of stacking one, two, and three levels is widely used in the operation and control of islanded DC microgrids (DCmG), which consist of distribution generation units (DGU), loads, and power lines. However, a comprehensive analysis across all layers is typically lacking. In this work, we address this limitation by setting up a top-down hierarchical control architecture. Distributed voltage controllers connected to DGUs form our primary layer. Under the management of an MPC-based energy management system (EMS), our third layer generates optimal power references and decision variables for DGUs. Specifically, decision variables can be used to turn on/off DGUs and select their operating modes. The intermediate secondary layer converts EMS power references into appropriate voltage signals required by the primary layer. More specifically, to provide voltage solutions, the second layer solves an optimization problem embedded with flow equations that are always solvable. Since the load voltage is not directly enforced, their uniqueness is necessary for DGUs to produce reference powers provided by the EMS. To this end, we infer a novel uniqueness condition solely based on local load parameters. Our control framework, besides being applicable to general DCmG topologies, can also adapt to topological changes caused by EMS commands. Its functionality is validated through simulation on a modified 16-node DC system. 2 Mathematical Model
Detailed mathematical models and explanations are provided in Part 4.
You can also click this link to download:
Hierarchical Control in Island DC Microgrids with Flexible Structure | IEEE Journals & Magazine | IEEE Xplore
Editor
3 Examples and Running Results
Editor
Editor
Editor
Editor
Editor
Editor
Editor
Editor
Editor
Editor
Editor
Editor
Editor
Editor
4. Matlab code and detailed article explanation: This article only displays a portion of the code, all code and detailed articles can be found in:
Editor
plot(t_plot(:, (sim_init)*(length(tr))+1 : (sim_end)*(length(tr)))/3600, y_plot(sourcenodes_mod, (sim_init-1)*(length(tr))+1 : (sim_end-1)*(length(tr)), 'linewidth', 2.5);
5 Conclusion In this paper, we propose a top-down hierarchical control structure for isolated DCmGs. Our monitoring controller located above the primary voltage layer consists of two and three levels. By utilizing load/generation forecasting and plotted measurement values from both loads and DGUs, our third-level EMS produces optimal power references that are meaningful to the primary voltage control layer. To make the EMS power reference meaningful to the primary voltage control layer, the secondary layer converts them into appropriate voltage references. More specifically, the voltage references are generated through an optimization problem that takes into account practical operational constraints such as DGU capacity limits and DCmG allowed voltage ranges. We investigated the completeness of the second-level optimization problem and derived new conditions for generator voltage and DGU power injection uniqueness. Finally, on a 16-node DCmG, we demonstrated how multiple layers of our hierarchical control scheme work together to achieve the desired objectives. Future work will focus on the development of the EMS, enabling DCmGs to operate in grid-connected mode without requiring full understanding of the DCmG topology's auxiliary layer. To design a fully scalable DCmG control architecture, we will also strive towards decentralization at the level of the second and third control layers.

## Images

![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](01.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](02.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](03.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](04.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](05.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](06.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](07.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](08.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](09.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](10.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](11.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](12.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](13.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](14.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](15.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](16.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](17.png)
![Hierarchical Control of Islanded DC Microgrid with Flexible Structure (Malab Code Implementation)](18.png)

<!-- PAYMENT_BLOCK -->

## Get this dataset

- Payment link (Stripe): [Buy now](https://buy.stripe.com/3cs8yP7sY87d0vu9AB)
- Payment QR code: ![Payment QR code](pay.png)

<!-- /PAYMENT_BLOCK -->
