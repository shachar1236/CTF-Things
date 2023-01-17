# CTF-Things



## A list of useful things that can help you in CTFs.
---------------------------------------
## Websites

## [Beeceptor](https://beeceptor.com/)
```
A website where you can create a mock api that can act as your server and recive requests.
```

-----------------------
## Payloads

### [Payload All The Things](https://github.com/swisskyrepo/PayloadsAllTheThings)
```
A useful repository that has all kinds of payload for a lot of diffrent attacks.
```

### A Python code that can call a function from any library without using the import statment.
```
[t for t in ().__class__.__base__.__subclasses__() if t.__name__ == 'Sized'][0].__len__.__globals__['__builtins__']['__import__'](<the library name>).<the function>

example:
[t for t in ().__class__.__base__.__subclasses__() if t.__name__ == 'Sized'][0].__len__.__globals__['__builtins__']['__import__']("subprocess").check_output(['ls', '-l'])

In this example we call the check_output function from the subprocess library.
This example can essentioly run any shell code on the machine using python.
```

-----------------------------
## Tools

### [Burp suite](https://portswigger.net/burp/communitydownload)
```
Everyone knows burpsuite, but for those who dont I can explain:
essentialy burp suite let you see your http traffic, act as a proxy, change http requests, and a lot more!!!
```


### [Wireshark](https://www.wireshark.org/)
```
Another classic like burp suite...
Wireshark lets you sniff the network traffic on your computer and open sniffs files.
```

### [Ida](https://hex-rays.com/ida-free/)
```
A reverse engineering tool!
lets you see the assembly code of a program in a graph representation.
```

### [Ghidra](https://github.com/NationalSecurityAgency/ghidra)
```
A decompiler for cpp, very good for reverse engineering!
```

-----------------------------
## Python libraries

### [Requests](https://pypi.org/project/requests/)
```
A python library that lets you send http requests on the web.
```

### [Pwn tools](https://docs.pwntools.com/en/stable/)
```
A python library that gives you a lot of tools to use in CTFs.
Tools like - netcat from a script with the pwn.remote function, analizing binary files.
```

******************
