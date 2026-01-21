# Cerebrus

A Python network scanner similar to nmap. Scans ports, discovers hosts, and detects services

## Requirements

Python 3.6+ (no external dependencies)

## Usage

```
python cerebrus.py <target> [options]
```

## Examples

```
python cerebrus.py 192.168.1.1
python cerebrus.py 192.168.1.1 -p 22,80,443
python cerebrus.py 192.168.1.1 -p 1-1000
python cerebrus.py 192.168.1.0/24 -d
python cerebrus.py 192.168.1.1 -sV
python cerebrus.py 192.168.1.1 -o results.txt
```

## Options

```
target              Target IP, hostname, or CIDR range
-p, --ports         Ports to scan (22,80 or 1-1000)
-d, --discover      Host discovery only
-sV, --version      Detect service versions
--top-ports N       Scan top N common ports
--all-ports         Scan all 65535 ports
-t, --threads       Number of threads (default 100)
--timeout           Timeout in seconds (default 1.0)
-o, --output        Save results to file
--no-banner         Skip banner display
```

## Legal

Only scan networks you own or have permission to test.

