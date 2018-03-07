# GPGPU enabled HPC Cloud Platform based on OpenStack(基于OpenStack利用GPGPU构建高性能计算云平台)

## 1. 存在的问题    
1. > But still these commercial Cloud services provide GPU instance with PCI pass-through technique that virtual machines (VMs) cannot access other's host's GPU.    
PCI 传输技术`PCI pass-through`只能让连接的本地主机使用GPU，无法让其他主机上的虚拟机访问。    

## 2. 期望的效果    
1. > Using GPUs across network

2. > Additionally if node with a GPU is occupied by VMs that don't use a GPU, there should be way to provider the GPU, which remains idle, to other VMs.    
   此外，如果具有CPU的节点被不使用GPU的VM占用，则应该有办法将空闲的GPU提供给其他VM。    

## 3. 论文亮点    
1. > `rCUDA API forwarding technique`. With API forwarding, our Cloud platform can support multiple VMs to share single GPU which is important to maximize GPU resource utilization.    
   利用`rCUDA API forwarding technique`，支持多个虚拟机共享单个GPU。    

2. > Also it is possible for single VM to use multiple GPUs across different hosts.    
   单个虚拟机跨不同的主机使用他们的GPU也是可能的。    


