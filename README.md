# FakeHoneypot

A simple Python-based honeypot that simulates a fake SSH server on Windows. It listens for incoming connections, captures fake login attempts (IP, username, password), and logs them for analysis.

## Objective

Detect potential attackers by simulating a vulnerable SSH service, and log their activities without granting actual access.

---

## How It Works

- Listens on port `2222` (not the real SSH port 22, for safety)
- Accepts fake login credentials via raw socket
- Logs the attacker's:
  - IP address
  - Username and password attempt
  - Timestamp

---

## Project Structure

