# Note2Link Desktop Client Port Settings Guide

This document will guide you on how to configure the port settings of the Note2Link desktop client to fully utilize acceleration and synchronization features.

## Port Settings Overview

The Note2Link desktop client provides two proxy port settings:
1. **System Proxy Port**: For system applications (such as note-taking software)
2. **Browser Proxy Port**: For use with browser extensions

![Note2Link Port Settings Interface](./assets/images/port_settings_en-US.png)

## System Proxy Port

The system proxy port is used to automatically set up system proxy, enabling acceleration and synchronization features for note-taking software.

- Default port: **35777**
- Function: Note2Link client automatically sets up system proxy, no manual configuration needed
- Application scenarios: Acceleration and synchronization for various note-taking software

> **Tip**: If the default port conflicts with other applications, you can modify it to another unused port.

## Browser Proxy Port

The browser proxy port needs to be used with browser extensions. Here are the configuration steps:

### Recommended: Proxy SwitchyOmega 3 (ZeroOmega)

As browsers gradually phase out Manifest V2 support, we recommend using **Proxy SwitchyOmega 3 (ZeroOmega)**, abbreviated as **ZeroOmega**, which is a modified version of Proxy SwitchyOmega that supports the new Manifest V3.

#### ZeroOmega Configuration Steps:

1. Install **Proxy SwitchyOmega 3 (ZeroOmega)** from the browser extension store
2. Open the extension settings interface
3. Create a new proxy configuration with the following settings:
   - Proxy protocol: **SOCKS5**
   - Proxy server: **127.0.0.1**
   - Proxy port: **35778** (Note2Link default browser proxy port)

![ZeroOmega Settings Interface](./assets/images/zeroomega_settings_en-US.png)

4. Save and apply the configuration

#### Usage Method:

1. Click on the ZeroOmega icon in the browser toolbar
2. Select the Note2Link proxy configuration you created
3. Your browser is now accelerated through Note2Link

> **Note**: For users migrating from SwitchyOmega, ZeroOmega's management interface is almost identical, allowing for seamless replacement.

## Common Issues

### What if the port is already in use?

If the default port is being used by another application, you can modify it to another unused port in the Note2Link settings, then update your browser extension configuration accordingly.

### Why is ZeroOmega recommended?

The original Proxy SwitchyOmega is based on Manifest V2, which browsers are gradually ceasing to support. Proxy SwitchyOmega 3 (ZeroOmega) supports Manifest V3, ensuring your browser extension can be used long-term.

## Summary

By correctly configuring Note2Link's port settings and browser extension, you can fully utilize the acceleration and synchronization features provided by Note2Link, enhancing the experience of your note-taking software and browser. These settings will help you manage and access your notes more effectively, whether in local applications or during web browsing.
