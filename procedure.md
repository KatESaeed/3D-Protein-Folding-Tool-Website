---
layout: post
---
## Procedure
This procedure will allow you to prepare an STL file of an amino acid side chain. It does not currently include the steps to print the finished file. 
### ChemDraw:
1.	Open ChemDraw.
2.	Select File -> Open Templates -> Amino Acid Side Chains.
3.	Select the side chain of the amino acid you would like to print. They are organized in a table by their three-letter abbreviation.
4.	Under the tools bar, select Lasso.
5.	Use the lasso tool to highlight the amino acid side chain.
6.	Copy the highlighted side chain using CTRL+C or right click -> Copy. You will paste the amino acid structure directly into Chem3D.
   
### Chem3D:
7.	Open Chem3D.
8.	On the right side under “ChemDraw - LiveLink” paste the side chain using CTRL+V or right click -> Paste.
9.	In the top bar, select Calculations -> MM2 -> Minimize Energy.
10.	Select Run.
11.	Select File -> Save As.
12.	Save your file with “SYBYL2 (*.mol2)” as the file type.
    
### Chimera:
13.	Open Chimera.
14.	Select File -> Open.
15.	Select your .mol2 file.
16.	Select Select -> Chemistry -> Element -> H. (Skip if you want to show hydrogen in your model).
17.	Select Actions -> Atoms/Bonds -> Hide. (Skip if you want to show hydrogen in your model).
18.	Select Favorites -> Command Line.
19.	Copy the following into the command line located at the bottom of the app:
- represent b+s
- ~disp solvent
- setattr M ballScale 0.3
- setattr M stickScale 1.2
- bondcolor grey
- setattr p drawMode 1
20.	Select File -> Export Scene
21.	Save your file with “VMRL [.wrl, .vmrl]” as the file type.

### Blender:
22.	Open Blender.
23.	Click “x” to delete the cube that is in the file by default.
24.	In the side bar, select MolPrint.
25.	Select Open VMRL.
26.	Select your .vmrl or .wrl file.
27.	Select Open VMRL2.
28.	Input the following settings (if there are double bonds):
- double bond scale (DB scale) = 0.40
- double bonds separation (DB separ) = 1.41
29.	If there are any double bonds in the amino acid, right click where the double bond should be and select Double Bonds on the left side.
30.	On the carbon that attaches to the backbone, any attached hydrogen bonds or atoms.
31.	Select File -> Export -> Stl (.stl).
32.	Save your file.
