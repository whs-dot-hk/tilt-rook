```sh
sudo dd if=/dev/zero of=/var/lib/libvirt/images/rook-0.img bs=1M seek=4096 count=0
sudo dd if=/dev/zero of=/var/lib/libvirt/images/rook-1.img bs=1M seek=4096 count=0
sudo dd if=/dev/zero of=/var/lib/libvirt/images/rook-2.img bs=1M seek=4096 count=0
```
```sh
virsh attach-device --config debian11-kind rook-0.xml
virsh attach-device --config debian11-kind rook-1.xml
virsh attach-device --config debian11-kind rook-2.xml
```
