---?image=assets/images/gitpitch-audience.jpg
@title[Platform Build Win Emulator Lab]
<br>
<!---  Uncomment once gitPitch is done
<span style="font-size:0.75em" >This slide deck has moved to:  https://gitpitch.com/tianocore-training/EDK_II_CI_Unit_Test_Framework/master#/</span>
-->
<br><br>
## <span class="gold"   >UEFI & EDK II Training</span>

<span style="font-size:0.95em" > EDK II Continuous Integration (CI) Unit Test Framework for Developer Validation </span>

<br>
<span style="font-size:0.75em" ><a href='http://www.tianocore.org'>tianocore.org</a></span>
<br>
<span style="font-size:0.75em" >See also <a href="https://github.com/Laurie0131/EDK_II_CI_Unit_Test_Framework/blob/master/UnitTestFramework_Lab.md">UnitTestFramework_Lab.md</a> for Unit Test Framework Lab
<br>

@box[bg-purple-pp text-white rounded my-box-pad2  ](<p style="line-height:60% "><span style="font-size:0.75em;" ><b>ONLY</b> this title slide is complete<br>&nbsp;</span></p>)
Note:
  PITCHME.md for UEFI / EDK II Training  EDK II Continuous Integration (CI) Unit Test Framework for Developer Validation

  Copyright (c) 2020, Intel Corporation. All rights reserved.<BR>

  Redistribution and use in source (original document form) and 'compiled'
  forms (converted to PDF, epub, HTML and other formats) with or without
  modification, are permitted provided that the following conditions are met:

  1) Redistributions of source code (original document form) must retain the
     above copyright notice, this list of conditions and the following
     disclaimer as the first lines of this file unmodified.

  2) Redistributions in compiled form (transformed to other DTDs, converted to
     PDF, epub, HTML and other formats) must reproduce the above copyright
     notice, this list of conditions and the following disclaimer in the
     documentation and/or other materials provided with the distribution.

  THIS DOCUMENTATION IS PROVIDED BY TIANOCORE PROJECT "AS IS" AND ANY EXPRESS OR
  IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF
  MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO
  EVENT SHALL TIANOCORE PROJECT  BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
  SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
  PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS;
  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
  WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR
  OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS DOCUMENTATION, EVEN IF
  ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.



---  
@title[Lesson Objective]

### <p align="center"<span class="gold"   >Platform Build Labs </span></p>
<br>
<!---  Add bullets using https://fontawesome.com/cheatsheet certificate
-->
 @fa[certificate gp-bullet-magenta]<span style="font-size:0.9em">&nbsp;&nbsp;Pin Visual Studio Command Prompt to Windows <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Task Bar  </span><br><br>
 @fa[certificate gp-bullet-green]<span style="font-size:0.9em">&nbsp;&nbsp;Build a EDK II Platform using Emulator package </span><br><br>
 @fa[certificate gp-bullet-cyan]<span style="font-size:0.9em">&nbsp;&nbsp;Run the Emulator in Windows  </span><br><br>
   


---?image=assets/images/binary-strings-black2.jpg
@title[Pin VS CMD Prompt Section]
<br><br><br><br><br>
## <span class="gold"  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pin VS Command Prompt </span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Pin the Visual Studio Command prompt to Windows <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Task Bar</span>


---
@title[Pin VS CMD Prompt]
### <p align="right"><span class="gold" >Pin  VS Command Prompt</span></p>

@snap[north-east span-25 ]
<br>
<br>
<p style="line-height:40%" align="center">@fa[windows gp-bullet-cyan]<BR><span style="font-size:0.450em;  " >Windows 10 </span></p>
<br>
@snapend

@snap[north-east span-60 ]
<br>
<br>
<br>
<br>
<p style="line-height:80%" align="left"><span style="font-size:0.80em;  " >Steps to Pin Visual Studio Command Prompt to task bar for Windows 10 </span></p>
<ol style="line-height:0.8;">
 <li><span style="font-size:0.80em;  " >Using the Start menu in Windows 10, Left Click on "Windows Key" Lower Left @fa[windows gp-bullet-cyan]</span></li>
 <li><span style="font-size:0.80em;  " >Scroll down from the scroll bar on the right until "Visual Studio 201@color[#e49436](<i>n</i>)" </span></li>
 <li><span style="font-size:0.80em;  " >Left Click "Visual Studio 201@color[#e49436](<i>n</i>)"</span></li>
</ol>
<br>
@snapend


Note:



