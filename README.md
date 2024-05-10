# LinuxOnWin11
## Install ubuntu in Win11 using hyper-v to run .net7 application compiled with visual studio
- Enbale hyper-v in win11 pro
- Create a virtual machine to install ubuntu
  https://ubuntu.com/server/docs/how-to-set-up-ubuntu-on-hyper-v
- Install .net SDK and runtime
  https://learn.microsoft.com/en-us/dotnet/core/install/linux-ubuntu-install?tabs=dotnet8&pivots=os-linux-ubuntu-2404

  ```
  sudo snap install dotnet-sdk --classic
  sudo apt-get install -y dotnet-runtime-7.0
  ```
- Create a .net7 project in visual studio
- Publish the .net project target to linux-64 in visual studio
  https://www.youtube.com/watch?v=V0xBxA6a-MI
- Just directly copy the publish result to ubuntu system
- Make dll executable and run it in terminal

## Run Avalonia in ubuntu
* Install Avalonia extension in visual studio https://docs.avaloniaui.net/docs/get-started/
* New an Avalonia application that contains 2 projects, and the one with the extension of Desktop is the executable app
* Just publish the Desktop project
* Copy the result to ubuntu system to execute
