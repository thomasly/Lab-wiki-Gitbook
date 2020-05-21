# Connect to HPCs

The IP addresses of the DGX-Lei workstation and the Hunter DLS Server are:

| HPC | IP address |
| :--- | :--- |
| DGX | 146.95.214.135 |
| DLS | 146.95.128.169 |

### 1. Inside the Hunter Network

You can use `ssh` via a computer inside the Hunter network to access it:

```text
ssh yourname@IPaddress
```

### 2. Outside the Hunter Network

If you want to access the HPCs outside the Hunter network, a two-step login is needed:

1. Use `ssh` to connect to eniac from anywhere using your [eniac account](http://web.archive.org/web/20190726111206/http://www.geography.hunter.cuny.edu/tbw/CS.Linux.Lab.FAQ/department_of_computer_science.faq.htm):

   ```text
   ssh yourname@eniac.cs.hunter.cuny.edu
   ```

   \(Note: Eniac account should be claimed by logging in from one of the Computer Science Linux Labs \(1001B or 1001C\), or it will be deleted\)

2. After connecting to eniac, use `ssh` to connect to the HPCs:

   ```text
   ssh yourname@IPaddress
   ```
