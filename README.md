# User Manual

# Radiant Reflow Oven

#### 08.09.

**─**

Brandon Hu CS

Micah Rice CE

Mihretab Desta EE

Rohan Mathew EE

This is a converted PDF of our User Manual, and is missing images.
Please check out the pdf in the files for full picture. :)

## Table of Contents


- Safety & Instructions
   - Instructions for Regular Use:
   - Rules & Recommendations:
- User Interface
   - Home Screen
      - Start (Bottom Right in Green)
      - Edit (Bottom Right)
      - Profile List (Bottom Right)
      - Dropdown Menu (Top Left)
   - Drop Down Menu
      - Home
      - Profile List
      - Settings
      - Server Address
   - Edit Profile Screen
      - Measured (Middle left, yellow switch)
      - Save(bottom right)
      - Cancel(bottom right)
      - Control Panels(top left)
   - Profile List Screen
      - Upload (bottom right)
      - Create New (bottom right)
      - Cancel (bottom right)
      - Load
      - Edit
      - Download
   - Settings Screen & Defaults
      - Proportional, Integral, Derivative
      - Use Cooling fan with PID
      - Look Ahead
      - Enable Preheat
      - Always hit peak
   - Network Settings
      - Server Port
      - Allow Remote Connections
      - Dark Mode
      - Primary Color
      - Secondary Color
   - Server Address Panel
- Operating Specifications
- Build Package
   - Bill of Materials
   - Resources:
      - PCB
      - R-Pi
      - Oven
      - Integration
      - Additional Design Recommendations


## Safety & Instructions

### Instructions for Regular Use:

**If the oven is OFF/Unplugged:**
Before plugging in the oven, inspect for any burningaroma or any marks on the oven. It is
important to confirm that the oven is not damagedbefore it is turned on.

```
Check Dials on the front of the oven:
○ The top dial labeled TEMP does not matter
○ The middle dial labeled FUNCTION should ALWAYS beset to Convection
○ The bottom dial labeled TIME should ALWAYS be setat STAYON
```
If the screen is OFF, **turn on the switch on the bottomright hand of the case** , on the bottom of
the white adapter.

```
The on/off Switch
```

When plugging in or switching on the oven, allow the boot process to fully complete to the point
of displaying the control panel Home Screen as shownbelow(color may differ):

```
Home Screen for Profile Control.
```
**Oven is ON:**
Confirm that the temperature inside the oven is safeto open before placing your desired PCB
with solder paste applied and components ready onthe board. After placing the PCB inside on
the metal rack in the middle of the oven, close theoven door completely.

**Confirm that the selected profile matches the neededprofile for the solder paste you are
using.**

Open the profile list as seen on the home screen inthe bottom right, or by hitting the button
displayed at the top left and selecting Profile Listfrom the drop down menu.

```
Screen displayed after navigating to the Profile List,and tapping your preferred profile
```

Load your desired profile by clicking ‘Load’ in the bottom right of the popup display.

Additional features can be explored in the SettingsMenu at this time for advanced users in
special cases. Read the Settings section of the UserManual to gain an understanding of your
options here, as well as the default settings.

Hit Start at the bottom right to **begin the profile.**

While the oven is on, the user and anyone else inclose contact with the oven **must** be aware of
the temperature inside the oven based on what is shownon the display screen. While the reflow
profile is running be sure to keep an eye on the trendof the measured profile and that it is
following the desired profile appropriately. Oncethe notification to open the oven door appears
along with a beeping sound, the user **must** grab onlythe oven handle and open it to the first or
second notch. **DO NOT** touch any other part of the ovenbecause it could be extremely hot and
may very likely burn your skin on prolonged contact.While the oven doors are open, be sure to
maintain a foot or two distance from the oven untilthe cooling phase is done.

**The cooling phase** continues from the user prompt toopen the door until the temperature
reaches 30 C. Depending on your equipment, you maychoose to remove the PCB prior to
reaching 30 C, but beware of burns. It is recommendedto use tongs to remove the PCB if done
before 30 C and allow it to cool to room temperatureon a safe surface such as the foil covered
open door of the oven, which should cool much fasterthan the rest of the oven if opened to
100%.
Note that this product was designed and tested tobe a reflow oven. Do not put any other items
other than a circuit board with the appropriate componentson the oven tray. This product is a
tool and not a toy, and is not for food. Always beaware of what is around the reflow oven. Make
sure the area is clean and free of anything whichreacts negatively to heat.


### Rules & Recommendations:

#### ● DO NOT change the PID settings unless you know exactlywhat you are

#### doing. Default PID: P = 300, I = 0.075, D = 1360

#### ● When prompted by the oven during cooling, open thedoor to the first or

#### second notch, which is 10-25% open. It is not recommendedto immediately

#### open the door 100%.

#### ● Do Not leave cooling oven unattended with door open

#### ● Do Not leave any items on top of the oven at any time.

#### ● Do Not Touch the oven flat surfaces during heatingor cooling. Surfaces will

#### be very HOT!

#### ● Do Not attempt to run/program heat profiles above300 C

