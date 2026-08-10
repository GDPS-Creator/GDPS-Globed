# Helping
If you happen to notice any issues and know how to fix them, please submit an issue; you’ll be helping not just yourself, but the entire GDPS creator community! 
Try to be kind to each other!
# Informations
This method of adding Globed multiplayer does not require knowledge of C++ or any other programming language; all you need is patience and the desire to do it!

**What you will need:**
- Playit.gg | Required to create the domain used to access the multiplayer mode; this is a free option, though you can use private VPS hosting instead.
- Clone the repository | Ideally, use the `git clone` command, or simply download the ZIP archive via `Code -> Download ZIP`.
- Any text editor. | VSCode or Notepad or Notepad++
- Your GDPS database credentials. | MySQL and FTP

# Instruction
*I will explain using the example of Playit.gg.*

- Go to Playit, register an account, and create a tunnel.
- Enter a name of your choice (e.g., "globed-server"—you won't actually need it).
- For the IP address, enter either 127.0.0.1 (meaning you will host it on your PC) or the IP of your VPS/router with open ports.
- Set the port to 4342 and the mode to UDP.
- Then, fill in the details using the following format:
```
memory_usage = 3
compression_level = 3
central_server_url = "127.0.0.1:4342 (or the router's IP address with open ports, or a VPS hosting IP)"
central_server_password = "any password (We recommend leaving it at the default setting.)"
server_name = "Pixel Multiplayer (Multiplayer name (any))"
server_id = "main-server"
server_region = "Global"
server_address = "(In Playit, you will find your unique tunnel address at the top; copy it and paste it here, replacing this text.)"
enable_stat_tracking = false
tickrate = 30
verify_script_signatures = true

[tcp]
enable = true
address = "0.0.0.0:5351"

[udp]
enable = true
ping_only = false
address = "0.0.0.0:5351"
binds = 1

[logging]
file_enabled = true
directory = "logs"
file_level = "debug"
console_level = "info"
filename = "game-server.log"
rolling = false
retention_days = 7
```
It is highly recommended to create a second tunnel using port 5351 in Playit.gg

# For questions, please use the Issues section.
