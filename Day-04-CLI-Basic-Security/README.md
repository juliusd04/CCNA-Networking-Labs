# Day 4 - Cisco CLI and Basic Security Configuration

## Overview

In this lab, I used Cisco Packet Tracer to practice configuring basic security settings on Cisco routers and switches through the Command Line Interface (CLI). The objective was to become familiar with different Cisco IOS command modes, configure privileged access passwords, and learn how to view and save device configurations.

## Tools Used

- Cisco Packet Tracer
- Cisco IOS Command Line Interface
- Jeremy's IT Lab CCNA Course

## Lab Objectives

- Navigate between different Cisco IOS command modes.
- Configure passwords to protect privileged EXEC mode.
- Enable password encryption for supported configuration entries.
- View and verify device configurations.
- Save configuration changes to startup-config.
- Practice troubleshooting incorrect or incomplete CLI commands.

## Lab Activities

### 1. Navigating Cisco IOS Command Modes

I practiced accessing different command modes on Cisco switches and routers.

The main modes included:

- **User EXEC Mode (`SW1>`)** - Provides access to basic monitoring commands.
- **Privileged EXEC Mode (`SW1#`)** - Provides access to additional monitoring and administrative commands.
- **Global Configuration Mode (`SW1(config)#`)** - Allows changes to the device configuration.

I used commands such as:

```text
enable
configure terminal
exit
```

I also practiced using abbreviated commands, such as `conf t`.

### 2. Configuring Privileged Access Passwords

I practiced configuring and verifying privileged EXEC passwords using Cisco IOS.

The lab introduced two password configuration methods:

```text
enable password
enable secret
```

I learned that `enable secret` takes priority when both commands are configured.

The `enable secret` command stores a hashed password, while `enable password` can use weaker password storage methods.

### 3. Enabling Password Encryption

I configured password encryption using:

```text
service password-encryption
```

After enabling this setting, I viewed the running configuration to observe how the password appeared.

I learned that this command uses reversible Type 7 encoding for certain passwords, which helps prevent casual viewing but does not provide strong security.

### 4. Viewing Device Configurations

I used the following commands to examine device configurations:

```text
show running-config
show startup-config
```

The running configuration represents the device's active configuration, while the startup configuration contains the saved configuration used during startup.

I also practiced using:

```text
do show running-config
```

This allowed me to execute a privileged EXEC command while remaining in global configuration mode.

### 5. Saving Configuration Changes

I practiced saving device configurations using:

```text
write memory
```

And:

```text
copy running-config startup-config
```

Both commands allowed me to save the active configuration so it could be retained after a device restart.

I verified the saved configuration using:

```text
show startup-config
```

### 6. Troubleshooting CLI Commands

During the lab, I encountered errors when entering incomplete commands or using incorrect syntax.

For example, I initially entered an incorrect destination filename when attempting to copy the running configuration.

After correcting the command to:

```text
copy running-config startup-config
```

The device successfully saved the configuration and displayed an `[OK]` message.

This helped me become more comfortable identifying and correcting Cisco IOS command errors.

## Key Takeaways

- Cisco IOS uses different command modes for monitoring and configuration.
- Privileged EXEC mode can be protected using passwords.
- `enable secret` is preferred over `enable password` for privileged access.
- Type 7 password encryption is reversible and should not be considered strong protection.
- `show running-config` displays the active configuration.
- `show startup-config` displays the saved configuration.
- Configuration changes must be saved to persist after a restart.
- Understanding CLI syntax is important for configuring and troubleshooting network devices.

## Conclusion

This lab introduced me to basic Cisco IOS administration and security configuration. I gained hands-on experience navigating the CLI, configuring passwords, examining device settings, and saving configurations.

These skills provide a foundation for more advanced networking and cybersecurity tasks, including secure device management, network troubleshooting, and access control.
