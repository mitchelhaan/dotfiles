## Useful Commands
Force SSH to connect to a server, regardless of the host key validity. I find this useful when SSHing into live images, because the host key is different on every boot. From [ShellHacks](https://www.shellhacks.com/disable-ssh-host-key-checking/).
```
ssh -o "UserKnownHostsFile=/dev/null" -o "StrictHostKeyChecking=no" user@host
```
