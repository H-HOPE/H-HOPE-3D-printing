<div align="right">
<img src="/res/Logo_istituzionale.png" alt="drawing" width="250"/>
</div>


# 3D Printing of the energy harvester of the H-Hope project

The innovative technology for energy harvesting from hidden hydro sources, developed as part of the H-Hope project, has been intentionally designed to be accessible to users of all technical skill levels. The assembly process is straightforward, allowing individuals with minimal expertise to construct the device. Furthermore, the system is cost-effective, as it consists of 3D-printed components alongside a few metallic parts that are readily available at local stores. In this section, we provide a detailed Step-by-Step Guide for the 3D printing of these components.
&nbsp;

For the purpose of this guide, we will demonstrate the process using two professional-grade filament printers:  **a Bambu Lab X1 Carbon** printer and **a PRUSA MK3 printer**. Each printer comes along with a slicer software developed by the same company, i.e. **Bambu Studio** and **PRUSA Slicer**, respectively. However, it is important to emphasise that the same procedures can be followed with any 3D printer, including more affordable models. Moreover, both **Bambu Studio** and **PRUSA Slicer** supports slicing for a wide range of printer models from various vendors. This makes the software highly versatile and strongly recommended for use with different 3D printers. It is worth noting that both **PrusaSlicer** and **Bambu Studio** are quite similar in terms of functionality. They share many of the same symbols for their tools and also use similar terminology, making it easy to transition between the two programs. This compatibility allows users to switch from one software to the other smoothly, without needing to learn a completely new interface or workflow.  
- At the end of this tutorial, you will find a complete list of the files required for printing each component of the energy harvester. These files are also accessible in the **H-Hope Data Hub**, which can be found at the following site: **PLACE LINK HERE.**

***Importing an STL File into Bambu Studio and Generating a 3D Print File*** 
&nbsp;

The **Bambu Lab X1** printer is a versatile and powerful 3D printer, and using the **Bambu Studio** slicer allows you to prepare 3D models for printing efficiently. In this tutorial, we'll walk through the process of importing an STL file into Bambu Studio, configuring your print settings, and exporting the G-code file needed to print the object on a **Bambu Lab X1** printer.
&nbsp;
***What You’ll Need:***
•	**Bambu Studio** (the slicer software from _Bambu Lab_). You can download it from: https://bambulab.com/en/download/studio.
•	**STL files** (the 3D model you want to print). You can find the stl files corresponding to all the printable components of the H-Hope harvester below in this page. 
•	**Bambu Lab X1 printer**
•	**Bambu Lab filament** or other compatible filament: For this specific project, **PETG** (Polyethylene terephthalate glycol-modified) is an ideal choice when waterproofing is essential for the 3D-printed model. This filament provides excellent resistance to both water and moisture, creating an effective barrier, and it is also relatively easy to print with. Its durability and moisture-resistant characteristics make PETG particularly suitable for applications where exposure to water is a primary concern. Alternatively, filaments made from other common materials, such as **PLA** or **ABS**, can be used for this project. However, it is important to note that the overall durability and longevity of the harvester may be compromised when compared to using PETG. 
&nbsp;

***Step 1: Install and Open Bambu Studio***
- **Download and install Bambu Studio:**
•	Visit the **official Bambu Lab website** (https://www.bambulab.com/) and **download Bambu Studio** for your operating system (Windows/macOS/Linux).
•	**Install** the software following the standard installation procedure for your operating system.
- **Launch Bambu Studio:** Open the program by clicking on the Bambu Studio icon after installation.

***Step 2: Import Your STL File***
- **Open your STL file**:
•	In Bambu Studio, click on the cubic icon **“Add”** button located at the top left of the tool bar or simply drag-and-drop your .stl file into the workspace.
•	If space on the printer plate allows, you can print multiple parts simultaneously. 
- **Inspect the model:**
•	After importing, you will see your model displayed on the virtual print bed.
•	Use the mouse to rotate, zoom in/out, or pan around the model to ensure it has loaded properly.

&nbsp;
&nbsp;
add image 1
_Figure 1: Bambu Studio software layout. The screen shot shows an example of one of the H-Hope harvester parts being prepared for printing_
&nbsp;
&nbsp;

***Step 3: Prepare the Model for Printing***
Once the STL file is imported, you need to prepare it for slicing by adjusting its orientation, scale, and position.
- **Adjust orientation:**
•	Sometimes the model may import in a suboptimal orientation. To rotate the model:
	Select the model, then use the **“rotate”** tool located in the middle of the toolbar.
	Adjust the model's angles by clicking and dragging the rotation circles, or input precise values in the rotation boxes for each axis (X, Y, Z).
	You can also simply use the **“auto orient”** tool or lay on face tool to place the part in the best printing configuration. 
- **Scale the model** (if needed):
•	The parts provided in H-Hope project are already scaled, thus this step is not needed. However, if the model needs to be resized for a tailored fabrication, use the **“scale”** tool also available in the left toolbar.
•	You can scale uniformly or input specific dimensions for height, width, or depth.
- **Position the model on the print bed:**
•	Ensure the model is sitting flat on the build plate.
•	Use the move tool to centre or reposition the model on the virtual print bed.
•	If multiple parts will be printed, you can automatically arrange them on the plate with the button **“Arrange all objects”**.
**Step 4: Select the Print Settings**
Now that the model is properly oriented and positioned, it's time to configure the print settings for your **Bambu Lab X1 printer**.
- **Choose the printer profile:**
•	At the top-right corner of Bambu Studio, ensure that your specific model of Bambu Lab **printer and nozzle size** is selected as the active printer profile. If it is not available: Click on **“Add a new printer”** and select the Bambu Lab model from the list of available printers.
- **Select the material/filament:**
•	In the top-right section, under **Filament**, select the type of filament you're using (e.g., PLA, ABS, PETG, etc.). Bambu Lab offers its own filaments, but you can use compatible filaments by selecting the “Generic” filament or setting the appropriate settings provided by the filament vendor.
- **Configure slicing settings:**
•	On the right panel, you’ll find the following slicing settings:
	**Layer Height:** Choose a layer height for your print. Lower layer heights (e.g., 0.1 mm) provide finer detail but take longer, while higher layer heights (e.g., 0.28 mm) print faster but may have less detail.
	**Infill Density:** Set the infill percentage. Common values range from 10% to 20% for general prints, with higher infill offering more strength at the cost of print time and material.
	**Shell Thickness:** Adjust the number of outer perimeters. A thicker shell adds strength.
  	**Supports:** Enable **auto supports** if your model has overhangs that need extra support during printing.
	**Build Plate Adhesion:** You can enable a brim, raft, or skirt for better adhesion depending on the model’s footprint and material used.
The right configuration might vary for printer to printer. Typically, the default settings are suitable for the kind of parts used in the H-Hope project. You can find specific settings for PETG and PLA in the table below


&nbsp;
&nbsp;
&nbsp;

<div align="center">
<img src="./res/H-HOPE_footer.JPG" alt="drawing" width="1472"/>
</div>

