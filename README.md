<div align="right">
<img src="/res/Logo_istituzionale.png" alt="drawing" width="250"/>
</div>


# 3D Printing of the energy harvester of the H-Hope project

The innovative technology for energy harvesting from hidden hydro sources, developed as part of the H-Hope project, has been intentionally designed to be accessible to users of all technical skill levels. The assembly process is straightforward, allowing individuals with minimal expertise to construct the device. Furthermore, the system is cost-effective, as it consists of 3D-printed components alongside a few metallic parts that are readily available at local stores. In this section, we provide a detailed Step-by-Step Guide for the 3D printing of these components.
&nbsp;

For the purpose of this guide, we will demonstrate the process using two professional-grade filament printers:  **a Bambu Lab X1 Carbon** printer and **a PRUSA MK3 printer**. Each printer comes along with a slicer software developed by the same company, i.e. **Bambu Studio** and **PRUSA Slicer**, respectively. However, it is important to emphasise that the same procedures can be followed with any 3D printer, including more affordable models. Moreover, both **Bambu Studio** and **PRUSA Slicer** supports slicing for a wide range of printer models from various vendors. This makes the software highly versatile and strongly recommended for use with different 3D printers. It is worth noting that both **PrusaSlicer** and **Bambu Studio** are quite similar in terms of functionality. They share many of the same symbols for their tools and also use similar terminology, making it easy to transition between the two programs. This compatibility allows users to switch from one software to the other smoothly, without needing to learn a completely new interface or workflow. &nbsp;

At the end of this tutorial, you will find a complete list of the files required for printing each component of the energy harvester. These files are also accessible in the **H-Hope Data Hub**, which can be found at the following site: 
<a href="https://github.com/H-HOPE/Data-Hub"> **H-HOPE Data Hub**</a>
<br />

## Table of content

