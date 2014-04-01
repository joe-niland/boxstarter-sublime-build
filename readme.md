# Sublime Build System for BoxStarter

## Installation
1. Copy boxstarter.sublime-build to %APPDATA%\Sublime Text 3\Data\Packages\User\

   Now when you look in the **Tools -> Build System** menu, you'll see a **BoxStarter** entry.

## Usage
The build system file has been configured to be auto-selected when working on files with extension **.ps1**.
If you are OK with that, simply open your ChocolateyInstall.ps1 file from withih your BoxStart package's tools directory and hit **Ctrl-B**.

If you already have a build system in place for **.ps1** file select **Tools -> Build System -> BoxStarter** to manually enable the build system. As above, using the keyboard shortcut **Ctrl-B** will build your package.

BoxStarter will place the built package in your chosen Local Repository location. By default this is `%APPDATA%\Boxstarter\BuildPackages\`

## BoxStarter Environment Configuration

You can view the current BoxStart config with the command:

   Get-BoxStarterConfig

You can change this location from within Powershell/BoxStarter Shell with the command:
   
   Set-BoxStarterConfig -LocalRepo YOUR_REPO_PATH

More info here: http://boxstarter.org/UsingBoxstarter

## Licence

The MIT License (MIT)

Copyright (c) 2014 Joe Niland

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.