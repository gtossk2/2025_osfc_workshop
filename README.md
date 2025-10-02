2025 OSFC Workshop Pre-built Image for Running OpenBMC and Validating
Server Manageability on Virtual Arm Servers

* Pre-built Image : https://github.com/gtossk2/2025_osfc_workshop/releases/tag/v1.0
* Docs : https://gitlab.arm.com/server_management/PoCs/fvp-poc
* Quick steps :

```
# Install Host Dependencies
$> sudo apt update
$> sudo apt install qemu-kvm libvirt-daemon-system iproute2 pv xterm pushd popd script nohup sshpass ssh socat head telnet retry pgrep inotify-tools
$> sudo systemctl start libvirtd

# Execute fvp-poc
$> tar -xvf run-fvp-poc.tar.gz
$> cd run-fvp-poc
$> ./setup_tap.sh
$> ./run.sh -m /home/ubuntu/run-fvp-poc/host/binary/models/Linux64_GCC-9.3/FVP_RD_V3_R1
```

