pvesh create /nodes/promox01/lxc \
      -vmid 1001 \
      -ostemplate local:vztmpl/ubuntu-16.04-x64-base.tar.gz \
      -cores 2 -cpuunits 1024 \
      -memory 4096 -swap 128 \
      -hostname ct1001.example.com \
      -net1 name=eth1,ip=192.168.0.2/32,bridge=vmbr1 \
      -rootfs local:24 \
      -onboot 1
