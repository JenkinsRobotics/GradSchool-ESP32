## Jenkins Robotics
# Jenkins CNC

<!-- This is commented out. -->

## Project Information

Project Status : <mark style="background-color: green"> &nbsp; COMPLETED &nbsp;</mark>  
Code Status : <mark style="background-color: green"> &nbsp; GOOD &nbsp;</mark>  
Development Status : <mark style="background-color: red"> &nbsp; NOT ACTIVE &nbsp;</mark>  



&nbsp;
## General Information


 This is the project files for our Shapeoko 3 xxl. Our goal is to make our shapeoko 3 as automated as possible. To achive this goal we have installed multiple upgrades onto our cnc including: 
- [x] Automated Tool Change
- [x] Manual Tool Change
- [x] Coolent 
- [x] Tool Z Probe Macro
- [x] Work Piece XYZ Probe
- [x] Spindle Control
- [x] Modularity

&nbsp;
## WATCH NOW ON YOUTUBE


 Watch the project playlist on youtube. 

 &nbsp;

[![image alt text](http://img.youtube.com/vi/w-qWbZ5-IQw/0.jpg)](https://youtube.com/playlist?list=PLNTKXZ4hgP_jekZOWw05JcJtyseCdSsIV "YouTube")

&nbsp;
## Support

Did this project help you? Consider supporting! 

Consider Subscribing: https://bit.ly/2DgZyuq <br>
Patreon ➔ https://www.patreon.com/JenkinsRobotics <br>
Venmo ➔ https://venmo.com/u/JenkinsRobotics <br>



&nbsp;
## Table of Contents


**[Project File Structure](#project-file-structure)**<br>
**[Installation Instructions](#installation-instructions)**<br>
**[Next Steps](#next-steps)**<br>
**[Components](#components)**<br>
**[Notes and Miscellaneous](#notes-and-miscellaneous)**<br>
**[Links](#links)**<br>


&nbsp;
## Project File Structure

The following is a breakdown of the different folders and the files contained in them:

1. **FUSION 360 POST PROCESSOR**
    - *JenkinsCNCReprap.cps*
    A post processor is the link between the CAM system and your CNC machine. The Post Processor translated the CAM instruction including information like the toolpath data, the type of operation, and the desired spindle feeds/speeds into the language that a CNC machine understands (gcode). Despite the fact that the DUET 3 runs RepRap Firmware, the standard RepRap post processor do not work for CNC machining. Our Custom post processor is based on the default RepRap post processor but fixes the gcode syntax errors and adds many additional modular features. 
    **Directions:**
      - Uploading file to Fusion 360 Cloud Storage [Personal-cloud]
        With-in Fusion 360 open the project navigation panel. Under Libraries select "Assets", then select folder "CAMPosts" (if no folder exist then create one.) Upload the custom Post Processor within this folder for cloud storage. 
      - Create NC Program
        After creating your CAD model select the "Manufacturing Tab" in Fusion 360. Complete the "Setup" process and the desired toolpaths. Create a new "NC Program".  Under "Post Configuration / Library" specify the location of the Post Processor File [personal-cloud recommended]. Under Post specify the desired file "Jenkins CNC RepRap". Adjust Post Properties if desired, then export gcode.  


    
    &nbsp;
2. **GCODE**  
   - *SDCARD*
    This folder contains a copy of all they files located on our Duet 3 Motherboard SD Card. The system drive contains multiple subfolders each containing different gcode / system files. Before Copying/referencing our  custom files it is best to upgrade the stock firmware and system files. The official Duet 3 releases can be found on GitHub.  [RepRap Files](https://github.com/Duet3D "Duet3D").
      
   - *Macros*
    The Macro folder contains all the additional system files needed for the Duet 3. Files are grouped by their function. 
     **Directions:**
        - Upload any of the desired files. Then review the files and make any necessary  adjustment to the position points and the probe/sensors numbers.  

   - *Sys*
    The System folder contains all the important system files needed for the Duet 3. Each file serves as important gcode files that configures the machine and provide necessary gcode for specific processes like tool changes. 
        **Directions:**
        - For AutoTool Change Upload the following files:  TFree, Tpost, Tpre, ToolZProbe        
        - For manual tool Change Upload the following files:  manualtoolchange, ToolZProbe,



    &nbsp;
3. **GH Pages**
    - Files used for Github Pages and readme text file. 


  

    &nbsp;
4. **MANUALS**
   - *Post Processor Training Guide*
     - The reference file for fusion 360 post proccessor. Contains reference material for different hadware apart of the CNC. 
    
  
      


> Note: Updating the RepRap firmware should be done carefully. Uploading the updated ZIP file could erase custom gcode files. 


&nbsp;
## Installation Instructions

Installation instructions can be found in the youtube video linked below 
 

 ### Video link  be updated soon

[![image alt text](http://img.youtube.com/vi/w-qWbZ5-IQw/0.jpg)](https://youtube.com/playlist?list=PLNTKXZ4hgP_jekZOWw05JcJtyseCdSsIV "YouTube")


<!-- This is commented out.  

The following is a breakdown of the different folders and the files contained in them:


```
cd utils
node build.js
```


Create a file with a `.zip` extension containing these files and directories:

```
manifest.json
common/
chrome/
```


Create a file with a `.xpi` extension containing these files and directories:

```
chrome.manifest
install.rdf
common/
firefox/
```

 This is commented out. -->


&nbsp;
## Next Steps

This project is now completed. No next steps are planned. We can release bug fixes if found. 

If you require assistant join our discord channel linked down below.



&nbsp;
## Components 

The following is a breakdown of key components for this project:
&nbsp;
| Item          | Function      | Cost  |
| ------------- |:-------------:| -----:|
| Fusion 360    | CAD           | Free |
| VS Code       | Text Editor   |   Free |


&nbsp;
## Notes and Miscellaneous


Disclaimer :
Modifying your Shapeoko  will void the warranty. Do at your own risk.

**ENJOY!!**

That’s  all Folks. Hope this can help you in some way.
... Consider Supporting Us Down Below. 

&nbsp;
## Links


SUPPORT US ► 

Consider Subscribing: https://bit.ly/2DgZyuq <br>
Patreon ➔ https://www.patreon.com/JenkinsRobotics  <br>
Venmo ➔ https://venmo.com/u/JenkinsRobotics <br>


FOLLOW US ►

Discord ➔ https://discord.gg/sAnE5pRVyT <br>
Patreon ➔ https://www.patreon.com/JenkinsRobotics <br>
Twitter ➔ https://twitter.com/j <br>
Instagram  ➔ https://www.instagram.com/jenkinsrobotics/ <br>
Facebook ➔ https://www.facebook.com/jenkinsrobotics/  <br>
GitHub  ➔ https://jenkinsrobotics.github.io <br>











