<div align="center">

## Create a new thread in VB\.Net


</div>

### Description

Create a new thread with ease.
 
### More Info
 


<span>             |<span>
---                |---
**Submitted On**   |
**By**             |[Thomas Raben](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByAuthor/thomas-raben.md)
**Level**          |Intermediate
**User Rating**    |3.8 (15 globes from 4 users)
**Compatibility**  |VB\.NET
**Category**       |[System Services/ Functions](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByCategory/system-services-functions__10-23.md)
**World**          |[\.Net \(C\#, VB\.net\)](https://github.com/Planet-Source-Code/PSCIndex/blob/master/ByWorld/net-c-vb-net.md)
**Archive File**   |[](https://github.com/Planet-Source-Code/thomas-raben-create-a-new-thread-in-vb-net__10-67/archive/master.zip)





### Source Code

This is the way to make a thread in VB.Net, and its very easy:<br><br>
class myThread<br>
  sub newThread()<br>
    msgbox("Hello from another thread.")<br>
  end sub<br>
end class<br><br>
Now, place this code, where you want to start the thread:<br><br>
dim thread as new myThread()<br>
dim mThread as new system.threading.threadstart(addressof thread.newThread)<br>
dim oThread as new system.threading.thread(mThread)<br>
oThread.start()<br><br>
That's it, and it works compiled, etc.<br>

