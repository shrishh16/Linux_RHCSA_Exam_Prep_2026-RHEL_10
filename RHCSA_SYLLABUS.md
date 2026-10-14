# RHCSA EX200 — Complete Topic Tree & Study Sequence

> **Exam:** Red Hat Certified System Administrator (EX200)  
> **Based on:** Red Hat Enterprise Linux 10  
> **Format:** 100% Hands-on, performance-based (no internet, no notes allowed)  
> **Duration:** 3 hours | **Passing Score:** 210/300 (70%)  
> **Golden Rule:** ALL configurations must persist after reboot without intervention.

---

## How to Use This File

1. **Follow the sequence** — Topics are ordered so each builds on the previous.
2. **Create folders** for each Module (the folder structure is shown below).
3. **Each subtopic** = one focused study session (1-2 hours).
4. **Practice on a VM** after every subtopic — never just read.
5. **Checkboxes** track your progress. Mark `[x]` when done.

---

## Your Folder Structure (Create This)

```
Linux/
├── RHCSA_SYLLABUS.md              ← THIS FILE (your master guide)
│
├── Module-01_Essential_Tools/
│   ├── 01_Shell_Basics/            ✅ COMPLETED
│   ├── 02_IO_Redirection/
│   ├── 03_Grep_and_Regex/
│   ├── 04_File_and_Text_Management/
│   ├── 05_Links_Hard_and_Soft/
│   ├── 06_File_Permissions/
│   ├── 07_Archiving_and_Compression/
│   └── 08_SSH_Remote_Access/
│
├── Module-02_File_System_Navigation/
│   ├── 01_Linux_File_System_Hierarchy/
│   ├── 02_Navigation_Commands/
│   └── 03_File_and_Directory_Operations/
│
├── Module-03_Users_Groups_Permissions/
│   ├── 01_User_Management/
│   ├── 02_Group_Management/
│   ├── 03_Password_and_Aging/
│   ├── 04_Standard_Permissions_ugo_rwx/
│   ├── 05_Special_Permissions_SUID_SGID_Sticky/
│   ├── 06_Default_Permissions_umask/
│   └── 07_Privileged_Access_sudo/
│
├── Module-04_Operate_Running_Systems/
│   ├── 01_Boot_Reboot_Shutdown/
│   ├── 02_Systemd_Targets/
│   ├── 03_Interrupt_Boot_Password_Recovery/
│   ├── 04_Process_Management/
│   ├── 05_Process_Scheduling_nice_renice/
│   ├── 06_Tuning_Profiles/
│   ├── 07_System_Logging_rsyslog/
│   ├── 08_Journalctl_and_Persistent_Journals/
│   └── 09_Service_Management_systemctl/
│
├── Module-05_Software_Management/
│   ├── 01_RPM_Basics/
│   ├── 02_DNF_Package_Manager/
│   ├── 03_Repository_Configuration/
│   └── 04_Flatpak_Management/
│
├── Module-06_Shell_Scripting/
│   ├── 01_Variables_and_Input/
│   ├── 02_Conditional_Execution_if_test/
│   ├── 03_Loops_for_while_until/
│   ├── 04_Processing_Command_Output/
│   └── 05_Practical_RHCSA_Scripts/
│
├── Module-07_Local_Storage/
│   ├── 01_Storage_Concepts_Block_Devices/
│   ├── 02_GPT_Disk_Partitioning/
│   ├── 03_LVM_Physical_Volumes/
│   ├── 04_LVM_Volume_Groups/
│   ├── 05_LVM_Logical_Volumes/
│   ├── 06_Extending_Logical_Volumes/
│   └── 07_Swap_Management/
│
├── Module-08_File_Systems/
│   ├── 01_Creating_File_Systems_ext4_XFS_VFAT/
│   ├── 02_Mounting_and_fstab/
│   ├── 03_NFS_Network_File_System/
│   ├── 04_Autofs_Automounting/
│   └── 05_Diagnosing_Permission_Problems/
│
├── Module-09_Networking/
│   ├── 01_Network_Concepts/
│   ├── 02_IPv4_Configuration_nmcli/
│   ├── 03_IPv6_Configuration/
│   ├── 04_Hostname_and_DNS_Resolution/
│   ├── 05_Network_Services_at_Boot/
│   └── 06_Firewalld_Configuration/
│
├── Module-10_System_Deployment_and_Maintenance/
│   ├── 01_Task_Scheduling_cron_at/
│   ├── 02_Systemd_Timer_Units/
│   ├── 03_Time_Services_Chrony/
│   ├── 04_Bootloader_GRUB2/
│   └── 05_System_Target_Configuration/
│
├── Module-11_Security_SELinux/
│   ├── 01_SELinux_Concepts_and_Modes/
│   ├── 02_SELinux_File_and_Process_Contexts/
│   ├── 03_Restoring_Default_Contexts/
│   ├── 04_SELinux_Port_Labels/
│   ├── 05_SELinux_Booleans/
│   ├── 06_SSH_Key_Based_Authentication/
│   └── 07_Firewall_Security_Rules/
│
└── Module-12_Exam_Practice/
    ├── Mock_Exam_1/
    ├── Mock_Exam_2/
    └── Pre_Reboot_Checklist/
```

