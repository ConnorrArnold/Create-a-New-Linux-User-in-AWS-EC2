# Create a New Linux User in AWS EC2

## Objective

Created a new Linux user account on an AWS EC2 Ubuntu 24.04.4 LTS instance and granted it administrative privileges. The project focused on understanding user management, UID/GID assignment, and privilege escalation through the sudo group. This is a foundational sysadmin skill for managing multi-user Linux environments.

### Skills Learned

- Linux user creation with adduser
- UID/GID assignment and group management
- Setting and updating user passwords
- Populating user metadata (full name, contact info)
- Granting sudo privileges with usermod

### Tools Used

- AWS EC2
- Ubuntu 24.04.4 LTS
- adduser command
- usermod command
- OpenSSH (terminal access)

## Steps
1. Connected to the EC2 instance via SSH
2. Ran sudo adduser student to create the new user
3. Set and confirmed a password for the student account
4. Entered user metadata (name, room number, phone numbers) when prompted
5. Confirmed the information was correct at the [Y/n] prompt
6. Ran sudo usermod -aG sudo student to add the user to the sudo group, granting administrative privileges
