# :waning_crescent_moon: What is Blue Light Blocker 
This applet is the Linux Mint equivalent of '**Night Light**' (on Windows), and '**Night Shift**' (on macOS).

<img alt="Night Light in Windows" src="https://github.com/user-attachments/assets/bc55a22c-b986-496c-b77e-b9e718308fd2" width="250" height="250">
<img alt="Night Shift in MacOS" src="https://github.com/user-attachments/assets/2d0a4e9c-1c55-476e-b2b4-29f133f49c56" width="500" height="250">

It acts as a blue light filter and makes your display use warmer colors, according to your likings. This applet, **Blue Light Blocker**, also allows you to control the brightness of your screen at will. 

# :sunglasses: YOU are in control!
Some applets are time-based, meaning they only block blue light at certain times of the day. The user has no control over the blue light filtering.

With Blue Light Blocker, however, you are in total control!

Is it still day time? Is it night time? Who cares! Don't let the clock dictate when your screen has to block blue light from entering your precious little eyes! 👁️ 👄 👁️

You want to block blue light *all day*? You got it!

You want to block blue light *only at night*? It's your call, boss!

You want to block blue light *only when you feel like it*? No problemo! 

You can enable and disable this applet anytime in merely 2 clicks! 
Adjusting the warmth tone of your screen or it's brightness has never been easier, thanks to simple sliders with real-time feedback!

What a time to be alive :relieved: :sparkles:

# :battery: Batteries Included!
This version of Blue Light Blocker comes with everything it needs right out of the box!

You won't need to install additionnal packages (*unless you perform an [automatic installation](#-automatic-installation)) or enter commands in your terminal!

# 💻 Manual Installation
- Download the github repository as a ZIP file

- Extract the ZIP file

- Place the `Blue-light-blocker@samuel12sam` folder inside `/home/[your_name]/.local/share/cinnamon/applets/`
  
    > If you do not see `.local`, make sure you have enabled **'Show Hidden Files'** by going into the **'View'** tab of your File Explorer and ticking the option or by using the **CTRL+H** keyboard shortcut.

- Open the 'Applets' window, through the 'System Settings' or by right-clicking on any panel and clicking on 'Applets'.

    <img alt="Applets window" src="https://github.com/user-attachments/assets/af491c83-8ed9-4e2f-ac0d-0bf08e01a0fc" width="400" height="316">

- Select Blue Light Blocker by clicking on it, press the '+' sign at the bottom of the window to add Blue Light Blocker to your panel.

    <img alt="Button to click in order to add the applet to the panel" src="https://github.com/user-attachments/assets/e85972c0-d480-4e68-a64e-5979b4f031b1" width="400" height="316">

# :construction_worker: Usage
Click on the Blue Light Blocker Applet in the panel and use the sliders to modify the color temperature of your screen or its brightness.

 <img alt="Using Blue Light Blocker" src="https://github.com/user-attachments/assets/5300ee3f-28e9-4ad9-8547-edab8240591a" width="381" height="220">

# :wrench: Configuration

Right click on the Blue Light Blocker applet in your panel and click on 'Configure...'

<img alt="Opening the configuration window" src="https://github.com/user-attachments/assets/2c608c1c-71c6-41be-b5b3-8f21b34f9b95" width="253" height="167">
<img alt="Configuration window" src="https://github.com/user-attachments/assets/8d66fc1e-1d92-4d39-aa8a-03af1d648ab8" width="300" height="250">

# 🚮 Uninstalling Blue Light Blocker

- Make sure to first remove the applet from your panel by pressing the '-' button.

 <img alt="Uninstalling Blue Light Blocker" src="https://github.com/user-attachments/assets/a81dc679-0331-4eba-a10a-6de0c1ea7ffb" width="469" height="392">

- Then uninstall it by pressing the trashcan button from the same window

<img alt="Uninstalling Blue Light Blocker" src="https://github.com/user-attachments/assets/ae47e9b6-9543-4b31-9465-c2a6717fd149" width="469" height="358">



# 🚧 Possible Future Features
- Allow the user to use a custom icon/image for the applet in the panel
- Allow the user to display a custom format for the color temperature in brightness info in the panel
- Translations for other languages

# ⚡ Automatic Installation
Please note that users who install Blue Light Blocker from the 'Download' tab in the 'Applet' window on Linux Mint will be prompted to install the `xsct` package, as opposed to users who [manually install it](#-manual-installation).

That is because Cinnamon does not allow developpers to publish their applets with pre-compiled code and compiling the code automatically after the applet gets downloaded from the 'Download' tab
would require users to have 2 libraries/packages installed on their computer that most people don't have by default (`libx11-dev` and `libxrandr-dev`). 

### What's `xsct` and why is it required?
`xsct` is a public domain (open-source, but better) UNIX tool that allows you to change the color temperature of your screen. However, it only functions via terminal commands, which is a total pain in the butt to use if you
frequently change the color temperature of your screen. 

Blue Light Blocker uses this UNIX tool at its core and provides a user-friendly interface to let the user block the blue light from their screen
using precise sliders while also adding a layer of security by making it impossible for the user to set the brightness of their screens to 0, which is possible with `xsct` via the terminal commands. 
Blue Light Blocker also adds a lot of Quality of Life features that simply don't exist with the `xsct` package alone. 

In short, Blue Light Blocker reduces the amount of tinkering necessary to change the brightness or the color temperature of your screen while also offering a simple yet very nice user experience.

For more information about `xsct` : https://github.com/faf0/sct