---

## COMPLETE TOPIC TREE (Dendogram)

```
RHCSA EX200 (RHEL 10)
│
├─── MODULE 1: ESSENTIAL TOOLS ✅ (partially done)
│    │
│    ├─── 1.1 Shell Basics ✅ COMPLETED
│    │    ├── Terminal, Console, Shell, Prompt
│    │    ├── Types of Shells (bash, sh, zsh, ksh)
│    │    ├── Login vs Non-Login Shell
│    │    ├── Interactive vs Non-Interactive Shell
│    │    ├── Shell Configuration Files
│    │    ├── Command Format (command + options + arguments)
│    │    ├── Internal vs External Commands
│    │    ├── Command History & Shortcuts
│    │    ├── Tab Completion
│    │    ├── Quoting & Escaping
│    │    ├── man Pages & Documentation
│    │    └── Shell Scripting Introduction
│    │
│    ├─── 1.2 I/O Redirection
│    │    ├── File Descriptors (stdin=0, stdout=1, stderr=2)
│    │    ├── Output Redirection (>, >>)
│    │    ├── Error Redirection (2>, 2>>)
│    │    ├── Combined Redirection (&>, 2>&1)
│    │    ├── Input Redirection (<, <<, <<<)
│    │    ├── /dev/null (discarding output)
│    │    ├── Pipes (|, |&)
│    │    └── tee Command (write to file AND screen)
│    │
│    ├─── 1.3 Grep & Regular Expressions
│    │    ├── grep Basics (-i, -v, -n, -r, -l, -c, -w)
│    │    ├── Basic Regular Expressions (. * ^ $ [] [^])
│    │    ├── Extended Regular Expressions (+ ? | () {})
│    │    ├── grep with Pipes (filtering output)
│    │    └── Practical: Searching logs and config files
│    │
│    ├─── 1.4 File & Text Management
│    │    ├── Creating Files (touch, vim, nano, echo, cat)
│    │    ├── Viewing Files (cat, less, more, head, tail, tail -f)
│    │    ├── Editing Files with vim (modes, navigation, editing, search/replace)
│    │    ├── Copying Files (cp, cp -r, cp -a, cp -p)
│    │    ├── Moving/Renaming (mv)
│    │    ├── Deleting (rm, rm -r, rm -f, rmdir)
│    │    ├── Creating Directories (mkdir, mkdir -p)
│    │    ├── File Information (file, stat, wc)
│    │    └── Sorting & Processing (sort, uniq, cut, awk, sed basics)
│    │
│    ├─── 1.5 Hard Links & Soft Links
│    │    ├── Inodes Explained
│    │    ├── Hard Links (ln, same inode, can't cross fs, can't link dirs)
│    │    ├── Soft/Symbolic Links (ln -s, different inode, can cross fs, can link dirs)
│    │    ├── Differences & When to Use Which
│    │    └── Identifying Links (ls -li, readlink)
│    │
│    ├─── 1.6 File Permissions (ugo/rwx)
│    │    ├── Understanding rwx (read, write, execute)
│    │    ├── User, Group, Others (ugo)
│    │    ├── Reading ls -l Output
│    │    ├── chmod — Symbolic Mode (u+x, g-w, o=r)
│    │    ├── chmod — Numeric/Octal Mode (755, 644)
│    │    ├── chown & chgrp (changing ownership)
│    │    ├── Directory Permissions (r=list, w=create/delete, x=cd into)
│    │    └── Recursive Permissions (-R)
│    │
│    ├─── 1.7 Archiving & Compression
│    │    ├── tar — Create Archives (tar -cvf)
│    │    ├── tar — Extract Archives (tar -xvf)
│    │    ├── tar — List Contents (tar -tvf)
│    │    ├── gzip / gunzip (.gz) — tar -czvf
│    │    ├── bzip2 / bunzip2 (.bz2) — tar -cjvf
│    │    ├── xz / unxz (.xz) — tar -cJvf
│    │    ├── Extracting to Specific Directory (-C)
│    │    └── Preserving Permissions
│    │
│    └─── 1.8 SSH & Remote Access
│         ├── SSH Basics (ssh user@host, ssh -p port)
│         ├── First Connection (host key verification)
│         ├── SSH Key Generation (ssh-keygen)
│         ├── Copying Keys (ssh-copy-id)
│         ├── Key-Based Authentication Setup
│         ├── SSH Config File (~/.ssh/config)
│         ├── Secure File Transfer (scp, sftp, rsync)
│         └── SSH Server Config (/etc/ssh/sshd_config)
│
├─── MODULE 2: FILE SYSTEM NAVIGATION
│    │
│    ├─── 2.1 Linux File System Hierarchy
│    │    ├── / (root), /home, /etc, /var, /tmp
│    │    ├── /boot, /usr, /opt, /dev, /proc, /sys
│    │    ├── /bin, /sbin, /lib (and their /usr counterparts)
│    │    └── Purpose of Each Directory
│    │
│    ├─── 2.2 Navigation Commands
│    │    ├── pwd, cd, cd -, cd .., cd ~
│    │    ├── Absolute vs Relative Paths
│    │    └── . (current), .. (parent), ~ (home)
│    │
│    └─── 2.3 Listing & Finding Files
│         ├── ls (options: -l, -a, -h, -R, -t, -S, -d, -i)
│         ├── find (by name, type, size, time, permissions, exec)
│         └── locate & updatedb
│
├─── MODULE 3: USERS, GROUPS & PERMISSIONS
│    │
│    ├─── 3.1 User Management
│    │    ├── /etc/passwd File Structure (7 fields)
│    │    ├── /etc/shadow File Structure
│    │    ├── useradd (options: -u, -g, -G, -d, -s, -c, -m)
│    │    ├── usermod (options: -aG, -L, -U, -s, -d -m)
│    │    ├── userdel / userdel -r
│    │    └── /etc/default/useradd, /etc/login.defs, /etc/skel
│    │
│    ├─── 3.2 Group Management
│    │    ├── /etc/group File Structure
│    │    ├── groupadd, groupmod, groupdel
│    │    ├── Adding Users to Groups (usermod -aG, gpasswd)
│    │    ├── Primary vs Supplementary Groups
│    │    └── groups, id, newgrp Commands
│    │
│    ├─── 3.3 Password & Aging Policies
│    │    ├── passwd Command (set, lock, unlock)
│    │    ├── chage Command (-M, -m, -W, -I, -E, -d, -l)
│    │    ├── Password Aging Explained
│    │    └── Force Password Change on Next Login
│    │
│    ├─── 3.4 Standard Permissions (ugo/rwx)
│    │    ├── Read, Write, Execute — Files vs Directories
│    │    ├── chmod (symbolic & numeric)
│    │    ├── chown, chgrp
│    │    └── Recursive Operations
│    │
│    ├─── 3.5 Special Permissions
│    │    ├── SUID (4xxx) — Run as file owner
│    │    ├── SGID (2xxx) — Run as group / inherit group on dirs
│    │    ├── Sticky Bit (1xxx) — Only owner can delete
│    │    └── Identifying: ls -l shows s, S, t, T
│    │
│    ├─── 3.6 Default Permissions (umask)
│    │    ├── How umask Works (666/777 minus umask)
│    │    ├── Viewing: umask, umask -S
│    │    ├── Setting: umask 0027
│    │    └── Making Persistent (~/.bashrc, /etc/bashrc)
│    │
│    └─── 3.7 Privileged Access (sudo)
│         ├── /etc/sudoers File Format
│         ├── visudo Command (safe editing)
│         ├── /etc/sudoers.d/ Drop-in Files
│         ├── Syntax: user HOST=(RUNAS) COMMANDS
│         ├── NOPASSWD Configuration
│         └── wheel Group
│
├─── MODULE 4: OPERATE RUNNING SYSTEMS
│    │
│    ├─── 4.1 Boot, Reboot & Shutdown
│    │    ├── systemctl poweroff / reboot / halt
│    │    ├── shutdown Command (options: -h, -r, -c, +time)
│    │    └── Wall Messages
│    │
│    ├─── 4.2 Systemd Targets (Runlevels)
│    │    ├── What Are Targets? (multi-user, graphical, rescue, emergency)
│    │    ├── systemctl get-default
│    │    ├── systemctl set-default
│    │    ├── systemctl isolate (switch at runtime)
│    │    └── Target Equivalents to Old Runlevels
│    │
│    ├─── 4.3 Interrupt Boot — Password Recovery
│    │    ├── Accessing GRUB2 Menu
│    │    ├── Editing Kernel Parameters (rd.break, init=/bin/bash)
│    │    ├── Remounting / as rw (mount -o remount,rw /sysroot)
│    │    ├── chroot /sysroot
│    │    ├── Resetting Root Password
│    │    ├── SELinux Relabeling (touch /.autorelabel)
│    │    └── Complete Step-by-Step Procedure
│    │
│    ├─── 4.4 Process Management
│    │    ├── Viewing Processes (ps aux, ps -ef, top, htop)
│    │    ├── Identifying CPU/Memory Intensive Processes
│    │    ├── Signals (SIGTERM=15, SIGKILL=9, SIGHUP=1)
│    │    ├── kill, killall, pkill
│    │    ├── Job Control (bg, fg, jobs, &, Ctrl+Z)
│    │    └── nohup (persist after logout)
│    │
│    ├─── 4.5 Process Scheduling (nice/renice)
│    │    ├── Nice Values (-20 to +19)
│    │    ├── nice -n value command (start with priority)
│    │    ├── renice -n value -p PID (change running process)
│    │    └── Only root can set negative nice values
│    │
│    ├─── 4.6 Tuning Profiles (tuned)
│    │    ├── What is tuned?
│    │    ├── tuned-adm list / active / profile / recommend
│    │    ├── Common Profiles (balanced, throughput-performance, virtual-guest)
│    │    └── Enabling tuned service
│    │
│    ├─── 4.7 System Logging (rsyslog)
│    │    ├── /etc/rsyslog.conf Configuration
│    │    ├── Log Files: /var/log/messages, secure, boot.log, cron
│    │    ├── Facilities & Priorities
│    │    └── Custom Log Rules
│    │
│    ├─── 4.8 Systemd Journal (journalctl)
│    │    ├── journalctl (all logs)
│    │    ├── journalctl -u unit (service logs)
│    │    ├── journalctl -f (follow/live tail)
│    │    ├── journalctl -p priority (filter by severity)
│    │    ├── journalctl -b (current boot)
│    │    ├── journalctl --since / --until (time filters)
│    │    ├── Persistent Journals (/var/log/journal, Storage=persistent)
│    │    └── journald.conf Configuration
│    │
│    └─── 4.9 Service Management (systemctl)
│         ├── start / stop / restart / reload
│         ├── enable / disable / enable --now
│         ├── status / is-active / is-enabled
│         ├── list-units / list-unit-files
│         ├── mask / unmask
│         ├── daemon-reload
│         └── Secure File Transfer (scp, sftp, rsync)
│
├─── MODULE 5: SOFTWARE MANAGEMENT
│    │
│    ├─── 5.1 RPM Basics
│    │    ├── What is RPM? (Red Hat Package Manager)
│    │    ├── rpm -qa (query all installed)
│    │    ├── rpm -qi package (info)
│    │    ├── rpm -ql package (list files)
│    │    ├── rpm -qf /path (which package owns file)
│    │    └── rpm -ivh / -e (install/remove)
│    │
│    ├─── 5.2 DNF Package Manager
│    │    ├── dnf install / remove / update
│    │    ├── dnf search / info / list
│    │    ├── dnf provides (find which package has a file)
│    │    ├── dnf group list / group install
│    │    ├── dnf history (transaction history)
│    │    └── dnf clean all
│    │
│    ├─── 5.3 Repository Configuration
│    │    ├── /etc/yum.repos.d/*.repo Files
│    │    ├── Repo File Format ([repo-id], name, baseurl, enabled, gpgcheck)
│    │    ├── dnf repolist / repolist all
│    │    ├── dnf config-manager --add-repo
│    │    └── Enabling/Disabling Repos
│    │
│    └─── 5.4 Flatpak Management (NEW in RHEL 10)
│         ├── What is Flatpak? (sandboxed apps)
│         ├── flatpak remote-add / remote-list / remote-delete
│         ├── flatpak install / uninstall
│         ├── flatpak list / search / update
│         └── Flatpak vs RPM — When to Use Which
│
├─── MODULE 6: SHELL SCRIPTING
│    │
│    ├─── 6.1 Variables & User Input
│    │    ├── Defining Variables (VAR="value")
│    │    ├── Using Variables ($VAR, ${VAR})
│    │    ├── Environment vs Local Variables (export)
│    │    ├── readonly Variables
│    │    ├── read Command (interactive input)
│    │    └── Positional Parameters ($0, $1, $#, $@, $*)
│    │
│    ├─── 6.2 Conditional Execution
│    │    ├── if / elif / else / fi
│    │    ├── test Command (equivalent to [ ])
│    │    ├── [ ] Single Brackets
│    │    ├── [[ ]] Double Brackets (extended)
│    │    ├── File Tests: -f, -d, -e, -r, -w, -x, -s
│    │    ├── String Tests: -z, -n, =, !=
│    │    ├── Numeric Tests: -eq, -ne, -lt, -le, -gt, -ge
│    │    └── case / esac Statement
│    │
│    ├─── 6.3 Looping Constructs
│    │    ├── for Loop (lists, files, ranges, command output)
│    │    ├── while Loop
│    │    ├── until Loop
│    │    ├── break & continue
│    │    ├── Reading Files Line by Line (while read)
│    │    └── C-style for Loop: for ((i=0; i<10; i++))
│    │
│    ├─── 6.4 Processing Command Output
│    │    ├── Command Substitution: $(command)
│    │    ├── Piping Inside Scripts
│    │    ├── Processing with cut, awk, sed
│    │    ├── Capturing Exit Status ($?)
│    │    └── Error Handling (|| and &&)
│    │
│    └─── 6.5 Practical RHCSA Scripts
│         ├── User Management Scripts
│         ├── System Monitoring Scripts
│         ├── Backup Scripts
│         └── Exam-Style Scripting Tasks
│
├─── MODULE 7: LOCAL STORAGE (LVM & Partitions)
│    │
│    ├─── 7.1 Storage Concepts
│    │    ├── Block Devices (/dev/sda, /dev/vda, /dev/nvme0n1)
│    │    ├── Partitions vs Whole Disks
│    │    ├── MBR vs GPT Partition Tables
│    │    ├── lsblk, blkid, fdisk -l
│    │    └── /dev/mapper, Device-Mapper
│    │
│    ├─── 7.2 GPT Disk Partitioning
│    │    ├── fdisk /dev/sdX (interactive partitioning)
│    │    ├── gdisk (GPT-specific tool)
│    │    ├── parted (scriptable partitioning)
│    │    ├── Creating, Deleting, Resizing Partitions
│    │    ├── Partition Types (Linux, swap, LVM)
│    │    └── partprobe (inform kernel of changes)
│    │
│    ├─── 7.3 LVM — Physical Volumes (PV)
│    │    ├── What is a PV?
│    │    ├── pvcreate /dev/sdX1
│    │    ├── pvs / pvdisplay
│    │    └── pvremove
│    │
│    ├─── 7.4 LVM — Volume Groups (VG)
│    │    ├── What is a VG?
│    │    ├── vgcreate vg_name /dev/sdX1
│    │    ├── vgs / vgdisplay
│    │    ├── vgextend / vgreduce
│    │    └── vgremove
│    │
│    ├─── 7.5 LVM — Logical Volumes (LV)
│    │    ├── What is an LV?
│    │    ├── lvcreate -n name -L size vg_name
│    │    ├── lvcreate -l 100%FREE
│    │    ├── lvs / lvdisplay
│    │    ├── LV Path: /dev/vg/lv or /dev/mapper/vg-lv
│    │    └── lvremove
│    │
│    ├─── 7.6 Extending Logical Volumes
│    │    ├── lvextend -L +5G /dev/vg/lv
│    │    ├── lvextend -l +100%FREE
│    │    ├── Resize Filesystem: xfs_growfs (XFS)
│    │    ├── Resize Filesystem: resize2fs (ext4)
│    │    ├── lvextend -r (extend + resize in one step)
│    │    └── XFS Can ONLY Grow (never shrink)
│    │
│    └─── 7.7 Swap Management
│         ├── What is Swap?
│         ├── Creating Swap Partition (mkswap, swapon)
│         ├── Creating Swap on LVM
│         ├── Persistent Swap in /etc/fstab
│         ├── swapon --show, free -h
│         └── Adding Swap Non-Destructively
│
├─── MODULE 8: FILE SYSTEMS
│    │
│    ├─── 8.1 Creating File Systems
│    │    ├── mkfs.xfs (default in RHEL)
│    │    ├── mkfs.ext4
│    │    ├── mkfs.vfat (FAT32)
│    │    ├── XFS vs ext4 vs VFAT — Comparison
│    │    └── Labels: xfs_admin -L, e2label
│    │
│    ├─── 8.2 Mounting & Persistent Mounts (fstab)
│    │    ├── mount /dev/X /mnt/point (temporary)
│    │    ├── umount
│    │    ├── /etc/fstab Format (device, mountpoint, type, options, dump, pass)
│    │    ├── Mounting by UUID (blkid to find UUID)
│    │    ├── Mounting by LABEL
│    │    ├── mount -a (test fstab without reboot!)
│    │    └── df -h, du -sh
│    │
│    ├─── 8.3 NFS (Network File System)
│    │    ├── What is NFS?
│    │    ├── Installing nfs-utils
│    │    ├── showmount -e server (discover exports)
│    │    ├── Manual Mount: mount -t nfs server:/share /mnt
│    │    └── Persistent NFS in /etc/fstab
│    │
│    ├─── 8.4 Autofs (Auto-mounting)
│    │    ├── What is Autofs? (mounts on demand)
│    │    ├── Installing autofs
│    │    ├── Master Map: /etc/auto.master.d/*.autofs
│    │    ├── Indirect Maps (relative paths)
│    │    ├── Direct Maps (absolute paths)
│    │    ├── Wildcard Maps (* for any subdirectory)
│    │    └── systemctl enable --now autofs
│    │
│    └─── 8.5 Diagnosing File Permission Problems
│         ├── Check Standard Permissions (ls -l)
│         ├── Check Ownership (chown)
│         ├── Check SELinux Context (ls -Z)
│         ├── Check Mount Options (noexec, nosuid, ro)
│         └── Troubleshooting Approach (systematic)
│
├─── MODULE 9: NETWORKING
│    │
│    ├─── 9.1 Network Concepts
│    │    ├── IP Addresses, Subnets, Gateways
│    │    ├── IPv4 vs IPv6
│    │    ├── Network Interfaces (eth0, ens33, enp0s3)
│    │    ├── NetworkManager Service
│    │    └── nmcli vs nmtui vs nm-connection-editor
│    │
│    ├─── 9.2 IPv4 Configuration (nmcli)
│    │    ├── nmcli device status
│    │    ├── nmcli connection show
│    │    ├── nmcli connection modify (ipv4.addresses, gateway, dns, method)
│    │    ├── nmcli connection add (new connection)
│    │    ├── nmcli connection up (activate)
│    │    └── Static vs DHCP Configuration
│    │
│    ├─── 9.3 IPv6 Configuration
│    │    ├── IPv6 Address Format
│    │    ├── nmcli connection modify (ipv6.addresses, gateway, method)
│    │    └── Verifying: ip -6 addr show
│    │
│    ├─── 9.4 Hostname & DNS Resolution
│    │    ├── hostnamectl set-hostname
│    │    ├── /etc/hostname
│    │    ├── /etc/hosts (static entries)
│    │    ├── /etc/resolv.conf (DNS — managed by NM)
│    │    ├── nmcli connection modify ipv4.dns
│    │    └── Testing: getent hosts, dig, nslookup
│    │
│    ├─── 9.5 Network Services at Boot
│    │    ├── systemctl enable NetworkManager
│    │    ├── Connection autoconnect settings
│    │    └── Verifying after reboot
│    │
│    └─── 9.6 Firewalld
│         ├── Firewalld Concepts (zones, services, ports, rich rules)
│         ├── firewall-cmd --get-default-zone
│         ├── firewall-cmd --list-all
│         ├── firewall-cmd --add-service=X --permanent
│         ├── firewall-cmd --add-port=X/tcp --permanent
│         ├── firewall-cmd --remove-service/port --permanent
│         ├── firewall-cmd --reload
│         ├── Changing Default Zone
│         ├── Rich Rules (source-based filtering)
│         └── Runtime vs Permanent (--permanent + --reload)
│
├─── MODULE 10: SYSTEM DEPLOYMENT & MAINTENANCE
│    │
│    ├─── 10.1 Task Scheduling — cron
│    │    ├── Crontab Format (min hour day month weekday command)
│    │    ├── crontab -e / -l / -r
│    │    ├── System Crontab: /etc/crontab, /etc/cron.d/
│    │    ├── Cron Directories: /etc/cron.daily, hourly, weekly, monthly
│    │    ├── Access Control: /etc/cron.allow, /etc/cron.deny
│    │    └── Common Patterns (*/5, 0 2 * * 1-5, etc.)
│    │
│    ├─── 10.2 Task Scheduling — at
│    │    ├── at now + 5 minutes
│    │    ├── at 14:00, at noon tomorrow
│    │    ├── atq (list), atrm (remove)
│    │    └── /etc/at.allow, /etc/at.deny
│    │
│    ├─── 10.3 Systemd Timer Units
│    │    ├── Timer Unit (.timer) + Service Unit (.service)
│    │    ├── OnCalendar= (calendar-based)
│    │    ├── OnBootSec= (time after boot)
│    │    ├── OnUnitActiveSec= (recurring)
│    │    ├── systemctl list-timers
│    │    └── Creating Custom Timers (step-by-step)
│    │
│    ├─── 10.4 Time Services (Chrony)
│    │    ├── What is NTP? Why time sync matters?
│    │    ├── /etc/chrony.conf (server, pool, iburst)
│    │    ├── systemctl enable --now chronyd
│    │    ├── chronyc sources (check sync)
│    │    ├── chronyc tracking
│    │    ├── timedatectl (view/set timezone, NTP status)
│    │    └── timedatectl set-timezone, set-ntp
│    │
│    └─── 10.5 Bootloader (GRUB2)
│         ├── /etc/default/grub (TIMEOUT, CMDLINE_LINUX)
│         ├── grub2-mkconfig -o /boot/grub2/grub.cfg
│         ├── UEFI: /boot/efi/EFI/redhat/grub.cfg
│         ├── grubby (modify kernel parameters)
│         └── Adding/Removing Kernel Boot Parameters
│
├─── MODULE 11: SECURITY & SELinux
│    │
│    ├─── 11.1 SELinux Concepts & Modes
│    │    ├── What is SELinux? (Mandatory Access Control)
│    │    ├── Enforcing vs Permissive vs Disabled
│    │    ├── getenforce / setenforce (temporary)
│    │    ├── /etc/selinux/config (persistent)
│    │    └── Why SELinux Matters (real-world security)
│    │
│    ├─── 11.2 SELinux Contexts
│    │    ├── Context Format: user:role:type:level
│    │    ├── ls -Z (file contexts)
│    │    ├── ps -Z (process contexts)
│    │    ├── id -Z (user context)
│    │    └── Important Types (httpd_sys_content_t, etc.)
│    │
│    ├─── 11.3 Managing & Restoring Contexts
│    │    ├── semanage fcontext -l (list rules)
│    │    ├── semanage fcontext -a -t type "/path(/.*)?" (add rule)
│    │    ├── restorecon -Rv /path (apply contexts)
│    │    ├── chcon (temporary change — lost on restorecon)
│    │    └── When to Use semanage+restorecon vs chcon
│    │
│    ├─── 11.4 SELinux Port Labels
│    │    ├── semanage port -l (list all port labels)
│    │    ├── semanage port -a -t type -p tcp PORT (add)
│    │    ├── semanage port -m (modify)
│    │    └── semanage port -d (delete)
│    │
│    ├─── 11.5 SELinux Booleans
│    │    ├── getsebool -a (list all)
│    │    ├── getsebool boolean_name (check one)
│    │    ├── setsebool boolean on/off (temporary)
│    │    ├── setsebool -P boolean on/off (persistent!)
│    │    └── semanage boolean -l (with descriptions)
│    │
│    ├─── 11.6 SSH Key-Based Authentication
│    │    ├── ssh-keygen (generate key pair)
│    │    ├── ssh-copy-id user@host (copy public key)
│    │    ├── ~/.ssh/authorized_keys
│    │    ├── Correct Permissions (700, 600)
│    │    └── Disabling Password Auth in sshd_config
│    │
│    └─── 11.7 Default File Permissions (umask)
│         ├── umask — View and Set
│         ├── File Default: 666 - umask
│         ├── Directory Default: 777 - umask
│         └── Persistent: ~/.bashrc or /etc/bashrc
│
└─── MODULE 12: EXAM PRACTICE
     │
     ├─── 12.1 Mock Exam 1 (Full 3-hour simulation)
     ├─── 12.2 Mock Exam 2 (Full 3-hour simulation)
     └─── 12.3 Pre-Reboot Checklist
          ├── mount -a (verify fstab)
          ├── systemctl is-enabled (all services)
          ├── firewall-cmd --list-all --permanent
          ├── restorecon -Rv (SELinux contexts)
          ├── setsebool -P (booleans persistent)
          ├── nmcli connection up (network)
          ├── systemctl get-default (boot target)
          └── REBOOT AND VERIFY EVERYTHING
```

