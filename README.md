## 📦 Week 2: Linux Basics – User & SSH Management

### ✅ Day 1 Task:
> **Create a user, assign to a group, give sudo, and restrict SSH access**

### 🔧 Tasks Performed:

- Created a user: `devops_user`
- Created a group: `devops_team`
- Added user to group: `devops_team`
- Set user password
- Granted sudo privileges
- Created another user: `mustansar_maqsood`
- Restricted SSH login using `/etc/ssh/sshd_config`

### 🧠 Key Concepts Learned:

- Linux user management via `/etc/passwd` and `/etc/group`
- Role of groups in access control
- Giving and controlling sudo access
- SSH security best practices: `AllowUsers` directive

### 🧪 Commands Used:

```bash
sudo adduser devops_user
sudo addgroup devops_team
sudo usermod -aG devops_team devops_user
sudo usermod -aG sudo devops_user
sudo adduser mustansar_maqsood
sudo nano /etc/ssh/sshd_config
