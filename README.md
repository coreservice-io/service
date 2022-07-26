# Service

Install app as system service, support Linux and Darwin

Precompiled files in /build

daemon-darwin-amd64<br />
daemon-linux-amd64<br />
daemon-linux-arm64<br />

If you need other system files, please compile it yourself.

## How to use
1. Compile program according to the operating system. 
2. Copy the compiled file into your project package and rename to "daemon".
3. Run cmd "sudo ./daemon [install/remove/start/stop/restart/status] [app name]"to manage process

### for example
```
├─yourProjectFolder
│  ├─configs    //cofig folder
│  ├─logs       //log folder
│  ├─assets     //assets folderr
│  ├─myapp      //executable file
│  └─daemon    //daemon file compiled and copy from this package
```

run cmd
```
//enter yourProjectFolder
cd ./yourProjectFolder

sudo ./daemon install myapp [arg1] [arg2] ...
sudo ./daemon start myapp
sudo ./daemon status myapp
sudo ./daemon restart myapp
sudo ./daemon stop myapp
sudo ./daemon remove myapp
```


