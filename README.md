# Apt Force Upgrader Ultra 🚀

An advanced, high-performance automated system upgrade utility engineered for Debian/Ubuntu-based Linux distributions. This tool bypasses standard interactive friction by orchestrating `apt-get dist-upgrade` workflows through a robust, asynchronous background runner written in systems-level compiled code.

Built for system administrators, DevOps engineers, and power users who require absolute precision, raw terminal performance, and automated privilege escalation management.

---

## 🔥 Key Technical Specialties

*   **Asynchronous Background Runner:** Leverages compiled multi-threaded architecture (`pthread`, `epoll`) to decouple the live terminal UI from the underlying APT system processes.
*   **Elevated Automation Management:** Seamlessly handles user-provided privilege tokens (`sudo` integration) to execute full platform upgrades (`dist-upgrade`) without blocking or losing stream contexts.
*   **Zero-Lag Live Terminal Stream:** Implements real-time I/O multiplexing to pipe live APT processing metrics straight to the user display without context bottlenecks.
*   **Phased-Update Overrides:** Explicitly enforces `APT::Get::Always-Include-Phased-Updates=true` policy flag configurations natively to ensure no security updates are delayed by phased distribution policies.
*   **Self-Contained Executable Environment:** Built on native Linux syscalls and direct automotive dynamic linking dependencies (`glibc`), optimizing runtime efficiency and memory footprint.

---

## 🛠 Architectural Overview

The application relies on deep kernel-level primitives such as `epoll_create1`, `eventfd`, and `timerfd_settime` to run non-blocking processing event loops. Standard output formatting is backed by custom system tessellation models to ensure lightweight memory usage while handling highly intense diagnostic log parsing.

---

## 📥 Installation

Choose one of the following methods to install the binary on your Linux system:

### Method 1: Quick Install via Script
```bash
curl -sSL https://githubusercontent.com | bash
```

### Method 2: Manual Binary Installation
Download the latest pre-compiled binary from the Releases tab and execute:
```bash
sudo mv apt-force-upgrader-ultra /usr/local/bin/apt-force-upgrader
sudo chmod +x /usr/local/bin/apt-force-upgrader
```

---

## 🚀 Usage Commands

Run the utility with the appropriate flags based on your operational requirements:

### Standard Force Upgrade
Executes a complete distribution upgrade, overriding phased updates automatically:
```bash
apt-force-upgrader --run
```

### Unattended Daemon Mode
Runs the upgrader entirely in the background, suppressing interactive prompts while logging to a secure file:
```bash
apt-force-upgrader --daemon --log-path /var/log/apt_force_upgrader.log
```

### Check Version & System Footprint
```bash
apt-force-upgrader --version
```

---

## 📝 License
Distributed under the MIT License. See `LICENSE` for more information.
