# Linux admin commands
- **Check if port is used:**
  `fuser 1099/tcp`

- **Check os info:**
  `uname -a`

- **Check ip:**
  `ifconfig` or `ip addr show`

- **Work with services (systemd):**
  `service service_name status/stop/start` or
  `systemctl status service_name`
  `enable/disable` options to on/off autostart

- **Check open ports (network sockets):**
  `netstat` use `-tulpn` for typical udp/tcp check (use sudo to see PIDs of all processes)

- **Check wayland session:**
  `echo $XDG_SESSION_TYPE`

- **Find process:**

  `pidof process_name` or `ps -aux | grep process_name`

- **Stop all processes (SIGKILL) by name:**

  `killall -s 9 process_name`