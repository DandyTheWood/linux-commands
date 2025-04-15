
# Linux Commands Reference

## 1. File & Directory Management

| **Command** | **Use**                             | **Common Parameters**                                |
|-------------|--------------------------------------|-------------------------------------------------------|
| `ls`        | List directory contents              | `-l`, `-a`, `-h`, `-R`, `-t`                          |
| `cp`        | Copy files and directories           | `-r`, `-v`, `-u`, `-p`                                |
| `mv`        | Move/rename files and directories    | `-v`, `-n`, `-u`                                      |
| `rm`        | Remove files or directories          | `-r`, `-f`, `-v`                                      |
| `mkdir`     | Create directories                   | `-p`, `-v`                                            |
| `rmdir`     | Remove empty directories             | `--ignore-fail-on-non-empty`                         |
| `touch`     | Create empty files / update timestamps |                                                     |
| `stat`      | Display file info                    | `-c`, `--format`                                     |
| `file`      | Determine file type                  | `-i`, `-b`                                            |
| `basename`  | Strip directory and suffix from file |                                                       |
| `dirname`   | Extract directory part of path       |                                                       |

## 2. Text Processing

| **Command** | **Use**                            | **Common Parameters**                                |
|-------------|-------------------------------------|-------------------------------------------------------|
| `cat`       | Concatenate and display files       | `-n`, `-b`, `-A`                                     |
| `less`      | View files one page at a time       | `/` (search), `n`, `q`                              |
| `head`      | Show first lines                    | `-n`                                                 |
| `tail`      | Show last lines                     | `-n`, `-f`                                           |
| `cut`       | Cut sections of each line           | `-d`, `-f`, `-c`                                     |
| `awk`       | Pattern scanning and processing     | `-F`, `-v`, `'pattern { action }'`                   |
| `sed`       | Stream editor                       | `-e`, `-i`, `s/old/new/`, `-n`                       |
| `sort`      | Sort lines of text                  | `-n`, `-r`, `-k`, `-u`, `-t`                         |
| `uniq`      | Filter duplicate lines              | `-c`, `-d`, `-u`                                     |
| `wc`        | Count words/lines/bytes             | `-l`, `-w`, `-c`                                     |
| `tr`        | Translate/delete characters         | `-d`, `-s`, `a-z A-Z`                                |
| `nl`        | Number lines                        | `-b`, `-n`, `-s`                                     |

## 3. System Information & Monitoring

| **Command**    | **Use**                               | **Common Parameters**                             |
|----------------|----------------------------------------|----------------------------------------------------|
| `uname`        | Show system info                      | `-a`, `-r`, `-s`, `-m`                             |
| `uptime`       | Show how long system is running       | —                                                  |
| `top`          | Live process monitoring               | —                                                  |
| `htop`         | Interactive top                       | `-d`, `-u`                                         |
| `vmstat`       | Virtual memory statistics             | `interval`, `count`                               |
| `iostat`       | I/O and CPU statistics                | `-x`, `-d`                                         |
| `free`         | Memory usage                          | `-h`, `-m`, `-g`                                   |
| `df`           | Disk space                            | `-h`, `-T`, `--total`                              |
| `du`           | Directory/file space usage            | `-h`, `-s`, `--max-depth`                          |
| `who`          | Show who is logged in                 | —                                                  |
| `id`           | Show user ID info                     | `-u`, `-g`, `-n`                                   |
| `which`        | Show path of command binary           | `which <command>`                                 |
| `whereis`      | Locate binary, source, man pages      | `-b`, `-s`, `-m`                                   |
| `hostname`     | Display/set system hostname           | `-I`, `-f`, `-s`                                   |

## 4. Networking & Internet

| **Command**  | **Use**                                | **Common Parameters**                              |
|--------------|-----------------------------------------|-----------------------------------------------------|
| `ping`       | Check connectivity                      | `-c`, `-i`, `-t`                                    |
| `traceroute` | Trace network hops                      | `-n`, `-m`, `-w`                                    |
| `dig`        | DNS queries                             | `+short`, `ANY`, `MX`, `NS`                         |
| `nslookup`   | DNS lookup                              | —                                                   |
| `host`       | DNS lookup                              | —                                                   |
| `wget`       | Download files                          | `-c`, `-r`, `-O`, `--limit-rate`                    |
| `curl`       | Transfer data with URLs                 | `-O`, `-L`, `-d`, `-H`                              |
| `scp`        | Secure copy                             | `-r`, `-P`, `-i`                                    |
| `rsync`      | Sync files                              | `-avz`, `--delete`, `--progress`                    |
| `ssh`        | Remote login                            | `-p`, `-i`, `-N`, `-T`                              |
| `netstat`    | Show network connections                | `-tuln`, `-p`, `-r`                                 |
| `ss`         | Show socket stats (modern netstat)      | `-tuln`, `-p`, `-s`                                 |
| `ifconfig`   | Show or configure network interfaces    | `up`, `down`, `inet`                               |
| `ip`         | Manage IP and network                   | `ip a`, `ip r`, `ip link`                          |
| `nmap`       | Network scanner                         | `-sS`, `-p`, `-A`, `-O`, `-T4`                      |