#### ● Ensure the materials you are using can survive theTemperature Profile

#### selected.

#### ● Make sure your Temp Profile matches your solder Paste

#### ○ The Oven has default profiles for the following compounds,shown

#### below accessible in the Profile List:

#### ■ Sn96.5Ag3Cu.

#### ■ Sn42Bi57.6Ag0.

#### ■ Sn63Pb

#### ■ Sn42Bi57Ag

#### ■ STMaxLeadFree(an example custom profile)

#### ○ Caution : Program new profiles for other compoundsusing diligent

#### research and at your own risk. Our oven is not capableof achieving

#### slopes higher than 2.17 degrees C/s. Program higherslopes at

#### your own peril.


#### ● IN CASE OF FIRE or Damage to parts, IMMEDIATELY press the

#### STOP button on the touchpad control screen located at the TOP RIGHT or

#### the BOTTOM RIGHT of the display. Wait for parts tocool before removal.

#### The internal temperature of the oven can be read atthe TOP LEFT of the

#### home control screen.

#### ○ STOP buttons appear while the profile is actuallyrunning. If you do

#### not see a STOP button in these locations, the profileis not active, but

#### THE OVEN MAY STILL BE HOT.

```
STOP located in top and bottom right locations & temperaturereading at top left.
```
**TIP:** For **Settings panels** , remember to **always hit theSave button** on all settings screens
once you have input your new preferred values.


## User Interface

### Home Screen

#### Start (Bottom Right in Green)

This green button starts the profile that is currentlyloaded.

#### Edit (Bottom Right)

This button opens the Profile editor screen.

#### Profile List (Bottom Right)

This button opens the Profile List, to select anotherSolder Paste Profile.

#### Dropdown Menu (Top Left)

This button opens the dropdown menu, which containsaccess to the Home page, the Profile
List, the Settings for PID, Hardware, Network, andAppearance, and the Server Address display.

```
The STOP buttons are located in the bottom right &top right of an active profile on the Home
Screen.
```
The current temperature in the oven is in the topleft, to the right of the drop down menu and
home button.


### Drop Down Menu

#### Home

This button brings you to the Home screen, which iswhere you Load and Start a profile.

#### Profile List

This button opens the Profile List, to select anotherSolder Paste Profile.

#### Settings

This button opens all adjustable settings for thedisplay screen. Here the user can customize the
profile line color as well as the actual temperaturecurve that represents the temperature inside
the oven at that time.

#### Server Address

This button will display a popup showing the currentserver address of the oven. The default
server address of our particular installation is **10.156.28.**


### Edit Profile Screen

#### Measured (Middle left, yellow switch)

This will show up if you are editing a profile youhave just run. It allows you to edit the profile
with knowledge of how the existing profile actuallyperformed due to oven characteristics.

#### Save(bottom right)

Save will save the profile as it currently existsin the editor. If a profile already exists named
exactly the same thing, a (1) will be appended.

#### Cancel(bottom right)

This button will cancel the editing process and notsave the current profile’s edited version.

#### Control Panels(top left)

The ordered pair at the top shows the current locationof the point that is selected. The arrows
below will move that point by one unit in the prescribeddirection.
The number of nodes available can be adjusted usingthe - or + in the next panel below.
The Max Time - or + will move the x axis max valuebetween 300 up to a max of 20000.


### Profile List Screen

This screen is a list of all currently programmedprofiles. There are 5 default profiles. 4 are for
different Solder paste compounds, and one is an exampleof a custom profile. You may create
your own profiles and save it to run it.

#### Upload (bottom right)

If you have a .json profile already stored locally,you can upload it by pressing this button and
selecting the .json profile.

#### Create New (bottom right)

This will open the editor to create a new profilefrom scratch.

#### Cancel (bottom right)

Brings you back to the home screen.

**When you click on a profile,** a popup will appear showingthe profile you selected.

#### Load

This will open the home screen with this profile loadedand ready to start.


#### Edit

This will open the profile editor with this profileloaded and ready to edit.

#### Download

This will download a .json file locally. Useful ifyou have nearly 50 profiles stored. The maximum
number of profiles the controller will store is 50,after which it begins deleting non default profiles
to store additional ones.

### Settings Screen & Defaults

The Settings screen gives you access to settings andinformation for 4 different categories. PID
controller, Hardware(GPIO ports, Temperature Readings,preheat control/profile behavior
control), Network(default Port for Web UI connections),and Appearance(Colors, dark mode).

#### Proportional, Integral, Derivative

One of the most important settings on the Reflow Oven.These constants control the weighting
of the PID algorithm and are tested to specificallyfollow precisely the temperature profile. In
most cases, altering these values is NOT RECOMMENDED.If you have trouble following a
profile, first investigate whether the slope is toosteep for the oven(in our case above 2.
degrees C per second), or the cooling is too steep(fasterthan 0.5-1 degree per second).
**Default Values: Proportional = 300, Integral = 0.075,Derivative = 1360**


#### Use Cooling fan with PID

This setting is only useful if you have installed a cooling fan. No fan is currently installed in our
build.

