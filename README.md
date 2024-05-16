# VLSI-LAB-EXP-6

**AIM:**
To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

**APPARATUS REQUIRED:**
1.	Laptop with MobaXterm
2.	Cadence tool

**PROCEDURE**
Creating a new library:
1.	In the library manager, execute File - New library. The new library form appears.
2.	In the new library form, type ‘my design lib’ in the name section.
3.	In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.
4.	In the next ‘technology file for new library form select option attach to an existing tech file and click ok.
5.	In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.
6.	After creating a new library you can verify it from the library manager.
7.	If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

Creating a schematic cell view:
1.	In the CIW or library manager, execute file – new – cell viw.
2.	Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.
3.	Click ok when done the above setting. A black schematic window for the inverter design appears.

Adding components to schematic:
1.	In the inverter schematic window, click the instance fixed menu icon to display the add instance form.
2.	2.	Click on the browse button. This opens up a library browser from which you can select components and the symbol view.
3.	After you complete the add instance form move your cursor to the schematic window and click left to place a component.
4.	This is a table of components for building the inverter schematic.
5.	After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.

![329845465-ff2e4de9-cd56-4227-8ce4-c9887921b4f2](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/a6dbb28c-dded-427f-9330-262f32ac7d21)

 Adding pins to schematic:
1.	Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.
2.	Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin.
3.	Select cancel and then the schematic window enter window file or press the f bind key.
Adding wires to schematic:
1.	Click the wire (narrow) icon in the schematic window.
2.	In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.
3.	Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.
4.	Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.
Saving the design: Click the check and save icon in the schematic editor window observe CIW output for any errors.

BUILDING THE INVERTER TEST DESIGN:

Creating the inverter test cell view:
1.	In the CIW or library manager, execute file – new – cell view.
2.	Setup the newfile as shown below.
3.	Click ok when done. A blank schematic window for the inverter test design appears.
4.	Using the components list and properties/ comments in this table build the inverter test schematic.
5.	Add the above components using create – instance or by pressing I.
6.	Click the wire (narrow) icon and wire your schematic.
7.	Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.
8.	Click on the check and save icon to save the design.

![329845717-4bf6bbe3-c876-45b8-8d0c-681a2591aa43](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/b8122edf-9ba5-4de0-9b0b-c849a2775c9c)

ANALOG SIMULATION WITH SPECTRA:

Starting the simulation environment:

1.	In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears. Choosing a simulator:
2.	In the simulation window (ADE) execute setup – simulator / directory / host.
3.	In the choosing simulator form, set the simulator field to specra and click ok.
4.	In the simulation window (ADE) execute the setup model libraries. To complete, move the cursor and click ok. Choosing Analysis:
5.	Click the choose- Analysis icon in the simulation window (ADE).
6.	The choosing analysis form appears.
7.	To Setup the transient analysis. a. In the analysis section select tron. b. Set the stop time as 100ns c. Click at the moderate or enabled button and the bottom and then click apply.
8.	To set for DC analysis a. In the analysis section select DC. b. Turn on save DC operating point. c. Turn on the component parameters. d. Double click the select Vpulse source or Type V0 (capital V zero). e. Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8. f. Select the enable button and click apply and then click ok.

Selecting output for plotting:
1.	Execute the o/p’s to be plotted -select on sschematic in the simulation window.
2.	Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

Running the simulation:
1.	Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.
2.	When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.


![329845746-0cfb0830-cee0-40e2-ba57-b04aed38a170](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/8e38982e-1231-4e1e-a932-9942bef034ab)

![329845769-fa4259ee-1da9-4989-9aef-af6634dbfd3e](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/995ebf89-46ce-4147-a6db-c46a066c3d10)

CMOS NAND GATE

NAND SCHEMATIC

![329845783-30bbf675-116a-4910-9195-37c198f40890](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/795ae677-4db7-4f0b-a842-f1b8af0cf83d)

NAND TEST CELL VIEW

![329845846-0a7baba8-dd19-45e6-8a97-e0b7be9462c8](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/a06f1d64-5cac-44f6-8ed2-b473c26a9acd)


NAND SIMULATION WITH SPECTRA

![329845863-9b180d74-92c7-42aa-8652-30e7fbe89260](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/d8e97de1-544d-4bfb-8d80-61117c6b2630)

CMOS NOR GATE

NOR SCHEMATIC

![329845885-3ec2637c-b359-430d-9642-10b92ebfdedb](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/7451b52f-20f8-457d-81f3-edd5d5c963ad)

NOR TEST CELL VIEW

![329845904-cd64ffe6-7ddb-47e3-8f66-256e15c62e45](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/f39d1142-b35e-438d-b710-8fb73de7143d)

NOR SIMULATION WITH SPECTRA

![329845913-40828e25-0474-43c1-8e49-0d297ae6a11a](https://github.com/kailashkarthikeyan/VLSI-LAB-EXP-6/assets/160568677/2e605d13-e35c-424f-8395-58d4edff252a)

RESULT:
