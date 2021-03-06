# Windows 10 Optimization
A guide on how to get more out of Windows 10. Mainly for me to use when setting up new win10 computers. All links at bottom

**NOT RECCOMENDED FOR LAPTOPS**

# DISCLAIMER
Results cannot be guarunteed. Proceed with caution. Always have a restore point in case things go wrong. I am not responsible for any damage caused to your system or files.

# What to expect
* 30-40 Windows Processes 
*  1-2% CPU Usage (Tested on i5-8250u)
* More stable FPS, lower input lag 
* Less tracking (Linux is still WAY better with this)
* Lower input lag in games (Not super noticeable, no false promises. Maybe I'm just not good enough lolol)

# Drivers
* Use NVCleanstall. Click recommended features, and install. 
* AMD Users are chilling
* Try to use drivers from manufacturer website as much as possible. If not there, use Snappy Driver Installer Origin (SDIO). 

# Windows Options
Most options will be changed by Chris Titus's script. Make sure hardware accelerated GPU scheduling is enabled if you have the option.

# Chris Titus Tech Debloat Script
* Put this in powershell (admin)  ` iwr -useb https://git.io/JJ8R4 | iex `
* Apply essential tweaks and security updates only
* Restart PC

# Sycnex/Windows10Debloater 
* Put this in powershell (admin) ` iwr -useb https://git.io/debloat|iex `
* Click remove all bloatware, disable telemetry/tasks, and remove bloatware regkeys.
 
 # Timer Resolution Service
* In most cases, this has improved my fps. Tested on desktop and gaming laptop
* Just follow read me in folder

# Device Manager Optimization (disable)
* Display adapters:
  * Intel graphics (if you don’t use it, ideally should be disabled in the BIOS)
* Network adapters:
    * All WAN miniports
    * Microsoft ISATAP Adapter
*	Storage controllers:
    * Microsoft iSCSI Initiator
*	System devices:
    * Composite Bus Enumerator
    * Intel Management Engine / AMD PSP
    * Intel SPI (flash) Controller
    * Microsoft GS Wavetable Synth
     * Microsoft Virtual Drive Enumerator (if not using virtual drives)
    * NDIS Virtual Network Adapter Enumerator
    * Remote Desktop Device Redirector Bus
    * SMBus
    * System speaker
    * Terminal Server Mouse/Keyboard drivers
    * UMBus
# Disable Antivirus
* It's in the name. Not necessary
# BCDEdit and system timers
Put these commands in a cmd (admin) window.

`bcdedit /set disabledynamictick yes`

`bcdedit /set useplatformtick yes`

# Power Plan
Paste in a cmd (admin)

`powercfg -duplicatescheme e9a42b02-d5df-448d-aa00-03f14749eb61`

Honestly use whatever power plan you want

# Memory Cleaners
I don't use one on my desktop, because I have 16gb of ram. The only one I know of is ISLC, and it seems to be disliked by the tweaking community.

On my laptop, I use ISLC because I only have 8gb ram. I followed this guide https://www.youtube.com/watch?v=cP1EMzGD9Xc

# What to avoid
* Avoid game boosters like Razer Cortex or Smart Game Booster. They only cause problems (for me). If your PC is that bad, just lower the resolution.
* I would really only recommend following Calypto or Fr33thy's guides on windows 10 optimizations. A custom ISO will beat every optimization done to stock windows.

# Custom ISO's
* If you thought this was too much work, here are 2 very nice custom iso's that get all the work done for you. GG has better performance, but I prefer Revi because I play Phasmophobia sometimes 
  * GGOS - https://discord.gg/ggos
  * ReviOS - https://www.revi.cc/ or https://discord.com/invite/962y4pU

# Credit
These were just a bunch of guides I found online slapped into one. I only put the things that actually seemed to increase my fps. I will link everything I have mentioned here.
* Calypto's Latency Guide: https://www.calypto.us
* Chris Titus Tech: https://www.youtube.com/c/ChrisTitusTech
* Debloat Script: https://github.com/Sycnex
* Glen Delahoy - SDIO https://www.snappy-driver-installer.org/
* TechPowerUp: NVCleanstall https://www.techpowerup.com/nvcleanstall/