---

## SEQUENTIAL STUDY ORDER (What to Study When)

### Phase A: Foundation (Weeks 1-2) ✅ MOSTLY DONE

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 1 | Introduction to Linux | Pre-Module | ✅ Done |
| 2 | Linux vs Unix, Kernel | Pre-Module | ✅ Done |
| 3 | Linux Distributions | Pre-Module | ✅ Done |
| 4 | Computer Languages & Virtualization | Pre-Module | ✅ Done |
| 5 | Shell Basics (terminal, commands, man pages, scripting intro) | Module 1.1 | ✅ Done |

### Phase B: Essential Tools (Weeks 3-4) ← YOU ARE HERE

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 6 | I/O Redirection (stdin, stdout, stderr, pipes, tee) | Module 1.2 | ⬜ Next |
| 7 | Grep & Regular Expressions | Module 1.3 | ⬜ |
| 8 | File & Text Management (vim, cp, mv, rm, mkdir, cat, sort, cut) | Module 1.4 | ⬜ |
| 9 | Hard Links & Soft Links | Module 1.5 | ⬜ |
| 10 | File Permissions (chmod, chown, ugo/rwx) | Module 1.6 | ⬜ |
| 11 | Archiving & Compression (tar, gzip, bzip2) | Module 1.7 | ⬜ |
| 12 | SSH & Remote Access | Module 1.8 | ⬜ |

