# osquery
 
## Installation
Download the RPM package from the repository
```bash
cd ~
wget https://github.com/JakePeralta7/osquery/blob/main/osquery-5.7.0-1.linux.x86_64.rpm
```
Install osquery and delete the installation file
```bash
rpm -i osquery-5.7.0-1.linux.x86_64.rpm
rm -f osquery-5.7.0-1.linux.x86_64.rpm
```

## Usage
### Enter the osquery interface
You can enter a shell-like interface where you can your queries using `osqueryi`

### Executing single query
```bash
osqueryi '<query>' --json
```

### Examples
```bash
osqueryi 'SELECT * FROM users' --json
osqueryi 'SELECT * FROM system_info' --json
osqueryi "SELECT * FROM logged_in_users WHERE type='user'" --json
```