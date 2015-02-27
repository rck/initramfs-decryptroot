# initramfs-decryptroot
A hook for initramfs to include a script to ease decryption of encrypted root file systems in early boot (e.g., via dropbear/ssh).

Assume you have your '/' file system encrypted and your server is (in a galaxy) far, far away. How do you enter the password to unlock '/'?

## Debian
- Follow this nice [blog post](http://blog.neutrino.es/2011/unlocking-a-luks-encrypted-root-partition-remotely-via-ssh/)
- Place that hook into /etc/initramfs-tools/hooks and regenerate the initramfs
- Regenerate initramfs
