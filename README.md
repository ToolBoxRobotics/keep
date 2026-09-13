# keep


Remove the sudo password prompt in the Ubuntu terminal
```bash
sudo visudo
```
```txt
sudo ALL=(ALL:ALL) ALL     ->     %sudo ALL=(ALL:ALL) NOPASSWD:ALL
```

