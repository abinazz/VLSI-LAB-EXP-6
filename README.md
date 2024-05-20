# VLSI-LAB-EXP-6
# AIM:
To design and simulate the CMOS inverter and observe the DC and transient responses using cadence tool.

# APPARATUS REQUIRED:
1.Laptop with MobaXterm

2.Cadence tool PROCEDURE SCHEMATIC ENTRY: Creating a new library:

3.In the library manager, execute File - New library. The new library form appears.

4.In the new library form, type ‘my design lib’ in the name section.

5.In the field of directory section, verify that the path to the library is set to ~/Database / Cadence- analog – lab –bl3 and click ok.

6.In the next ‘technology file for new library form select option attach to an existing tech file and click ok.

7.In the ‘attach design library to technology file’ form, select gpdk045 form the cyclic field and click ok.

8.After creating a new library you can verify it from the library manager.

9.If you right click on the ‘my design lib’ and select properties, you will find that gpdk045 library is attached as techlib to ‘my design lib’.

# Creating a schematic cell view:
1.In the CIW or library manager, execute file – new – cell viw.

2.Setup the new file form as follows, Do not edit the library path file and the above might be different from the path shown in your form.

3.Click ok when done the above setting. A black schematic window for the inverter design appears.

# Adding components to schematic:
1.In the inverter schematic window, click the instance fixed menu icon to display the add instance form.

2.Click on the browse button. This opens up a library browser from which you can select components and the symbol view.

3.After you complete the add instance form move your cursor to the schematic window and click left to place a component. LIBRARY NAME CELL NAME gpdk045 PMOS gpdk045 NMOS

4.This is a table of components for building the inverter schematic.

5.After entering components, click cancel in the add instance form or press ESC with your cursor in the schematic window.

![ABI 6(1)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/76bfda49-944a-436c-b300-c5d2e5ac4a3d)


# Adding pins to schematic:
1.Click the pin fixed menu icon in the schematic window. You can execute create pin or press ‘p’.

2.Add pin form appears. Type the following in the ADD pin form in the next order leaving space between the pin. PIN NAMES DIRECTION Vin,Vdd,Vss Input Vout Output

3.Select cancel and then the schematic window enter window file or press the f bind key. Adding wires to schematic:

4.Click the wire (narrow) icon in the schematic window.

5.In the schematic window click on a pin of one of your components as the first point for your wiring. A diamond shape appears over the starting point of this wire.

6.Follow the prompts at the bottom of design window and click left on the destination point for your wire. A wire is routed between the source and destination points.

7.Complete the wiring as shown in the figure and when done wiring press ECS key in the schematic window to cancel wiring.

# Saving the design:
Click the check and save icon in the schematic editor window observe CIW output for any errors.

# BUILDING THE INVERTER TEST DESIGN: Creating the inverter test cell view:
1.In the CIW or library manager, execute file – new – cell view.

2.Setup the newfile as shown below.

3.Click ok when done. A blank schematic window for the inverter test design appears.

4.Using the components list and properties/ comments in this table build the inverter test schematic. LIBRARY NAME CELL VIEW NAME PROPERTIES/COMMENTS My design lib Inverter Symbol Analog lib Vpulse Voltage1 = 0, Voltage2 = 1.8, delay Time = 0, Rise time=Fall time=1ns Period=20ns Analog lib Vdc, gnd Vdc = 1.8v

5.Add the above components using create – instance or by pressing I.

6.Click the wire (narrow) icon and wire your schematic.

7.Click create wire name or press c to name the i/p (vsin) and output wires as in below schematic.

8.Click on the check and save icon to save the design.

![ABI 6(2)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/4dc58d0f-1651-4435-aece-097fed857816)


# ANALOG SIMULATION WITH SPECTRA: Starting the simulation environment:
1.In the Inverter-test schematic window execute launch – ADEL. The variable virtuoso analog design environment (ADE) simulation window appears. Choosing a simulator:

2.In the simulation window (ADE) execute setup – simulator / directory / host.

3.In the choosing simulator form, set the simulator field to specra and click ok.

4.In the simulation window (ADE) execute the setup model libraries. To complete, move the cursor and click ok. Choosing Analysis:

5.Click the choose- Analysis icon in the simulation window (ADE).

6.The choosing analysis form appears.

7.To Setup the transient analysis. a. In the analysis section select tron. b. Set the stop time as 100ns c. Click at the moderate or enabled button and the bottom and then click apply.

8.To set for DC analysis a. In the analysis section select DC. b. Turn on save DC operating point. c. Turn on the component parameters. d. Double click the select Vpulse source or Type V0 (capital V zero). e. Select the DC voltage in the select window parameter and click in the form start and stop voltages are 0 to 1.8. f. Select the enable button and click apply and then click ok.

Selecting output for plotting:

1.Execute the o/p’s to be plotted -select on sschematic in the simulation window.

2.Follow the prompt at the bottom. Click on the o/p net vout input vin of the inverter. Press esc with the cursor after selecting.

# Running the simulation:
1.Execute the simulation Netlist and run in the simulation window to start the simulation on the icon. This will create the netlist as well as run the simulation.

2.When the simulation finishes the transient and DC plots automatically will be popped up along with netlist.

![ABI 6(3)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/532efeb8-78e1-47a6-8deb-346fcd55d00f)


![ABI 6(4)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/1d854898-c8f1-4c0b-a8ef-2df17de69ac0)


# CMOS NAND GATE
# NAND SCHEMATIC
![ABI 6(5)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/14b6fb6b-ea77-4faf-8a99-76bb59f76977)


# NAND TEST CELL VIEW
![ABI 6(6)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/6e6163fe-0bba-4577-a24e-53fb04f90afe)


# NAND SIMULATION WITH SPECTRA
![ABI 6(7)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/853f53c8-42e8-4009-ac6e-596036231aba)


# CMOS NOR GATE
# NOR SCHEMATIC
![ABI 6(8)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/7d732719-54dc-4234-801f-2dc206b36e58)


# NOR TEST CELL VIEW
![ABI 6(9)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/7c683cd7-c98b-4bde-9245-d47bdecb5140)


# NOR SIMULATION WITH SPECTRA
![ABI 6(10)](https://github.com/navaneethans/VLSI-LAB-EXP-6/assets/165630162/91db44c9-8351-4f62-a8b5-63f6001ba91c)


# RESULT:
THe design and simulation of the CMOS inverter and the DC and transient responses using cadence tool is successfully observed and verified.
