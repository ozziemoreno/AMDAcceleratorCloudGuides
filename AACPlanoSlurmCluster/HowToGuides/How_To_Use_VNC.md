# How To Use VNC on AAC

## Starting a VNC server

### Option 1: Interactive

The first metthod is to start an interactive job on the cluster, requesting number of GPUs and the partition that has been assigned. 
```
salloc --exclusive --mem=0 -p 1CN128C8G2H_2IB_MI210_Ubuntu22
```
This command allocates all the CPUs/GPUs with `--exclusive` and all the memory with `--mem=0`, the default duration for this particular partition/queue is 1 day.

Once the node has been allocated, we setup our environment for VNC.
```
module load turbovnc/3.0.3
```
Then we start the VNC server. (The first time the command is run, it will prompt us for a password - this is so other unauthorized users are not allowed on the VNC session. We recommend a strong password.)
```
vncserver :5
```
The output of this command is important. 

It tells us the name of the compute node `smc-r08-07` and the display port `:5` we will be using. 
```
Desktop 'TurboVNC: smc-r08-07:5 (ozmoreno)' started on display smc-r08-07:5

Starting applications specified in /shared/apps/ubuntu/turbovnc/3.0.3/bin/xstartup.turbovnc
Log file is /shared/prod/home/ozmoreno/.vnc/smc-r08-07:5.log
```

## Connecting to your VNC Server
Since the compute nodes in our cluster are only accessible through our login node, we must create a "tunnel" to the compute node. This will allow our VNC Client to access the compute node. 

The display port we assigned to the compute node will be needed, which will be `5900 + <display_port>`
```
started on display smc-r08-07:5
```
will use port 5905

### Option 1: Creating an SSH Tunnel
We will be using a basic template to create a tunnel to the compute node. This command will be executed in a new terminal on your local machine. 
```
ssh -N -L <port>:<compute_node_hostname>:<port> <username>@aac1.amd.com
```
The above command will establish an SSH tunnel so that we can connect our VNC Viewer.

Open the VNC Client installed on the local machine and connect to `localhost:<display_port>`

![image](https://github.com/ozziemoreno/AMDAcceleratorCloudGuides/assets/109979778/3bc5c8b7-821c-4de8-a42f-ba18f13c15b2)

Since we set up a password, we should be prompted for it upon connecting. 

## Killing a VNC Session
If we started the VNC Server on the wrong node we can kill it using the following command. 
```
vncserver -kill :<display> 
```
Following the example above, we would kill the VNC Session on display `:5`
