# Port Scanner

A small, interactive TCP port scanner written in Python. It checks whether selected TCP ports accept a connection and displays a known service label when one is available.

## Requirements

- Python 3.7 or later
- No third-party packages

## Run

From the project directory, start the interactive menu with:

```bash
python main.py
```

On Windows, you can also use:

```powershell
py main.py
```

## Usage

Choose an option from the menu:

1. **Scan single port** — enter an IPv4 address and one port number.
2. **Scan multiple ports** — enter an IPv4 address and a comma-separated list of port numbers, such as `21,22,80`.
3. **Scan common ports** — scan the ports listed in the built-in service map.
4. **Exit**

Ports must be between 1 and 65535. Results show each port as open or closed; ports not in the service map are labeled `Unknown`. The scanner uses a one-second connection timeout per port.

## Scope and permission

Only scan systems and networks that you own or have explicit permission to test. Port scans can trigger security alerts or violate network policies.
