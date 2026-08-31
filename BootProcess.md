<div align = "center">
 <h1> BOOT PROCESS </h1>
 </div>
<div>
  <p><b>Booting:</b> The process by which a computer initializes its 
    hardware components and loads the operating system into main memory, 
    making system ready for operations.</p>
</div>
<div>
  <h2>Steps that a computer follow to transform from a powered-off state to a fully-functional system are:-</h2>
  <li type = "none">
      <ul><b>Step 1: </b> Power ON 
      <p>Press the Power button</p>
      </ul>
      <ul><b> Step 2: </b> BIOS|UEFI 
      <p>BIOS and UEFI are the firmware typically resides in a computer chip and not on a hard drive. 
      It is not a part of the Operating System. </p>
       <li type ="none"> 
         <ul> <b> Step 2.1 POST - Power On Self Test: </b> In order to check the operability of all the hardware 
         connected to our computer system, BIOS carries out POST which will check the hardware components and if any problem 
         is found user is alerted with POST beeps and POST screen messaged. </ul>
 <br>       
<ul> <b> Step 2.2 Loads the MBR: </b> It loads and executes the first sector off the disk it decides to boot from. This first sector of a hard disk is called the Master Boot Recorder. </ul>
        </ul>
       </li>
 
 <ul><b>Step 3:</b> Executes MBR - 1st stage boot-loader
<p>The program in boot sector is loaded in memory and executed. This tiny program has information which programs should it load into memory next and where that program is located in Disk or Boot device. </p> </ul>
 
 <ul><b>Step 4: </b> Volume Boot Record - 2nd stage boot-loader 
<p>Such as GRUB, BOOTMGR, or BootX. Here, an Operating System is transferred to the kernel image and control is transferred to the kernel of the operating system. </p></ul>
  </li>
<ul><b>Step 5:</b> Kernel Initialization
 <p>After loading the kernel, bootloader turns over execution to it and the kernel initializes the rest of the operating system. Such as loads device drivers, sets up interrupts, and starts the process scheduler. </p> </ul> 

<ul><b>Step 6: </b> User Space Initialization
<p>Kernel then start the first user process called <b>systemd/init</b>. It always runs with Process ID (PID) 1.</p>
</ul>

<ul>
 <b>Step 7:</b> System Services Start 
 <p>Background services and daemons are started—for example, networking, audio, printing, security, and other system services. </p>
</ul>

<ul>
 <b>Step 8: </b> Login Screen Appears
<p> The operating system displays a GUI or command-line login interface.</p>
</ul>

<ul>
 <b>Step 9: </b> Applications Run 
 <p>After the user logs in, applications can be launched. The kernel allocates memory and CPU resources, and the CPU executes the application's instructions.</p>
</ul>
</div>
