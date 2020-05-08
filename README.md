Network Assessor for Skype for Business Online and Microsoft Teams
==================================================================

            

This is a free tool that functions as a frontend for [Microsoft's Network Assessment Command Line Tool](https://www.microsoft.com/en-us/download/details.aspx?id=53885):


![Image](https://github.com/jamescussen/network-assessor-for-skype-for-business-online-and-microsoft-teams/raw/master/networkassessor1.00-screenshot-sm.png)


**Version 1.00 Features**


  *  Graphs Packet Loss, Average Jitter, Latency and Reorder Ratio. 
  *  Zoom graphs in / out / forwards / backwards to view the data clearly. 
  *  Start / Stop and Pause the network tests at the click of a button. 
  *  Keep an eye on the status of testing using the tray icon colour by setting breach percentage thresholds. This will easily let you know that things are within your desired operating levels without having to open the interface. There are two levels of threshold
 breaches: one that changes the icon to orange in colour and the other that changes the icon to red in colour. These percentages are calculated on a per graph basis and if any graph breaches the percentage the colour will change.

  *  Graphs will automatically highlight in red points in each of the graphs which are outside of Microsoft’s recommended bounds of operation. There are two levels for these thresholds: Client thresholds and Edge Thresholds. For more details see the blog
 post link below. 
  *  You can select the frequency at which the tool will run tests. This ranges between 1 and 120 minutes (ie. Run a 17 second long test every 1 minute or up to every 2 hours).

  *  The status bar will display PASS/FAIL results for each graph. This calculation follows Microsoft's 'ResultsAnalyzer.exe' PASS/FAIL calculation which is based on any graph having more than 10% of test attempts resulting in (Client or Edge) threshold breaches
 will equal a FAIL result. 
  *  Allows for graphs to be saved as PNG images for use in documentation/reports.

  *  All the graphs can be shown at once or individual graphs can be selected using the “Window” menu item. Graphs are saved at the resolution that they are displayed, so opening individual graphs and then saving them can offer higher resolutions.

  *  Every session that is created by the tool gets recorded in a CSV file for future reference. Sessions will “roll” to a new file based on the “Roll Time (hours)” setting in the Settings dialog. Logs can be rolled between 1 and 12 hours.

  *  CSV files can be imported back in to the tool by using the File > Import CSV File menu or dragging and dropping the file onto the interface directly from Windows Explorer.

  *  Supports automatic download (note: Internet connection is required for this to work) and installation of the Microsoft Network Assessment Tool and VC++ Redistributable pre-requisite by using the Help > Install Microsoft Tool menu item.


 


**Version 1.10 Features**


 


  *  Works with Microsoft tool version 1.1.0.0 released on 5/3/2018 
  *  Support Connectivity Check. Select 'File > Connectivity Check' 
  *  Supports new Microsoft tool installation procedure 
  *  The Microsoft Tool in its latest incarnation doesn’t handle all exceptions that it throws. These seem to be mostly around when it does the initial lookup REST call where it gets a JSON list of the servers to connect to for testing. If DNS fails or
 there is no network interface available on the machine the Microsoft tool throws an unhandled exception. If this happens the Network Assessor GUI will report an error and stop running tests. 

  *  Be careful when trying to manually install the new 5/3/2018 version of the Microsoft Command Line tool because it does not install properly over the top of previous version (i.e. it doesn't install over it and still says that installation was successful).


 


**Note:** This tool is not intended for load/stress testing!


 


**For more details see: [http://www.myteamslab.com/2017/08/network-assessor-for-skype-for-business.html](http://www.myteamslab.com/2017/08/network-assessor-for-skype-for-business.html)**


 





        
    