## 5. Package Management

| **Command**    | **Use**                                 | **Common Parameters**                               |
|----------------|------------------------------------------|------------------------------------------------------|
| `apt`          | Debian/Ubuntu package manager            | `update`, `upgrade`, `install`, `remove`, `search`   |
| `dpkg`         | Debian package tool                      | `-i`, `-r`, `-l`, `-S`                                |
| `yum`          | RHEL/CentOS package manager              | `install`, `remove`, `update`, `search`, `info`      |
| `dnf`          | Modern Fedora package manager            | Same as `yum`                                        |
| `pacman`       | Arch Linux package manager               | `-S`, `-R`, `-Ss`, `-Qi`                              |
| `snap`         | Snap package manager                     | `install`, `remove`, `list`, `refresh`               |
| `flatpak`      | Flatpak package manager                  | `install`, `run`, `list`, `update`                   |

## 6. Development Tools

| **Command** | **Use**                             | **Common Parameters**                                 |
|-------------|--------------------------------------|--------------------------------------------------------|
| `gcc`       | GNU C compiler                       | `-o`, `-Wall`, `-g`, `-O2`                             |
| `make`      | Build automation                     | `-f`, `-j`, `--dry-run`                                |
| `gdb`       | GNU debugger                         | `-q`, `-ex`, `--args`                                  |
| `strace`    | Trace system calls                   | `-p`, `-e`, `-f`                                       |
| `lsof`      | List open files                      | `-i`, `+D`, `-u`, `-p`                                 |
| `time`      | Measure execution time               | `time <command>`                                      |
| `valgrind`  | Memory debugger                      | `--leak-check`, `--tool=memcheck`                     |

### Additional Commands

#### File & Directory Management
| `tree`       | Display directory tree                | `-L`, `-d`, `-a`, `--noreport`                       |
| `readlink`   | Resolve symbolic links                | `-f`, `-e`, `-n`                                     |
| `realpath`   | Show absolute path                    | `--relative-to`, `--canonicalize-existing`           |
| `find`       | Search files in directory hierarchy   | `-name`, `-type`, `-exec`, `-mtime`, `-size`         |
| `xargs`      | Build and execute command lines       | `-n`, `-d`, `-0`, `-I{}`                              |

#### Text Processing
| `paste`      | Merge lines of files                  | `-d`, `-s`                                           |
| `rev`        | Reverse lines                         | —                                                   |
| `column`     | Format output into columns            | `-t`, `-s`, `-n`                                     |
| `yes`        | Output a string repeatedly            | `yes [STRING]`                                      |
| `split`      | Split file into pieces                | `-b`, `-l`, `-d`, `--additional-suffix`              |

#### System Information & Monitoring
| `dmesg`      | Print kernel ring buffer messages     | `-T`, `--level`, `--color`                          |
| `uptime`     | Show system uptime                    | —                                                   |
| `whoami`     | Show current username                 | —                                                   |
| `groups`     | Show group memberships                | —                                                   |
| `watch`      | Periodically run a command            | `-n`, `-d`, `-t`                                     |

#### Networking & Internet
| `telnet`     | Terminal-based network protocol tool  | `host`, `port`                                      |
| `ftp`        | File transfer protocol client         | `open`, `put`, `get`, `bye`                         |
| `nc`         | Netcat - arbitrary TCP/UDP tool       | `-l`, `-p`, `-v`, `-z`, `-n`                         |
| `hostnamectl`| Manage hostname and system info       | `status`, `set-hostname`                            |
| `ipcalc`     | Display IP information from CIDR      | —                                                   |

#### Package Management
| `apt-cache`  | Get package info (Debian/Ubuntu)      | `search`, `show`, `depends`, `rdepends`             |
| `rpm`        | Red Hat package manager               | `-i`, `-q`, `-e`, `-V`                               |
| `zypper`     | openSUSE package manager              | `install`, `remove`, `info`, `update`               |
| `brew`       | macOS/Linux Homebrew                  | `install`, `search`, `update`, `list`               |

#### Development Tools
| `ldd`        | Show shared libraries                 | `ldd <binary>`                                      |
| `nm`         | List symbols from object files        | `-g`, `-n`, `-u`                                     |
| `objdump`    | Display information from binary files | `-d`, `-x`, `-s`, `-t`                               |
| `diff`       | Compare file differences              | `-u`, `-y`, `--side-by-side`                         |
| `patch`      | Apply a diff patch                    | `-p1`, `-N`, `--dry-run`                             |
