# RHCSA Study Kit

Old school discipline. Forward looking habits. Practical above all. This folder is a complete, hands-on path to pass RHCSA with confidence.

## What’s inside

Each module is a self-contained guide with mental models, must-know commands, pitfalls, labs, and a full solution key.

0. **Essential Tools** → [0.Understand-and-use-essential-tools.md](./0.Understand-and-use-essential-tools.md)
   Shell basics, redirection, grep and regex, SSH, targets, archives, editing, links, permissions, documentation.

1. **Manage Software** → [1.Manage-Software.md](./1.Manage-Software.md)
   Repos, DNF and RPM, module streams, Flatpak, ISO media repos, troubleshooting, speed drills.

2. **Create Simple Shell Scripts** → [2.Create-Simple-shell-Scripts.md](./2.Create-Simple-shell-Scripts.md)
   Shebangs, conditionals, loops, arguments, command output, functions, traps, ten tiny exam-grade scripts.

3. **Operate Running Systems** → [3.Operate-running-systems.md](./3.Operate-running-systems.md)
   Safe reboot, targets, boot interruption for recovery, process control, tuned, journals, services, secure transfers.

4. **Configure Local Storage** → [4.Configure-Local-Storage.md](./4.Configure-Local-Storage.md)
   MBR and GPT, LVM from PV to LV, XFS and ext4, UUID and LABEL in fstab, online growth, non-destructive expansion.

5. **Create and Configure File Systems** → [5.Create-and-Configure-file-systems.md](./5.Create-and-Configure-file-systems.md)
   XFS, ext4, VFAT, NFS client, autofs, extend LVs, permissions and ACLs, SELinux context fixes.

6. **Deploy, Configure, and Maintain Systems** → [6.Deploy-Configure-and-maintain-systems.md](./6.Deploy-Configure-and-maintain-systems.md)
   at and cron, service management, default targets, chrony, software from CDN or local, GRUB work.

7. **Manage Basic Networking** → [7.Manage-basic-networking.md](./7.Manage-basic-networking.md)
   IPv4 and IPv6 with nmcli, DNS and hostname, services at boot, firewalld runtime vs permanent, rich rules.

8. **Manage Users and Groups** → [8.Manage-users-and-groups.md](./8.Manage-users-and-groups.md)
   User and group lifecycle, password aging, sudo with drop-ins, shared group directories, gotchas.

9. **Manage Security** → [9.Manage-Security.md](./9.Manage-Security.md)
    Firewalld, umask and default ACLs, SSH keys, SELinux modes, contexts, booleans, port labels, restorecon mastery.

## How to use this kit

1. **Read the mental model** at the top of each module. You learn faster when you know why.
2. **Run the labs** exactly as written on a RHEL box or compatible environment. Verify every command.
3. **Speedrun the drills** the day after. Repetition builds calm under the clock.
4. **Fix your mistakes loudly**. Keep a scratch file of commands that bit you and why.

Coffee is recommended. Panic is not.

## Recommended lab setup

* One RHEL 9 VM for the main work.
* An extra VM to act as an SSH or NFS peer when needed.
* Keep SELinux Enforcing and firewalld running. That is the exam reality.
* Snapshot before storage and bootloader modules. You will thank yourself later.

## 10 day plan

* **Days 1–2**: Essential Tools, Shell Scripts
* **Day 3**: Users and Groups
* **Day 4**: Networking
* **Day 5**: Software Management
* **Day 6**: Operate Running Systems
* **Day 7**: Local Storage
* **Day 8**: File Systems + NFS + autofs
* **Day 9**: Security + SELinux
* **Day 10**: Full speed review. Run every “speed drill” once. Fix red flags.

## Conventions used

* Commands are ready to paste. Use `sudo` where shown.
* Paths are absolute. Variables are quoted. No guesswork.
* After editing `/etc/fstab` always run `mount -a`. After `--permanent` firewall changes always `--reload`. After changing GRUB with mkconfig always regenerate the correct path for BIOS or UEFI.

## Disclaimer

These notes target RHCSA-style skills on RHEL 9. Adjust minor package names or paths if your image differs.