### Phase C: Users, Groups & Permissions (Weeks 5-6)

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 13 | File System Hierarchy & Navigation | Module 2 | ⬜ |
| 14 | User Management (useradd, usermod, userdel) | Module 3.1 | ⬜ |
| 15 | Group Management (groupadd, gpasswd) | Module 3.2 | ⬜ |
| 16 | Password & Aging (passwd, chage) | Module 3.3 | ⬜ |
| 17 | Special Permissions (SUID, SGID, Sticky) | Module 3.5 | ⬜ |
| 18 | Default Permissions (umask) | Module 3.6 | ⬜ |
| 19 | Privileged Access (sudo, visudo) | Module 3.7 | ⬜ |

### Phase D: Running Systems (Weeks 7-8)

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 20 | Boot, Reboot, Shutdown | Module 4.1 | ⬜ |
| 21 | Systemd Targets | Module 4.2 | ⬜ |
| 22 | Interrupt Boot / Password Recovery | Module 4.3 | ⬜ |
| 23 | Process Management (ps, top, kill, jobs) | Module 4.4 | ⬜ |
| 24 | Process Scheduling (nice, renice) | Module 4.5 | ⬜ |
| 25 | Tuning Profiles (tuned-adm) | Module 4.6 | ⬜ |
| 26 | System Logging (rsyslog, journalctl) | Module 4.7-4.8 | ⬜ |
| 27 | Service Management (systemctl) | Module 4.9 | ⬜ |