---?image=/assets/images/slides/Slide5.JPG
@title[Pin VS CMD Prompt 02]
### <p align="right"><span class="gold" >Pin  VS Command Prompt</span></p>
@snap[north-east span-60 ]
<br>
<br>
<br>
<br>
<p style="line-height:80%" align="left"><span style="font-size:0.80em;  " >4. Left Click <b>"Visual Studio Tools"</b> </span></p>
<br>
<p style="line-height:80%" align="left"><span style="font-size:0.80em;  " >This will open another Windows file explorer window <br></span><span style="font-size:0.60em;  " > Note: <i>VS 2013 example, other version of VS maybe different</i>  </span></p>

<br>
@snapend


Note:



---?image=/assets/images/slides/Slide6.JPG
@title[Pin VS CMD Prompt 03]
### <p align="right"><span class="gold" >Pin  VS Command Prompt</span></p>
@snap[north-east span-50 ]
<br>
<br>
<p style="line-height:80%" align="left"><span style="font-size:0.80em;  " >5. Select <b>"Developer Command Prompt for VS201<i>n</i>"</b> </span></p>
<p style="line-height:80%" align="left"><span style="font-size:0.80em;  " >6. Right Click to open Windows dialog box </span></p>
<br>
<p style="line-height:80%" align="left"><span style="font-size:0.80em;  " ><font color="yellow">Do not use any of the other<br> ".. Command Prompts" </font></span></p>

<br>
@snapend
Note:



---?image=/assets/images/slides/Slide7.JPG
@title[Pin VS CMD Prompt 04]
### <p align="right"><span class="gold" >Pin  VS Command Prompt</span></p>

@snap[north-east span-40 ]
<br>
<br>
<br>
<p style="line-height:80%" align="left"><span style="font-size:0.80em;  " >7. Left Click  on <br>&nbsp;&nbsp;&nbsp;"Pin to to taskbar" </span></p>
<br>
@snapend


Note:



---?image=/assets/images/slides/Slide8.JPG
@title[Pin VS CMD Prompt 05]
### <p align="right"><span class="gold" >Pin  VS Command Prompt</span></p>

@snap[north-east span-50 ]
<br>
<br>
<br>
<p style="line-height:80%" align="left"><span style="font-size:0.80em;" >8. Open the VS Command Prompt </span></p>
<br>
<p style="line-height:60%" align="left"><span style="font-size:0.65em; ">&nbsp;  All Windows Labs use this short-cut to Build Edk II platforms and projects using Windows Visual Studio<br>
@size[.75em](2010 / 2012 / 2013 / 2015 or 2017)</span></p>
@snapend
Note:



---?image=assets/images/binary-strings-black2.jpg
@title[End of Pin VS Section]
<br><br><br><br><br>
## <span class="gold"  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;End Pin  VS Prompt</span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>



---?image=assets/images/binary-strings-black2.jpg
@title[Lab 1 -Build Emulator Section]
<br><br><br><br><br>
## <span class="gold"  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Build Emulator</span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Setup EmulatorPkg to build and run emulation <br> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;w/ Windows</span>

---
@title[Prerequisites]
<p align="right"><span class="gold" >@size[1.1em](<b> Prerequisites </b>)</span><br>
<span style="font-size:0.75em;" >- Done Before Class  </span></p>

<ul style="list-style-type:disc; line-height:0.75;">
<li><span style="font-size:0.7em">Windows 10: &nbsp;&nbsp; @fa[windows gp-bullet-cyan] </span></li>
<ul style="list-style-type:disc; line-height:0.7;">
  <li><span style="font-size:0.65em">Continuous Integration (CI) - Stuart CI Build with  Visual Studio VS2017 or VS2019  </span></li>
  <li><span style="font-size:0.65em">Non-Stuart CI - Visual Studio VS2015, VS2017 or VS2019  </span></li>
  <li><span style="font-size:0.65em">Windows SDK (for rc) & Windows WDK (for Capsules) </span></li>
</ul>

<li><span style="font-size:0.75em">Python 3.7.x or greater and /Scripts directories on Path: <a href="https://www.python.org/">Link</a> to download  </span></li>
<li><span style="font-size:0.75em">Git for Windows on Path : <a href="http://git-scm.com/download/win">Link</a></span></li>
<li><span style="font-size:0.75em">NASM for Win64 :<a href="https://www.nasm.us/pub/nasm/releasebuilds/2.12.02/win64/">Link</a> </span></li>
</ul>

@snap[north-east span-5 ]
<br>
<br>
<br>
<br>
![VS_logo](/assets/images/Brand_Visual_Studio_Win_2019.png)
<br>
<br>
<br>
<br>
@snapend