#### Look Ahead

**Default value: 5 seconds.** This causes the profilePID controller to look ahead X amount of
seconds in the profile and target that value. Thisis useful because the thermal inertia of the
oven may cause a delay in responding to inputs.

#### Enable Preheat

This setting allows the oven to preheat to the temperatureprescribed in the profile adjusted by
the look ahead value. This is highly useful for **profilesthat start at above room temperature**!
Based on the initial slope of a profile that beginsafter preheat, you may wish to adjust the %
power delivered during preheat to adjust the thermalinertia at the moment of beginning the
profile.
**Default values: Preheat= ON Power = 70%**

#### Always hit peak

This setting ensures that even in the case where theslope is not being matched perfectly or the
actual temperature curve is delayed behind the profileprescription, the oven will still ensure it
hits the max temperature prescribed and holds forthe amount of time the profile indicates from
the intended initial point of temperature peak. Thissetting is largely irrelevant unless the profile
has sections with unachievable slopes. For our oven,any slope **above2.17** °C **per second** is
**not achievable.
Default value: ON**

### Network Settings

#### Server Port

This setting defines what port the UI will be hostedon. Please ensure that the port is not taken
by a different application.
**Default value: 3001**


#### Allow Remote Connections

Allows connections to the WebUI to allow for monitoringand control of the oven from a different
computer within the same network. These connectionswould occur by navigating to the IP
address dictated in the Server Address panel, withthe :PortNumber added on which is dictated
here. For our implementation of the oven for example,this is found at **10.156.28.232:**

#### Dark Mode

Dark mode switch, turns on and off a darker vs lighterUI background.

#### Primary Color

The profile line color and UI highlight color aredetermined by this value.

#### Secondary Color

The actual temperature curve experienced is trackedin this color value.

### Server Address Panel

The IP address displayed allows you to access theweb UI interface from a remote computer in
the same network, so long as “allow remote connections”is ON in the Network panel of the
Settings Screen.


## Operating Specifications

```
Characteristic Value
```
```
Max Recommended Operating Temp 300 C
```
```
Max Temperature Ramp Slope 2.17 °C /s
```
```
Max Profile Duration 20,000 seconds (5.56 hours)
```
```
Max Cooling (Closed Door) (300-200)^1 °C /s
```
```
Max Cooling (Closed Door) (200-30) 0.5 °C /s
```
```
Max Cooling (Open Door) (200-30) Determined by PCB thermodynamic
characteristics. I.e surface area, materials.
The air in the oven itself will cool rapidly
toward 100 degrees, then 1 °C /s.
```
```
Max Number of Thermo Profiles^50
```
```
Default PID Settings: P = 300, I = 0.075, D = 1360
```
```
Default Temp offsets: -8 °C and +8.5%
```
```
GPIO PORT Defaults: Relay: GPIO 4 (Pin 7)
Convection Fan: GPIO 22 (Pin 15)
Buzzer: GPIO 24 (Pin 18)
```
```
Default Network Port^3001
```
```
IP address
specific to OUR implemented Oven:
```
##### 10.156.28.

```
To access WebUI from PC,
go to YourIP:YourPort
For us, that is:
10.156.28.232:
```

## Build Package

### Bill of Materials

### Resources:

#### PCB

```
● https://github.com/bhu413/reflow/blob/main/FinalReflowOvenController.zip
● We recommend using JLCPCB (jlcpcb.com) for printingthe circuit board whose
gerber files are enclosed in the above link
● For editing the design files, we recommend using AltiumDesigner
```
#### R-Pi

```
● https://github.com/bhu413/reflow
● Issues:https://github.com/bhu413/reflow/issues/new
● You may want to comment out a line in the startup.shwhich inverts the screen, if it
does not fit your use case. At the moment of thiswriting the script calls this
command on line 10 of startup.sh
```
#### Oven

```
● If you wish to achieve 3 degrees C/s ramp speed, werecommend altering the oven
with an additional heating rod. Without insulationthe oven listed in our Bill of
Materials is capable of 1.2 degrees C per second.With insulation, we have 2.
degrees C per second curve.
```

#### Integration

```
● Tools needed
○ Drill
○ Screw driver
○ Metal knockout punch
○ Wire crimpers
○ Hot glue
○ Heat gun
○ Soldering paste and soldering iron
● Overview steps
○ Open the oven top and side covers and connect theSSRs to the oven and the
convection fan. Assemble the PCB.
○ Insulate the oven and put the oven covers back onwith the thermocouple
going into the inside of the oven.
○ Put the SSRs, raspberry pi, PCB, outlet extender,and the fan inside the case
and secure them in place with screws or hot glue.
```
#### Additional Design Recommendations

```
● Perhaps an extra heating rod to achieve a max slopeof 3 degrees Celsius per
second
● Perhaps replace fan with extra powerful fan for additionalconvection and additional
cooling control
● Perhaps add a servo motor to control the door to automaticallyopen for cooling
Software and PCB already support two more additionalcontrolled outputs, using
the RED design which is currently unused.
```