### Phase E: Software & Scripting (Weeks 9-10)

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 28 | RPM & DNF Package Management | Module 5.1-5.2 | ⬜ |
| 29 | Repository Configuration | Module 5.3 | ⬜ |
| 30 | Flatpak Management | Module 5.4 | ⬜ |
| 31 | Shell Scripting — Variables & Input | Module 6.1 | ⬜ |
| 32 | Shell Scripting — Conditionals (if, test, case) | Module 6.2 | ⬜ |
| 33 | Shell Scripting — Loops (for, while) | Module 6.3 | ⬜ |
| 34 | Shell Scripting — Command Output Processing | Module 6.4 | ⬜ |

### Phase F: Storage & File Systems (Weeks 11-13)

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 35 | Storage Concepts & Block Devices | Module 7.1 | ⬜ |
| 36 | GPT Partitioning (fdisk, gdisk, parted) | Module 7.2 | ⬜ |
| 37 | LVM — Physical Volumes | Module 7.3 | ⬜ |
| 38 | LVM — Volume Groups | Module 7.4 | ⬜ |
| 39 | LVM — Logical Volumes | Module 7.5 | ⬜ |
| 40 | Extending Logical Volumes | Module 7.6 | ⬜ |
| 41 | Swap Management | Module 7.7 | ⬜ |
| 42 | Creating File Systems (ext4, XFS, VFAT) | Module 8.1 | ⬜ |
| 43 | Mounting & fstab (UUID, LABEL) | Module 8.2 | ⬜ |
| 44 | NFS (Network File System) | Module 8.3 | ⬜ |
| 45 | Autofs (Auto-mounting) | Module 8.4 | ⬜ |