@snap[north-east span-17 ]
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
![Python_logo](/assets/images/python-logo@2x.png)
@snapend


@snap[north span-5 ]
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
![git_logo](/assets/images/git_logo.png)
@snapend



Note:


---?image=/assets/images/slides/Slide12.JPG
@title[Create Work Space Directory]
<p align="right"><span class="gold" >@size[1.1em](<b>Create Workspace Directory  </b>)</span><br>
<span style="font-size:0.75em;" >  </span></p>

@snap[north-west span-40 ]
<br>
<br>
<br>
<br>
<br>
<br>
<br>
@box[bg-black text-white rounded my-box-pad2  ](<p style="line-height:60% "><span style="font-size:0.9em;" ><br><br><br><br><br><br>&nbsp;</span></p>)
@snapend

@snap[north-west span-50 ]
<br>
<br>
<p style="line-height:70%" align="left" ><span style="font-size:0.8em;" >
Open Windows Command Prompt <br><br>
Make new directory for Workspace: 
</span></p>
<p style="line-height:45%" align="left" ><span style="font-size:0.54em; font-family:Consolas;" ><br><br><br>&nbsp;&nbsp;
 $ cd / <br>&nbsp;&nbsp;
 $ Mkdir FW<br>&nbsp;&nbsp;
 $ cd FW<br>&nbsp;&nbsp;
 $ Mkdir edk2-ws<br>&nbsp;&nbsp;
 $ cd edk2-ws<br>&nbsp;&nbsp;
</span></p>

@snapend

Note:

---
@title[Download the EDK II Source Code ]
<p align="right"><span class="gold" >@size[1.1em](<b>Download the EDK II Source Code  </b>)</span><br>
<span style="font-size:0.75em;" >  </span></p>
<p style="line-height:80%" align="left" ><span style="font-size:0.9em;" >
Download the open source EDK II from Github &nbsp;@fa[github gp-bullet-white]
</span></p>
<p style="line-height:70%" align="left" ><span style="font-size:0.78em;" >
From the command prompt use “git clone” to download 
</span></p>
```bash
C:\FW\edk2-WS> git clone https://github.com/tianocore-training/edk2.git
C:\FW\edk2-WS> git clone https://github.com/tianocore/edk2-libc.git 
 
```
<br>
<p style="line-height:70%" align="left" ><span style="font-size:0.78em;" ><br>
Download the Submodules and Checkout the Lab Branch
</span></p>
```bash
C:\FW\edk2-wS> cd edk2
C:\FW\edk2-wS\edk2> git checkout LabBranch
C:\FW\edk2-wS\edk2> git submodule update –-init
C:\FW\edk2-wS> cd ..
 
 
```
 

---
@title[Download Lab_Material_FW -getting the Source ]
<p align="right"><span class="gold" >@size[1.1em](<b>Download Lab Material  </b>)</span><br>
<span style="font-size:0.75em;" >  </span></p>
<p style="line-height:80%" align="left" ><span style="font-size:0.85em" >Download the Lab_Material_FW.zip from : </span> @fa[github gp-bullet-white] 
<span style="font-size:0.7em"><a href="https://github.com/tianocore-training/Lab_Material_FW/archive/master.zip">github.com Lab_Matrial_FW.zip</a>
</span></p>
<br>
<span style="font-size:0.85em" >OR<br>Use "git clone" to download the Lab_Material_FW<span>
```bash
C:\> git clone https://github.com/tianocore-training/Lab_Material_FW.git
```
<span style="font-size:0.85em" >Directory Lab_Material_FW will be created</span>
```
   FW 
    - Documentation 
	- DriverWizard 
	- edk2-ws      
	- edk2Linux 
	- LabSampleCode 
	- Nasm
	
```

Note:

---?image=/assets/images/slides/Slide15.JPG
@title[Build  Edk2 -getting the Source ]
<p align="right"><span class="gold" >@size[1.1em](<b>Build EDK II  </b>)</span><br>
<span style="font-size:0.75em;" >– Extract the Source  </span></p>

@snap[north-west span-100 ]
<br>
<br>
<br>
<p style="line-height:70%" align="left"><span style="font-size:0.75em;  " >Extract the Downloaded <font face="Consolas">Lab_Material_FW-master.zip to C:\ </font> </span></p>
<br>
@snapend



Note:
Extract the Downloaded Lab_Material_FW.zip to Home (this will create a directory FW )

