+++
title = "Foundations"
author = ["svejk"]
lastmod = 2021-04-21T21:47:13-04:00
draft = false
weight = 1
+++

## The Command Line {#the-command-line}

The term **command line** will here refer to the various non-GUI executables installed with an operating system, along with the built-ins, keywords, and scripting capabilities available from the shell. To delineate some terms (and risk offending experts):

-   <span class="underline">terminal</span> : GUI window; takes commands and shows output
-   <span class="underline">shell</span> : the software that interprets and executes the commands typed in the terminal; examples are bash, sh, csh, tcsh, etc.
-   <span class="underline">CLI (Command Line Interface)</span> : a user interface in which users type commands and see results printed on the screen

Most examples are given in the bash shell and command language, largely due to its ubiquity.  This is often the only tool available to penetration testers, for example. <sup id="0bcbef12832cf2ccd09acf31ef8c6898"><a href="#troncone2019cybersecurity" title="Troncone \&amp; D, Cybersecurity Ops with bash: Attack, Defend, and Analyze  from the Command Line, O'Reilly Media (2019).">troncone2019cybersecurity</a></sup>


### Running bash commands on Windows {#running-bash-commands-on-windows}

There are several options for running bash commands on Windows systems.

-   <span class="underline">Git Bash</span> : The Windows installation of Git includes a port of bash.  **Git Bash** is herein the method of choice.
-   <span class="underline">Cygwin</span> : Cygwin is a full-featured Linux emulator that also includes the ability to install a variety of packages. Like Git Bash, it allows calling a number of native Windows commands in addition to standard Linux commands.
-   <span class="underline">Windows Subsystem for Linux</span> : Windows 10 includes a native method to run Linux if the Windows Subsystem for Linux (WSL) is installed.


### Command Line Basics {#command-line-basics}

When several words appear on the command line, bash assumes the first is the name of a program and the rest are arguments.  To have bash run the command \`mkdir\` and supply it with two arguments, one would input

{{< highlight shell "linenos=table, linenostart=1" >}}
mkdir -p /tmp/new/directory
{{< /highlight >}}

where, as is convention, the option is first and begins with '-'.  This creates a new directory **/tmp/new/directory**, and the option ensures no errors are reported and any intervening directories will be created along the way.

The commands that can be run are either files, built-ins, or keywords.