### Phase G: Networking (Weeks 14-15)

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 46 | Network Concepts | Module 9.1 | ⬜ |
| 47 | IPv4 Configuration (nmcli) | Module 9.2 | ⬜ |
| 48 | IPv6 Configuration | Module 9.3 | ⬜ |
| 49 | Hostname & DNS Resolution | Module 9.4 | ⬜ |
| 50 | Firewalld Configuration | Module 9.6 | ⬜ |

### Phase H: Deployment & Maintenance (Weeks 15-16)

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 51 | Task Scheduling — cron & at | Module 10.1-10.2 | ⬜ |
| 52 | Systemd Timer Units | Module 10.3 | ⬜ |
| 53 | Time Services (Chrony/NTP) | Module 10.4 | ⬜ |
| 54 | Bootloader (GRUB2, grubby) | Module 10.5 | ⬜ |

### Phase I: Security & SELinux (Weeks 17-18)

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 55 | SELinux Concepts & Modes | Module 11.1 | ⬜ |
| 56 | SELinux Contexts (ls -Z, ps -Z) | Module 11.2 | ⬜ |
| 57 | Managing & Restoring Contexts | Module 11.3 | ⬜ |
| 58 | SELinux Port Labels | Module 11.4 | ⬜ |
| 59 | SELinux Booleans | Module 11.5 | ⬜ |
| 60 | SSH Key-Based Authentication | Module 11.6 | ⬜ |