---?image=/assets/images/slides/Slide16.JPG
@title[Build  Edk2 -getting the Source 02]
<p align="right"><span class="gold" >@size[1.1em](<b>Build EDK II  </b>)</span><br>
<span style="font-size:0.75em;" > - Copy edk2-ws </span></p>

@snap[north-west span-100 ]
<br>
<br>
<br>
<p style="line-height:70%" align="left" ><span style="font-size:0.7em;" >From the downloaded Lab_Material_FW folder, 
<b>copy</b> and  <b>paste</b> folder "<font face="Consolas">..\edk2-ws</font>" to "<font face="Consolas">C:/FW</font>" <br>
    &nbsp;<i>Note</i>: Overwrite existing files and directories
</span></p>

@snapend



Note:
- From the downloaded Lab_Material_FW folder, copy and 
   -  paste folder “..\edk2-ws” to C:/FW


---?image=/assets/images/slides/Slide17.JPG
@title[Build  Edk2 -get Nasm]
<p align="right"><span class="gold" >@size[1.1em](<b>Build EDK II  </b>)</span><br>
<span style="font-size:0.75em;" > - Get Nasm </span></p>

@snap[north-west span-70 ]
<br>
<br>
<p style="line-height:70%" align="left" ><span style="font-size:0.7em;" >
Copy<font face="Consolas"> Nasm </font> directory to <font face="Consolas">C:&bsol;</font><br>
@size[.8em](&lpar;creating <font face="Consolas">C:&bsol;Nasm</font> directory&rpar;)
</span></p>

@snapend

Note:

Copy Nasm directory to C:\
(creating C:\Nasm directory)




---?image=assets/images/binary-strings-black2.jpg
@title[Stuart CI Build  sub Section]
<br><br><br><br><br><br>
### <span class="gold"  >Stuart CI Build EmulatorPkg </span>
<span style="font-size:0.9em" > @color[yellow](SKIP) if doing a Non-Stuart CI Build&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>

