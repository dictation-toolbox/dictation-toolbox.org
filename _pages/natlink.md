---
layout: page
title: Natlink
---

- [Qh.antenna.nl - Natlink, Unimacro and Vocola ](http://qh.antenna.nl/unimacro/index.html) - (Recommended) Documentation and install instructions

# Troubleshooting

-  When starting Dragon with NatLink `Cannot load compatibility module support 
    (GUID = {dd990001-bb89-1d2-b031-0060088dc929})`
  1. Install [Microsoft Visual C++ 2010 Service Pack 1 x86](https://www.microsoft.com/en-us/download/details.aspx?id=26999)
  2.  Reboot PC
  3.  Register regsvr32 manually on the natlink.pyd from an admin command prompt.  Detailed information on [Natlink\'s Troubleshooting Page](https://qh.antenna.nl/unimacro/installation/problemswithinstallation.html). 

- Running "Configure NatLink via GUI" does not bring up the settings window - try running the program as an administrator:
  1. Open an administrator command prompt by searching for "cmd" in start and either right click, run as administrator or ctrl-shift-enter.
  2. Change directory to the folder where start_configurenatlink.py was installed. This is likely to be `C:\NatLink\NatLink\confignatlinkvocolaunimacro` so the command would be `cd C:\NatLink\NatLink\confignatlinkvocolaunimacro`.
  3. Run `python start_configurenatlink.py`.
- To fix `ImportError: No module named win32con`
  Package win32con is out of date or not installed. Try `pip install pywin32`  Alternatively if the error persists use the [Windows installer](https://sourceforge.net/projects/pywin32/files/pywin32/Build%20221/pywin32-221.win32-py2.7.exe/download)
- To fix `lost sys.stderr`
  For Caster must use pywin32 for `system wide` features, such as registering COM objects or implementing Windows Services, then you **must** run the following command from an elevated command prompt: `python C:\Python27\Scripts\pywin32_postinstall.py -install`

- To fix `ImportError: cannot import name RuleWrap`
  You likely either have the wrong version of Dragonfly installed, or don't have it installed at all.  RuleWrap is a Dragonfly import. Try `pip uninstall dragonfly` (it\'s okay if it doesn\'t find the package) then `pip install dragonfly2`.

- To fix `ImportError: DLL load failed: %1 is not a valid Win32 application.` You're most likely using the 64-bit version of Python or 64-bit Python library.
  1. Uninstall Python 64-bit and delete `C:\Python27` to remove any extraneous libraries. 
  2. Then install or reinstall [Python v2.7.X  32-bit](https://www.python.org/ftp/python/2.7.15/python-2.7.15.msi) 

- To fix `UnicodeDecodeError: 'ascii' codec can't decode byte 0x83 in position 52: ordinal not in range(128)`when trying to use `words.txt`. 

  Dragonfly out of date **or** you\'re using the old `dragonfly` not `dragonfly2` package. Run the following in command prompt one at a time.
    1. `pip uninstall dragonfly` to check and remove the old dragonfly package.
    2. `pip install dragonfly2` or `pip install --upgrade dragonfly2` to install or update Dragonfly

**As Needed**

- [Register Natlink pyd Manually](https://www.youtube.com/watch?v=_WnMGOfHYuM)
- [Microsoft Visual C++ 2010 Service Pack 1 Redistributable Package MFC Security Update](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=1&cad=rja&uact=8&ved=2ahUKEwi874yllILeAhWKxYMKHYgrDF8QFjAAegQICRAB&url=https%3A%2F%2Fwww.microsoft.com%2Fen-us%2Fdownload%2Fdetails.aspx%3Fid%3D26999&usg=AOvVaw0cUChp6Ql2-eV0zUE9XCaC)
- [Qh.antenna.nl - Implementation_and_Acceptance_of Natlink.pdf](https://web.archive.org/web/20160711183956/https://qh.antenna.nl/unimacro/implementation_and_acceptance_of_natlink.pdf)

# Legacy
- [NatLink For Python 2.5](http://www.westga.edu/~drocco/voice/NatLink/)