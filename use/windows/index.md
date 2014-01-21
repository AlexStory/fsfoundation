---
layout: page
title: Use F# on Windows | The F# Software Foundation
headline: Use F# on Windows
---


### Option 1: Install the Visual F# Tools from Microsoft

![logo](/images/thumbs/vstudio.png)&nbsp;On Windows, F# programmers commonly use the Visual F# Tools from Microsoft.

If you already have Visual Studio 2012 or 2013 (Ultimate or Professional), then you already have F#. If not, then either get a [trial edition](http://www.visualstudio.com/downloads/download-visual-studio-vs); or

1. [Install the Visual F# Express Tools](http://go.microsoft.com/fwlink/?LinkID=261287)
2. See [fsharp.net](http://fsharp.net) for more information about the Visual F# Tools from Microsoft. 

You can also use a different editor and the command-line compiler (fsc.exe) or F# Interactive (fsi.exe) 
after you have installed the Visual F# Tools.

#### Visual Studio Power Tools for F# ####

There are some power tools which are handy to use with Visual Studio:

 - [Fantomas source code formatter](http://visualstudiogallery.msdn.microsoft.com/24ef5c87-b4e3-4c3b-b126-1064cc66e148) Provide formatting commands for F# in Visual Studio
 - [F# depth colorizer](http://visualstudiogallery.msdn.microsoft.com/07636c36-52be-4dce-9f2e-3c56b8329e33) Use F# parse tree information to display structure of F# code using background color
 - [FSharpJump](http://visualstudiogallery.msdn.microsoft.com/ddde6ac9-20c9-4c9b-92f6-090b09ab944a) An outlining and navigation tool for F#
 - [Math symbols](http://visualstudiogallery.msdn.microsoft.com/fe627c2a-5d09-4252-bcc7-300821ae707c) Math (Unicode) symbol extension for F#
 - [F# Outlining](http://visualstudiogallery.msdn.microsoft.com/bec977b8-c9d9-4926-999e-e50c4498df8a) Extension for F# regions outlining
 - [F# XML Doc](https://github.com/brianmcn/FSharpXmlDoc) An extension which automatically creates F# XmlDoc template when you type `///`
 - [FsEye](https://code.google.com/p/fseye/) A visual object tree inspector for the F# Interactive
 - [Regions and navigation bar](http://tomasp.net/blog/regions-navigation.aspx/) Code collapsing and Navigation bar for F#

##### Note to ReSharper users #####
When some versions of ReSharper are installed, the `Alt+Enter` shortcut key for the `Execute in Interactive`
command of the F# project system doesn't work, because ReSharper overrides this shortcut key for its own purposes.
However, there is no actual command clash, so you can keep using `Alt-Enter` both in F# and ReSharper without having
to remap keys.

To enable this, either upgrade to ReSharper 8.0.10.1959 or greater, or install the [resharper-fsi-friendly](https://github.com/citizenmatt/resharper-fsi-friendly) plugin.

<br />

### Option 2: Install F# and Xamarin Studio 

![logo](/images/thumbs/xamarin-studio.png)&nbsp;[Xamarin Studio](http://xamarin.com/studio) is a free IDE for general purpose development with commercial add-ins for mobile development. [MonoDevelop](http://monodevelop.com) is a free and open source IDE based on the same code.  F# can be used with either.

1. Install [the free standalone F# compiler tools](http://go.microsoft.com/fwlink/?LinkId=261286) 
2. Install [Xamarin Studio](http://xamarin.com/studio) or [MonoDevelop](http://monodevelop.com) for Windows
3. Install the F# Addin for Xamarin Studio or MonoDevelop from Tools --> Add-in Manager --> Gallery. 

   If no addins appear, press "Refresh" on the "Updates" tab of the Add-in Manager.

<br />


### Option 3: Install the F# compiler and tools alone

If you're just looking for a compiler and/or F# Interactive, e.g. for a build server or cloud VM image, then:

1. Requires .NET 4.5:

   On Windows 8 and Windows 2012 Server, this is already present by default
   
   On Windows 7 and Windows 2008 Server, [install .NET 4.5](http://www.microsoft.com/net/download) from Microsoft

2. Requires the Windows SDK:

   On Windows 8 or Windows 2012 Server use the [Windows 8 and .NET 4.5 SDK](http://msdn.microsoft.com/en-us/windows/hardware/hh852363.aspx) from Microsoft
   
   On Windows 7 or Windows 2008 Server use the [Windows 7 and .NET 4.0 SDK](http://www.microsoft.com/en-us/download/details.aspx?id=8279) from Microsoft
   
3. [Install the free standalone F# compiler tools](http://go.microsoft.com/fwlink/?LinkId=261286) from Microsoft

   Alternatively, do a quiet install from a PowerShell administrator prompt (the URL is the redirect of the above). 

       $webclient = New-Object Net.WebClient
       $url = 'http://download.microsoft.com/download/0/5/E/05E5C5E3-2A52-434F-A09E-C8150B987D09/VWD_FSharp.exe'
       $webclient.DownloadFile($url, "$pwd\VWD_FSharp.exe")
       .\VWD_FSharp.exe /install /quiet

The compiler tools are installed at

    C:\Program Files (x86)\Microsoft SDKs\F#\3.0\Framework\v4.0\fsc.exe
    C:\Program Files (x86)\Microsoft SDKs\F#\3.0\Framework\v4.0\fsi.exe
    C:\Program Files (x86)\Microsoft SDKs\F#\3.0\Framework\v4.0\fsiAnyCpu.exe
    
<br />

### Option 4: Install Tsunami

[Tsunami](http://tsunami.io) is an innovative fully featured F# IDE. 
It has a number of unique features ideally suited for Big Data, Data Science and Machine Learning. It is capable of being embedded directly into other Desktop Applications and Websites.

- Desktop: Install MSI from [Download](http://tsunami.io/download.html)
- Browser: Embed the object in [Cloud Tsunami](http://tsunami.io/cloud_tsunami.html)


<br />


### Option 5: Build HTML5 web apps or WinJS Windows Store apps

* ![logo](/images/thumbs/WebSharper.png)&nbsp;[Using F# for HTML5 Web Applications](/use/html5)

<br />

### Option 6: Learn F# in the Browser

* ![logo](/images/thumbs/tryfsharp.jpg)&nbsp;[Learn F# online at Try F#](http://tryfsharp.org)

<br />

### Option 7: Build F# from source

* Build the F# compiler and library from [the source](http://fsharp.github.com/fsharp)