@snap[east span-20 ]
![Stuart-ci](/assets/images/Stuart-CI.png
@snapend

---?image=/assets/images/slides/Slide20.JPG
@title[Stuart CI Build  Edk2 ]
<p align="right"><span class="gold" >@size[1.1em](<b>Stuart CI Build EDK II &nbsp;&nbsp;&nbsp;&nbsp; </b>)</span><br>
<span style="font-size:0.75em;" ></span></p>

<p style="line-height:70%" align="left" ><span style="font-size:0.75em;" >1. &nbsp;
Install the pip requirements @size[.8em](&lpar;Note, Proxy option needed behind a firewall&rpar;)
</span></p>
```bash
$ pip install --upgrade -r pip-requirements.txt --proxy http://proxy-chain.intel.com:911 
```

<p style="line-height:70%" align="left" ><span style="font-size:0.75em;" >2. &nbsp;
Get the code dependencies @size[.8em](&lpar;done only when submodules change&rpar;)
</span></p>
```bash
$ stuart_setup -c EmulatorPkg/PlatformCI/PlatformBuild.py TOOL_CHAIN_TAG=<Your TAG> -a X64
```

<p style="line-height:70%" align="left" ><span style="font-size:0.75em;" >3. &nbsp;
Update other dependencies @size[.8em](&lpar;done on new VS Command Prompt&rpar;)
</span></p>
```bash
$ stuart_update -c EmulatorPkg/PlatformCI/PlatformBuild.py TOOL_CHAIN_TAG=<Your TAG> -a X64
```

<p style="line-height:70%" align="left" ><span style="font-size:0.75em;" >4. &nbsp;
Build the BaseTools @size[.8em](&lpar;done only when BaseTools change and first time&rpar;)
</span></p>
```bash
$ python BaseTools\Edk2ToolsBuild.py -t <Your TAG>
```
<p style="line-height:70%" align="left" ><span style="font-size:0.75em;" >5. &nbsp;
Compile the EmulatorPkg
</span></p>
```bash
$ stuart_build -c EmulatorPkg/PlatformCI/PlatformBuild.py TOOL_CHAIN_TAG=<Your TAG> -a X64 BLD_*_ADD_SHELL_STRING=1
```


<p style="line-height:70%" align="left" ><span style="font-size:0.7em;" >
Where "&lt;Your TAG&gt;" is either "VS2017" or "VS2018"
</span></p>




Note:

---?image=/assets/images/slides/Slide21.JPG
@title[Output from CI Stuart Build]
<p align="right"><span class="gold" >@size[1.1em](<b>Output from CI Stuart Build  </b>)</span><br>
<span style="font-size:0.75em;" ></span></p>


@snap[north-east span-40  ]
<p style="line-height:50%" align="right"><span style="font-size:0.8em" >
<br>
<br>
<br>
<br>
<br>
<br>
<br>

Finished build
</span></p>
@snapend

Note:



---?image=assets/images/binary-strings-black2.jpg
@title[Non-Stuart CI Build  sub Section]
<br><br><br><br><br>
### <span class="gold"  >Non-Stuart CI Build EmulatorPkg </span>
<span style="font-size:0.9em" > @color[yellow](SKIP) if doing a Stuart CI Build &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>


---
@title[Non-Stuart CI Build  Edk2 -build BaseTools]
<p align="right"><span class="gold" >@size[1.1em](<b>Non-Stuart CI Build EDK II  </b>)</span><br>
<span style="font-size:0.75em;" > – build <font face="Consolas">BaseTools</font></span></p>

@snap[north-west span-100 ]
<br>
<br>
<p style="line-height:60%" align="left" ><span style="font-size:0.7em;" >
Open VS Command prompt and Cd to work space directory <br>
<span style="background-color: #000000"><font face="Consolas">
@size[.7em](&nbsp;&nbsp;cd  C:&bsol;&gt;FW\edk2-ws &nbsp;&nbsp;&nbsp;&nbsp;) </font></span> <br>
<br>
Setup the local environment: (see batch file setenv.bat )<br>
<span style="background-color: #000000"><font face="Consolas">
@size[.7em](&nbsp;&nbsp;$&gt; set WORKSPACE=%CD% &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;  <br>)
@size[.7em](&nbsp;&nbsp;$&gt; set PACKAGES_PATH=%WORKSPACE%\edk2;%WORKSPACE%\edk2-libc  &nbsp;&nbsp;  )</font></span> <br>
<br>
Invoke Edksetup.bat from directory <font face="Consolas">C:/FW/edk2-ws/edk2</font> to Build <font face="Consolas">BaseTools </font><br>
<span style="background-color: #000000"><font face="Consolas">
@size[.7em](&nbsp;&nbsp;$&gt; cd edk2&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;<br>)
@size[.7em](&nbsp;&nbsp;$&gt; edksetup.bat Rebuild&nbsp;&nbsp;&nbsp;&nbsp;)</font></span> <br>
</span></p>
<br>
@snapend

@snap[south-west span-100 ]
<p style="line-height:45%" align="left" ><span style="font-size:0.5em;" >
Building BaseTools only needs to be done once but setting up local environment and edksetup.bat needs to be done each new VS prompt session
</span></p>
@snapend


@snap[east span-40 fragment ]
<br>
<br>
<br>
<br>
<p style="line-height:40%" align="left"><span style="font-size:02.80em;  " ><br>
@color[yellow](&#8678;)
</span></p>
@snapend

Note:

---?image=/assets/images/slides/Slide23.JPG
@title[Non-Stuart CI Build Edk2 -update target.txt]
<p align="right"><span class="gold" >@size[1.1em](<b>Non-Stuart CI Build EDK II  </b>)</span><br>
<span style="font-size:0.75em;" > – Update <font face="Consolas">Target.txt</font></span></p>

@snap[north-west span-70 ]
<br>
<p style="line-height:60%" align="left" ><span style="font-size:0.7em;" >
@size[1.1em](<b>EmulatorPkg</b>) - Build with edk2  <br><br>
Invoke <font face="Consolas">Edksetup.bat </font>
</span></p>
<p style="line-height:45%" align="left" ><span style="font-size:0.5em; font-family:Consolas;">
<span style="background-color: #000000">
&nbsp;&nbsp;$&gt; cd C:\FW\edk2-ws\edk2 &nbsp;&nbsp;   <br>
&nbsp;&nbsp;$&gt; edksetup.bat &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;   <br>
</span>
</span></p>

<p style="line-height:50%" align="left" ><span style="font-size:0.7em;" ><br>
<b>Edit</b> the file <font face="Consolas">Conf/target.txt</font> @size[.7em](&lpar;change TOOL_CHAIN_TAG&rpar;<br>)
<font face="Consolas">@size[.7em](&nbsp; notepad Conf/target.txt )</font>
</span></p>

@snapend

@snap[north-west span-60 ]
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<p style="line-height:34%" align="left" ><span style="font-size:0.35em; font-family:Consolas;">
<font color="black"><br><br>
&nbsp;&nbsp;TARGET_ARCH&nbsp;&nbsp;&nbsp;&nbsp;           = X64 <br>
&nbsp;&nbsp; &nbsp;&nbsp;. &nbsp;&nbsp;. &nbsp;&nbsp;. <br>
&nbsp;&nbsp;TOOL_CHAIN_TAG &nbsp;       = VS2015x86 <br>
</font>
</span></p>
@snapend


@snap[south-west span-100 ]
<p style="line-height:50%" align="left" ><span style="font-size:0.75em;" >
@size[.8em](<b>Save</b> and <b>Exit</b>)<br>
<br>
<br>
<b>Build Emulator</b>
</span></p>
<p style="line-height:50%" align="left" ><span style="font-size:0.5em; font-family:Consolas;">
<span style="background-color: #000000">
&nbsp;&nbsp;$&gt; build -D ADD_SHELL_STRING -a X64 &nbsp;&nbsp;   <br>
</span>
</span></p>
@snapend


@snap[south-east span-30 fragment ]
<p style="line-height:10%" align="left"><span style="font-size:02.80em;  " ><br><br>
@color[yellow](&#8678;)
</span></p>
@snapend




Note:

-  Cd C:/fw/edk2-ws/edk2

- invoke edksetup.bat 
- change MYTOOLS to VS2015x86 or whatever
- edit Conf/target.txt
  -  TARGET_ARCH           = X64
  -	. . .
  -  TOOL_CHAIN_TAG        = VS2015x86

-  build -D ADD_SHELL_STRING  -a X64


---
@title[Possible Build Errors]
<p align="right"><span class="gold" >@size[1.1em](<b>Possible Build Errors </b>)</span><span style="font-size:0.75em;" ></span></p>

<p style="line-height:80%"><span style="font-size:0.8em" >1. If you get a BUILD Error:  Error “<font face="Consolas">C:/Program </font>“ not found</span></p>
<ul style="line-height:0.8;">
  <li><span style="font-size:0.7em" >First check that you have opened Visual Studio and installed the “C++”   </span> </li>
  <li><span style="font-size:0.7em" >Open Visual Studio and create a “C++” project </span> </li>
  <li><span style="font-size:0.7em" > (This will take some time to install)</span> </li>
</ul>  
<p style="line-height:80%"><span style="font-size:0.8em" >2. If you get a BUILD Error: Check if  RC.Exe compiler not found is the error -<a href="https://gitpitch.com/tianocore-training/Platform_Build_Win_Emulator_Lab/master#/35" > here</a> </span> </p>
<p style="line-height:80%"><span style="font-size:0.8em" >3. If you get a BUILD Error: <font face="Consolas">fatal error C1041: cannot open program database</font> … Check 
<a href="https://gitpitch.com/tianocore-training/Platform_Build_Win_Emulator_Lab/master#/36"> here</a>  </span> </p>


Note:



---?image=/assets/images/slides/Slide25.JPG
@title[Build Edk2 -build inside VS Prompt]
<p align="right"><span class="gold" >@size[1.1em](<b>Build EDK II  </b>)</span><br>
<span style="font-size:0.75em;" > – Inside VS Prompt</span></p>


@snap[south-east span-40  ]
<p style="line-height:50%" align="right"><span style="font-size:0.8em" >
Finished build
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
</span></p>
@snapend

Note:
- 

---?image=assets/images/binary-strings-black2.jpg
@title[Run the Emulator Section]
<br><br><br><br><br>
### <span class="gold"  >Run the Emulator </span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>


---?image=/assets/images/slides/Slide27.JPG
@title[Build Edk2 -invoke emulator]
<p align="right"><span class="gold" >@size[1.1em](<b>Invoke Emulation  </b>)</span><span style="font-size:0.75em;" ></span></p>

@snap[north-west span-45 ]
<br>
<br>
<p style="line-height:65%" align="left"><span style="font-size:0.75em" >From the command prompt<br><br></span>
&nbsp;&nbsp;<font face="Consolas"><span style="background-color: #000000; font-size:0.55em; ">
&nbsp;&nbsp;$&gt;  RunEmulator.bat &nbsp;&nbsp;</span></font>
<br>
<br>
<span style="font-size:0.75em" >
OR<br>
run <font face="Consolas">@color[yellow](WinHost.exe) </font> from:<br>&nbsp;&nbsp;
<font face="Consolas">@size[.7em](Build/ . . ./X64 directory)</font>
</span></p>
<br>
<p style="line-height:50%" align="left"><span style="font-size:0.5em" > Notice 2 "GOP Window n" opened </span></p>
@snapend



Note:

---?image=/assets/images/slides/Slide28.JPG
@title[Build Edk2 -exit emulator]
<p align="right"><span class="gold" >@size[1.1em](<b>Emulator at Shell Prompt  </b>)</span><span style="font-size:0.75em;" ></span></p>

@snap[north-west span-45 ]
<br>
<br>
<br>
<p style="line-height:80%" align="left"><span style="font-size:0.8em" >Type: "Reset" to exit<br><br>
</span></p>
@snapend

Note:


---  
@title[Summary]
##### <p align="center"<span class="gold"   >Summary </span></p><br>

 @fa[certificate gp-bullet-magenta]<span style="font-size:0.9em">&nbsp;&nbsp;Pin Visual Studio Command Prompt to Windows <br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Task Bar  </span><br><br>
 @fa[certificate gp-bullet-green]<span style="font-size:0.9em">&nbsp;&nbsp;Build a EDK II Platform using Emulator package </span><br><br>
 @fa[certificate gp-bullet-cyan]<span style="font-size:0.9em">&nbsp;&nbsp;Run the Emulator in Windows  </span><br><br>
 

---?image=assets/images/gitpitch-audience.jpg
@title[Questions]
<br>
![Questions](/assets/images/questions.JPG =10x) 

---
@title[return to main]
<p align="center"><span class="gold"   >@size[1.2em](<b>Return to Main Training Page</b>)</span></p>
<br>
<br>
<br>
<br>
<br>
<p align="center"><span style="font-size:0.9em">Return to Training Table of contents for next presentation <a href="https://github.com/tianocore-training/Tianocore_Training_Contents/wiki#schedule--outline">link</a></span></p>

@snap[north span-30 ]
<br>
<br>
<br>
<a href="https://github.com/tianocore-training/Tianocore_Training_Contents/wiki#schedule--outline">
![trainingLogo](/assets/images/returnTrainingLogo.png)</a>
@snapend

---?image=assets/images/gitpitch-audience.jpg
@title[Logo Slide]
<br><br><br>
![Logo Slide](/assets/images/TianocoreLogo.png =10x)


---
@title[Acknowledgements]
#### <p align="center"><span class="gold"   >Acknowledgements</span></p>

```c++
/**
Redistribution and use in source (original document form) and 'compiled' forms (converted
to PDF, epub, HTML and other formats) with or without modification, are permitted provided
that the following conditions are met:

Redistributions of source code (original document form) must retain the above copyright 
notice, this list of conditions and the following disclaimer as the first lines of this 
file unmodified.

Redistributions in compiled form (transformed to other DTDs, converted to PDF, epub, HTML
and other formats) must reproduce the above copyright notice, this list of conditions and 
the following disclaimer in the documentation and/or other materials provided with the 
distribution.

THIS DOCUMENTATION IS PROVIDED BY TIANOCORE PROJECT "AS IS" AND ANY EXPRESS OR IMPLIED 
WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND 
FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL TIANOCORE PROJECT BE 
LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES 
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, 
DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, 
WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) 
ARISING IN ANY WAY OUT OF THE USE OF THIS DOCUMENTATION, EVEN IF ADVISED OF THE POSSIBILITY 
OF SUCH DAMAGE.

Copyright (c) 2020, Intel Corporation. All rights reserved.
**/

```


---?image=assets/images/binary-strings-black2.jpg
@title[Backup Section]
<br><br><br><br><br>
## <span class="gold"  >&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Backup</span>
<span style="font-size:0.9em" > &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;</span>

---  
@title[Build Errors]
<br>
<br>
<br>
<br>
##### <p align="center"<span class="gold"   >Build Errors</span></p><br>


---
@title[Build Error- RC.exe ]
<p align="right"><span class="gold" ><b>Build Error- RC.exe </b></span></p>
<p style="line-height:90%"><span style="font-size:0.9em" >Because RC.Exe is not found, Error Message:</span></p>

```
   "c:\Program Files (x86)\Windows Kits\8.0\bin\x64\rc.exe" 
/Foc:\edkii.svn\Build\NT32IA32\DEBUG_VS2013x86\IA32\MdeModulePkg\Application\HelloWorld\HelloWorld\OUTPUT
\HelloWorldhii.lib 
c:\edkii.svn\Build\NT32IA32\DEBUG_VS2013x86\IA32\MdeModulePkg\Application\HelloWorld\HelloWorld\OUTPUT\He
lloWorldhii.rc
'c:\Program' is not recognized as an internal or external command,
operable program or batch file.
 
NMAKE : fatal error U1077: '"c:\Program Files (x86)\Windows Kits\8.0\bin\x64\rc.exe' : return code '0x1'
Stop.

```

<p style="line-height:90%"><span style="font-size:0.9em" >Find where the RC.EXE is located on your VS Installation:  </span></p>

<p style="line-height:90%"><span style="font-size:0.9em" >Example (VS 2013):  The RC.exe is located on this machine: <br>
<span style="font-size:0.5em" >`C:\Program Files (x86)\Windows Kits\8.1\bin\x64` </span></span></p>
<span style="font-size:0.9em" >Edit `Conf/tools_def.txt` </span>

Note:


+++
@title[Build Error- RC.exe 02]
<p align="right"><span class="gold" ><b>Build Error- RC.exe Cont...</b></span></p>

<span style="font-size:0.9em" ><b>Edit</b> `Conf/tools_def.txt` </span><br>
<p style="line-height:90%"><span style="font-size:0.9em" >Search for your installation of Visual Studio (2013, 2015 or 2017)</span></p>
<p style="line-height:90%"><span style="font-size:0.9em" >Update according to the path for where the RC.EXE is found </span></p>

```bash
# Microsoft Visual Studio 2013 Professional Edition
DEFINE WINSDK8_BIN       = c:\Program Files\Windows Kits\8.1\bin\x86\
DEFINE WINSDK8x86_BIN    = c:\Program Files (x86)\Windows Kits\8.1\bin\x64
 
# Microsoft Visual Studio 2015 Professional Edition
DEFINE WINSDK81_BIN       = c:\Program Files\Windows Kits\8.1\bin\x86\
DEFINE WINSDK81x86_BIN    = c:\Program Files (x86)\Windows Kits\8.1\bin\x64

# Microsoft Visual Studio 2017 Professional Edition
DEFINE WINSDK10_BIN       = C:\Program Files (x86)\Windows Kits\10\bin\x86
```

<p style="line-height:90%"><span style="font-size:0.9em" >Copy and Paste RC error to `Tools_def.txt`
<a href="https://github.com/tianocore-training/Platform_Build_Win_Emulator_Lab/blob/master/PITCHME.md#copy-paste-for-rc-error">link</a>
</span></p>


Note:
## Copy paste for RC Error
```bash
# Microsoft Visual Studio 2013 Professional Edition
DEFINE WINSDK8_BIN       = c:\Program Files\Windows Kits\8.1\bin\x86\
DEFINE WINSDK8x86_BIN    = c:\Program Files (x86)\Windows Kits\8.1\bin\x64
 
# Microsoft Visual Studio 2015 Professional Edition
DEFINE WINSDK81_BIN       = c:\Program Files\Windows Kits\8.1\bin\x86\
DEFINE WINSDK81x86_BIN    = c:\Program Files (x86)\Windows Kits\8.1\bin\x64

```

### RC FIX for VS 2017 at command prompt type > Set
```
 See what the value of WINSDK10_PREFIX is.  This is probably the problem
 Search your directory "C:\Program Files (x86)\" for the file rc.exe
 the one you want will be in  C:\Program Files (x86)\Windows Kits\10\bin\x86
 see below for the define: 
  From : DEFINE WINSDK10_BIN       = ENV(WINSDK10_PREFIX)DEF(VS2017_HOST)
  to : DEFINE WINSDK10_BIN       = C:\Program Files (x86)\Windows Kits\10\bin\x86
```

---
@title[Build Error- C1041 ]
<p align="right"><span class="gold" ><b>Build Error: fatal error C1041: </b></span></p>
<p style="line-height:90%"><span style="font-size:0.9em" >Build Error from fatal error C1041: cannot open program database</span></p>

<p style="line-height:90%"><span style="font-size:0.9em" >This Error is usually because the location you are building is being shared by another application in Windows.  Example: Syncplicity may cause this</span></p>

<span style="font-size:0.9em" >Error Message:</span>

```
k:\fw\edk2\MdePkg\Library\BaseLib\LinkedList.c : fatal error C1041: cannot open program 
database 
'k:\fw\edk2\build\nt32ia32\debug_vs2013x86\ia32\mdepkg\library\baselib\baselib\vc120.pdb'; if 
multiple CL.EXE write to the same .PDB file, please use /FS
NMAKE : fatal error U1077: '"C:\Program Files (x86)\Microsoft Visual Studio 
12.0\Vc\bin\cl.exe"' : return code '0x2'
Stop.

```

<p style="line-height:90%"><span style="font-size:0.9em" ><b>Solution:</b>  Try using a Workspace that is not shared
</span></p>

