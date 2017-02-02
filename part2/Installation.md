# Installation

All the scripts and expert advisers I will share at [LetMeBeFree.com](/letmebefree.com) run under Metatrader 4 on a Windows platform \(should also work on Metatrader 5, but not tested\). In most cases, I will only provide the compiled version, meaning you will not be able to see the code used to perform the task. However, this does not stop you using them.

To install a script or expert adviser, you will need to copy the EX4 file into the relevant sub-directory of your Metatrader 4 installation.

Scripts that run once, but do not remain on your chart must go into a sub-directory called "Scripts". Expert Advisers \(such as Zone-Trader Tutor\) that remain on your chart to repeatedly do something must go in a sub-directory called "Experts".

To ensure you have the correct directory, do the following:

1\) With your Metatrader 4 trading platform open, select the "File" menu and then "Open Data Folder". This opens a standard windows explorer window for navigating around the file system.

2\) Navigate into the "MQL4" folder by double clicking on it in the explorer window.

3\) To install an expert advisor such as Zone-Trader tutor, double click \(or right click and select "Open"\) on the folder called "Experts" This will open the folder where you must then copy the expert adviser file that I provide \(if you are installing a script, double click on the "Scripts" folder and copy the file into here instead\).

4\) Close and restart your Metatrader terminal.

5\) Run the script or expert adviser by using your mouse to drag it from the navigator window onto the relevant chart.

6\) It the script or EA requires any parameters, a box will pop up where you can enter these before clicking on "OK". For example, Zone-Trader tutor requires that a username and license key are entered in order for it to work.

_**Important**_

In order for the EA to work correctly, you must have your Metatrader EA settings \(Tools-&gt;Preferences\) something like below. In particular, the check box for "Allow DLL imports \(potentially dangerous, enable only for trusted applications\)". DLL imports are used for user authentication and obtaining time zone information.

![](/assets/import.png)



