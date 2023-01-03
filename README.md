# C# Code Challenge

* Write a GUI application to run the Windows `ping` utility, collect, process, and display the results.
* The GUI should display two buttons, Start and Stop that control the execution of the `ping` utility. 
* The GUI should display a text box to allow the user to enter a destination hostname or IP address.
* The GUI should provide a control to display results in a tabular format.
* When Start is pressed the `ping` utility should be run repeatedly every 5 seconds.
  * Each execution only needs to send a single request, limit this with the `-n` argument.
* The output of each execution of `ping` should be parsed and stored.
* The collected output should be processed every 1 minute and a mininum/maximum/average for the round trip time should be calculated for each 1 minute period.
  * The individual samples should be taken from the `time` value in the ping output.
* These aggregate 1 minute results should be presented in the GUI continuously as they are generated.

## General Approach and Assumptions

* This program should be written in C# using a recent version of .NET (5.0 or greater)
* The program should be built in Visual Studio Community Edition and use standard tooling and no thirdparty dependencies.
* Pick a native Microsoft Windows GUI toolkit of your choice (WinUI, WPF, WinForms)
* Ping is located at C:\Windows\System32\ping.exe

## Criteria

* You will not be evaluated on the UI design, but rather your ability to separate the concerns of the GUI from the rest of code and to correctly handle any ansynchronous interaction.
* Consistency of coding style.
* Correct error handling.
* Appropriate unit tests.
* Your solution must build and run cleanly by pressing F5 in Visual Studio Community Edition after opening from a clean clone of your repository.

## How to Submit Your Work

1. Fork this repository on GitHub.
2. Commit your solution preferably in multiple commits demonstrating your development process.
3. When you're finished, send us the URL of your public repository.