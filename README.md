🛠️ Rust Server Manager
<img width="799" height="722" alt="изображение" src="https://github.com/user-attachments/assets/054bc9b9-8e2b-4203-8ea4-a1f5f3e931ba" />

Rust Server Manager is a simple desktop application made with Python + PySide6 to easily install, configure, launch, and manage a Rust Dedicated Server.
✨ Features

    ✅ Install and update Rust server via steamcmd

    ⚙️ Configure server settings (port, seed, name, level, etc.)

    💾 Save and load all settings to/from config.json

    ▶️ Start / ⏹️ Stop the server

    💬 Send commands to the server console

    📥 Download and install Exiled mod framework

🖥️ Requirements

    Internet connection for downloading server files

Python dependencies:

pip install -r requirements.txt

<details> <summary>📄 requirements.txt content</summary>

PySide6

</details>
🚀 How to Use
1. Run the App

2. First Launch

    The app will automatically create a server_config.json file.

    Set your server name, level, port, and other fields.

    Click Save or Start Server to begin.

3. Install or Update Rust Server

Click the Install/Update Server button.
This uses steamcmd to download the latest server files.
4. Start the Server

After installation, press Start Server. The live console will appear below.
5. Send Console Commands

Enter any server command in the input field and press Send.
6. Stop the Server

Click Stop Server to safely stop it.
⚙️ Server Settings

The following settings are saved in server_config.json:

{
  "hostname": "My Rust Server",
  "port": 28015,
  "level": "Procedural Map",
  "maxplayers": 10,
  "seed": 12345,
  "rcon_port": 28016,
  "rcon_password": "changeme",
  "description": "My Rust Server",
  "url": "https://example.com"
}

You can also edit this file manually if needed.
🧩 Exiled Mod

To install Exiled, click the Install Exiled button.
If the default link gives 404, make sure the link is correct and not outdated (you can update it manually in the code if needed).
🧼 Troubleshooting

    Server doesn't start?
    Make sure steamcmd installed the server correctly in RustDedicated/.

    Exiled not downloading?
    Their releases change — update the .zip link in code.

    Console not showing all output?
    Python doesn't always flush all stdout — check future updates for improvements.

📁 File Structure

RustServerManager/
├── server_config.json     
└──  RustDedicated/             


📜 License

MIT License – free to use.
Just don’t resell it without permission.