### Phase J: Exam Preparation (Weeks 19-20)

| # | Topic | Module | Status |
|---|-------|--------|--------|
| 61 | Mock Exam 1 (full simulation) | Module 12.1 | ⬜ |
| 62 | Review Weak Areas | — | ⬜ |
| 63 | Mock Exam 2 (full simulation) | Module 12.2 | ⬜ |
| 64 | Pre-Reboot Checklist Practice | Module 12.3 | ⬜ |

---

## YOUR NEXT STEP

You have completed **Shell Basics (Module 1.1)**. Your next topic is:

```
→ Module 1.2: I/O Redirection
  ├── File Descriptors (stdin, stdout, stderr)
  ├── Output Redirection (>, >>)
  ├── Error Redirection (2>, 2>>)
  ├── Combined Redirection (&>, 2>&1)
  ├── Input Redirection (<, <<, <<<)
  ├── /dev/null
  ├── Pipes (|)
  └── tee Command
```

---

## EXAM DAY GOLDEN RULES

1. **Read every question twice** — exact hostnames, IPs, paths matter.
2. **Easy tasks first** — score quick points, then tackle hard ones.
3. **Test EVERYTHING** — `mount -a`, `systemctl restart`, verify.
4. **REBOOT before submitting** — verify all configs survive reboot.
5. **Use man pages** — they're your ONLY reference. Practice `/search` in man.
6. **`--permanent` for firewalld** — then `--reload`.
7. **`setsebool -P`** — the `-P` makes it persistent.
8. **fstab by UUID** — never use /dev/sdX (can change after reboot).
9. **`restorecon -Rv`** — after any file context change.
10. **`systemctl enable`** — for every service that must start at boot.

---

> **Last Updated:** August 2026  
> **Source:** Official Red Hat EX200 objectives (redhat.com) + RHEL 10 documentation
