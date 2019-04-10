# Linux mutt Command
-------------------
### Command Introduction (命令介绍)
> **mutt - The Mutt Mail User Agent**
### Command Format and Options (命令格式和选项)
```
Mutt 1.5.21 (2010-09-15)
```
### Command Example (命令范例)
```

  mutt

  Command-line email client.

  - Open the specified mailbox:
    mutt -f mailbox

  - Send an email and specify a subject and a cc recipient:
    mutt -s subject -c cc@example.com recipient@example.com

  - Send an email with files attached:
    mutt -a file1 file2 -- recipient@example.com

  - Specify a file to include as the message body:
    mutt -i file recipient@example.com

  - Specify a draft file containing the header and the body of the message, in RFC 5322 format:
    mutt -H file recipient@example.com


```