- [Importing an STL File into Bambu Studio and Generating a 3D Print File,](#bambu)
- [Importing an STL File into PrusaSlicer and Generating a 3D Print File,](#prusa)
- [Part List for 3D Printing the H-Hope Project Energy Harvester](#parts)
<br />

## Importing an STL File into Bambu Studio and Generating a 3D Print File<a name="bambu"></a>

The **Bambu Lab X1** printer is a versatile and powerful 3D printer, and using the **Bambu Studio** slicer allows you to prepare 3D models for printing efficiently. In this tutorial, we'll walk through the process of importing an STL file into Bambu Studio, configuring your print settings, and exporting the G-code file needed to print the object on a **Bambu Lab X1** printer.
<br />

### What You’ll Need:


•	**Bambu Studio** (the slicer software from _Bambu Lab_). You can download it from: https://bambulab.com/en/download/studio.<br />
•	**STL files** (the 3D model you want to print). You can find the stl files corresponding to all the printable components of the H-Hope harvester below in this page. <br />
•	**Bambu Lab X1 printer**<br />
•	**Bambu Lab filament** or other compatible filament: For this specific project, **PETG** (Polyethylene terephthalate glycol-modified) is an ideal choice when waterproofing is essential for the 3D-printed model. This filament provides excellent resistance to both water and moisture, creating an effective barrier, and it is also relatively easy to print with. Its durability and moisture-resistant characteristics make PETG particularly suitable for applications where exposure to water is a primary concern. Alternatively, filaments made from other common materials, such as **PLA** or **ABS**, can be used for this project. However, it is important to note that the overall durability and longevity of the harvester may be compromised when compared to using PETG. <br />
&nbsp;
<br />

### Step 1: Install and Open Bambu Studio

- **Download and install Bambu Studio:**
   - Visit the **official Bambu Lab website** (https://www.bambulab.com/) and **download Bambu Studio** for your operating system (Windows/macOS/Linux).
   -	**Install** the software following the standard installation procedure for your operating system.
- **Launch Bambu Studio:** Open the program by clicking on the Bambu Studio icon after installation.
<br />

### Step 2: Import Your STL File

- **Open your STL file**:
  - In Bambu Studio, click on the cubic icon **“Add”** button located at the top left of the tool bar or simply drag-and-drop your .stl file into the workspace.
  - If space on the printer plate allows, you can print multiple parts simultaneously. 
- **Inspect the model:**
  - After importing, you will see your model displayed on the virtual print bed.
  - Use the mouse to rotate, zoom in/out, or pan around the model to ensure it has loaded properly.


<div align="center">
<img src="/res/Example_Bambu.jpg" alt="drawing" width="700"/>
<br />
Figure 1: Bambu Studio software layout. The screen shot shows an example of one of the H-Hope harvester parts being prepared for printing
</div>
<br />

### Step 3: Prepare the Model for Printing

Once the STL file is imported, you need to prepare it for slicing by adjusting its orientation, scale, and position.
- **Adjust orientation:**
  - Sometimes the model may import in a suboptimal orientation. To rotate the model:
    - Select the model, then use the **“rotate”** tool located in the middle of the toolbar.
    - Adjust the model's angles by clicking and dragging the rotation circles, or input precise values in the rotation boxes for each axis (X, Y, Z).
    - You can also simply use the **“auto orient”** tool or lay on face tool to place the part in the best printing configuration. 
- **Scale the model** (if needed):
  - The parts provided in H-Hope project are already scaled, thus this step is not needed. However, if the model needs to be resized for a tailored fabrication, use the **“scale”** tool also available in the left toolbar.
  - You can scale uniformly or input specific dimensions for height, width, or depth.
- **Position the model on the print bed:**
  - Ensure the model is sitting flat on the build plate.
  - Use the move tool to centre or reposition the model on the virtual print bed.
  - If multiple parts will be printed, you can automatically arrange them on the plate with the button **“Arrange all objects”**.
<br />

### Step 4: Select the Print Settings

Now that the model is properly oriented and positioned, it's time to configure the print settings for your **Bambu Lab X1 printer**.
- **Choose the printer profile:**
  - At the top-right corner of Bambu Studio, ensure that your specific model of Bambu Lab **printer and nozzle size** is selected as the active printer profile. If it is not available: Click on **“Add a new printer”** and select the Bambu Lab model from the list of available printers.
- **Select the material/filament:**
  - In the top-right section, under **Filament**, select the type of filament you're using (e.g., PLA, ABS, PETG, etc.). Bambu Lab offers its own filaments, but you can use compatible filaments by selecting the “Generic” filament or setting the appropriate settings provided by the filament vendor.
- **Configure slicing settings:**
  - On the right panel, you’ll find the following slicing settings:
    - **Layer Height:** Choose a layer height for your print. Lower layer heights (e.g., 0.1 mm) provide finer detail but take longer, while higher layer heights (e.g., 0.28 mm) print faster but may have less detail.
    - **Infill Density:** Set the infill percentage. Common values range from 10% to 20% for general prints, with higher infill offering more strength at the cost of print time and material.
    - **Shell Thickness:** Adjust the number of outer perimeters. A thicker shell adds strength.
    - **Supports:** Enable **auto supports** if your model has overhangs that need extra support during printing.
    - **Build Plate Adhesion:** You can enable a brim, raft, or skirt for better adhesion depending on the model’s footprint and material used.
The right configuration might vary for printer to printer. Typically, the default settings are suitable for the kind of parts used in the H-Hope project. You can find specific settings for PETG and PLA in the table below

<div align="center">
<img src="/res/Filaments_parameters.jpg" alt="drawing" width="700"/>
<br />
Table 1: Typical printing settings for generic filaments of PETG (left) or PLA (right).
</div>
<br />

- **Advanced Settings (optional):**
  - If you are an experienced user, you can explore the **Advanced Settings** tab to fine-tune options such as speed, temperature, retraction settings, and more.
  - You can also modify specific behaviours like bridging, cooling, and acceleration of the printer extruder.
<br />

### Step 5: Slice the Model

Once the print settings are set, the next step is to slice the model.
  - After making all your adjustments, click the **“Slice plate”** button located in the upper-right corner.
  - Bambu Studio will now generate the **G-code file** based on the slicing settings you’ve chosen.
  - After slicing is complete, the software will display relevant information as the estimated print time and filament usage.
- **Preview the sliced model:**
  - After slicing, you can use the **“preview”** tool (right vertical slide bar) to view each layer and see the print path.
  - Ensure that the supports and infill look correct, and verify that the outer shell is well defined.
<br />

### Step 6: Export the G-code for Printing

Once you are happy with the sliced model and settings, you can generate the file for the **Bambu Lab X1 printer**.
**Export the G-code as a file:**
  - In the upper-right corner, select the option and **“Export plate sliced file”** and you’ll be prompted to save the G-code file.
  - Choose a location on your computer to save the file. This file will have the extension “.gcode.3mf”
**Transfer the file to the printer:**
  - If you’re using an SD card or USB drive, copy the G-code file to the card or drive and insert it into the Bambu Lab printer.
  - If your printer is connected to the network (Wi-Fi/LAN), you can upload the G-code file directly from Bambu Studio by selecting the on **“Print plate”** or **“Send”** option instead of manually transferring the file.
<br />

### Step 7: Start the Print on Bambu Lab X1

  - Ensure that the **Bambu Lab X1** printer is properly set up, with the filament loaded and the print bed cleaned.
  - Using the touchscreen on the **Bambu Lab X1** printer, navigate to the file (either on the SD card/USB or in the printer’s internal storage if uploaded wirelessly).
  - Select the file and press **“Start”** to begin printing.
  - It is a good practice to always watch the first layer of your print to ensure proper adhesion and that the filament is extruding smoothly.
  - The **Bambu Lab X1** has built-in sensors and a camera for remote monitoring through the Bambu Handy app, allowing you to check on the print’s progress remotely.
&nbsp;

<div align="center">
<img src="/res/Bambu_screen.jpg" alt="drawing" width="700"/>
  <br />
Figure 2: Bambu Lab X1 printer display. The screen presents relevant information about the printing progress of some of H-Hope harvester parts.
</div>
&nbsp;
<div align="center">
<img src="/res/Bambu_printing.jpg" alt="drawing" width="700"/>
  <br />
Figure 3: H-Hope harvester parts are being printed on a Bambu Lab X1 Carbon printer. The internal structure of the parts is visible. Note that the parts have filament supports which must be removed afterwards.
</div>
&nbsp;
<div align="center">
<img src="/res/Printed_parts.jpg" alt="drawing" width="700"/>
  <br />
Figure 4: Resulting printed H-Hope harvester components. Here, the fitting of the induction coils and the fittings of the movable parts are shown.
   <br />
</div>

[<img src="/res/Youtube_timelapse.JPG">](https://youtu.be/j71O5QZEREo)

Video 1: Timelapse video of the H-HOPE DIY generator 3D print.

<br />

### Step 8: Post-Processing

Once the print is complete, remove the print from the bed and proceed with any necessary post-processing tasks such as:

  - Removing supports
  - Smoothing or sanding
  - Adding treads for the screws.

By following these steps, you’ll be able to efficiently import an STL file into Bambu Studio, configure your print settings, and generate the G-code needed for a successful print on your **Bambu Lab X1 printer**. 

<br />

## Importing an STL File into PrusaSlicer and Generating a 3D Print File<a name="prusa"></a> 

The **Prusa MK3** is a reliable and popular 3D printer, and in combination with the slicing software **PrusaSlicer**, constitutes a professional tool to prepare 3D models for printing. In this tutorial, we present the same previously detailed printing instructions but this time adapted for using a PRUSA printer and **PrusaSlicer**, i.e. importing the .stl file, configuring the print settings, and exporting the g-code file required for the **Prusa MK3** printer.
<br />

### What You’ll Need:

  - **PrusaSlicer:** You can download the latest version from the official PRUSA website here: www.prusa3d.com.
  - **STL files:** The 3D model files you want to print. For example, all the printable components of the H-Hope harvester below in this page. 
  - **Prusa MK3 Printer:** The 3D printer where the model will be printed.
  - **Filament:** For this project, PETG is ideal for waterproof models due to its durability and resistance to water and moisture. However, PLA or ABS can also be used for different needs, though they may compromise longevity compared to PETG.

### Step 1: Install and Open PrusaSlicer

  - **Download and install PrusaSlicer:** Visit the official PRUSA website and download the appropriate version of **PrusaSlicer** for your operating system (Windows, macOS, or Linux).
  - **Follow the standard installation procedure** for your operating system.
  - **Launch PrusaSlicer:** Open the software by clicking the **PrusaSlicer** icon after installation.
<br />

### Step 2: Import Your STL File

 - **Open your STL file:** Click on the **“Add...”** button at the top left of the toolbar or drag-and-drop your .stl file into the **PrusaSlicer** workspace. You can import multiple parts and arrange them on the print bed if space allows.
 - **Inspect the model:** After importing, the model will appear on the virtual print bed. Use your mouse to rotate, zoom in/out, or pan around the model to ensure it has loaded correctly.
<br />

### Step 3: Prepare the Model for Printing

Once the STL file is imported, you can prepare the model by adjusting its orientation, scale, and position.
  - **Adjust orientation:** If the model isn't optimally oriented, select the model and use the **“Rotate”** tool. You can manually rotate the model or input precise angles for the X, Y, and Z axes. Alternatively, use the **“Place on face”** tool to align the model for the best print orientation.
  - **Scale the model (if necessary):** In most cases, models are already correctly scaled. However, if the model needs resizing, use the **“Scale”** tool, where you can scale it uniformly or adjust specific dimensions.
  - **Position the model on the print bed:** Ensure that the model is placed flat on the build plate. Use the **“Move”** tool to centre or reposition the model. For printing multiple parts, you can use the **“Arrange”** tool to automatically place all objects on the print bed efficiently.
&nbsp;
<div align="center">
<img src="/res/Prusaslicer.jpg" alt="drawing" width="700"/>
  <br />
Figure 5: PrusaSlicer software layout. The screen shot shows the H-Hope harvester parts being prepared for printing.
</div>
<br />
  
### Step 4: Select the Print Settings

After orienting and positioning the model, you can configure the print settings for your **Prusa MK3 printer.** 
  - **Choose the printer profile:** In **PrusaSlicer,** ensure the correct printer profile is selected **(Prusa MK3 or MK3S).** If it's not available, you can add it from the printer settings.
  - **Select the material/filament:** Choose the filament type you are using (PLA, PETG, ABS, etc.) under the “Filament” section. Prusa offers its own filaments, but compatible options are also available. Ensure that the correct filament profile is selected for optimal results.
  - **Configure slicing settings:** On the right-hand panel, you will find various slicing settings:
    - **Layer Height:** A smaller layer height (e.g., 0.1 mm) will provide finer detail, while a larger one (e.g., 0.2 mm) will print faster.
    - **Infill Density:** Set the percentage of infill. For general prints, 15-20% infill is typical, but higher percentages can add more strength.
    - **Supports:** Enable supports if your model has overhangs that require additional support during printing.
    - **Brim:** Select this options for better bed adhesion depending on the model and filament.
  - **Default settings:** PrusaSlicer offers pre-configured profiles for common filaments like PLA and PETG, which are generally suitable for most projects. However, you can customise them based on your needs.
<div align="center">
<img src="/res/Prusa_materials.JPG" alt="drawing" width="1000"/>
<br />
Table 2: Typical printing settings for generic filaments of PETG (left) or PLA (right).
</div>
<br />

### Step 5: Slice the Model

Once you have finalised your print settings, you can slice the model.
  - **Slice the model:** Click the **“Slice Now”** button in the lower-right corner of the interface. PrusaSlicer will generate a G-code file based on the print settings you have configured.
  - **Preview the sliced model:** After slicing, use the preview mode to check the print path layer by layer. Ensure the supports and infill are correct, and the outer shell is well-defined.
<br />

### Step 6: Export the G-code for Printing

After confirming the sliced model and settings, the next step is to generate the G-code file for your **Prusa MK3** printer.
  - **Export the G-code:** Click the **“Export G-code”** button, and choose where to save the file on your computer. The file will have the extension .gcode, which the **Prusa MK3** will read.
  - **Transfer the G-code to the printer:** Copy the G-code file to a SD card and insert it into the printer. 
<br />

### Step 7: Start the Print on Prusa MK3

  - **Prepare the printer:** Make sure the filament is loaded, and the print bed is clean.
  - **Start the print:** On the **Prusa MK3** display menu, navigate to the G-code file on the SD card using the printer’s knob and press it on **“Print from SD card”**. Select the file and press the know to start the process.
  - **Monitor the first layer:** It's always a good practice to watch the first layer of the print to ensure proper adhesion and smooth extrusion.
&nbsp;
<div align="center">
<img src="/res/Prusa.jpg" alt="drawing" width="700"/>
  <br />
Figure 6: Harvester parts printed on a PRUSA MK3 printer.
</div>
<br />

### Step 8: Post-Processing

Once the print is complete, remove the print from the bed and proceed with any necessary post-processing tasks such as:
  - Removing supports
  - Smoothing or sanding
  - Adding treads for the screws.

## Part List for 3D Printing the H-Hope Project Energy Harvester<a name="parts"></a> 

The energy harvester developed as part of the H-Hope project comprises nine distinct printable components. Each component is meticulously designed to optimise simplicity and functionality in energy harvesting applications. The corresponding CAD (Computer-Aided Design) models for these parts are readily available in the project's data hub, which can be accessed at the following link: ***Available shortly***.
The digital model files are in the widely used ".stl" format, ensuring compatibility with various slicer software. This format facilitates straightforward importation, as detailed in the previous tutorial. By incorporating these resources into their 3D printing workflow, users can integrate the parts with other metallic components to build a working prototype of the energy harvester easily, without requiring specific technical knowledge. A detailed list of the remaining parts and the assembly procedure, which includes a video tutorial, can be found at the following link: ***Available shortly.***
&nbsp;
<div align="center">
<img src="/res/Stl_Parts_figure.jpg" alt="drawing" width="700"/>
  <br />
Figure 7: List of 3D printable component necessary to build the H-Hope harvester. (a) Bearing housing. (b) Coil holder. (c) Connection rod bearing end. (d) Connection rod end. (e) Connector cover. (f) Flywheel magnet side. (g) Flywheel without magnets. (h) Spring arm connector. (i) Spring connector. (j) H-Hope harvester assembly
</div>

&nbsp;
&nbsp;

<div align="center">
<img src="./res/H-HOPE_footer.JPG" alt="drawing" width="1472"/>
</div>

