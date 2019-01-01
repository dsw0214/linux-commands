# Linux ssh Command
### Command Introduction (命令介绍)
-------------------
> **
     ssh — OpenSSH SSH client (remote login program)
                   CertificateFile
                   ChallengeResponseAuthentication
                   CheckHostIP
                   Cipher
                   Ciphers
                   ClearAllForwardings
                   Compression
                   CompressionLevel
                   ConnectionAttempts
                   ConnectTimeout
                   ControlMaster
                   ControlPath
                   ControlPersist
                   DynamicForward
                   EscapeChar
                   ExitOnForwardFailure
                   FingerprintHash
                   ForwardAgent
                   ForwardX11
                   ForwardX11Timeout
                   ForwardX11Trusted
                   GatewayPorts
                   GlobalKnownHostsFile
                   GSSAPIAuthentication
                   GSSAPIKeyExchange
                   GSSAPIClientIdentity
                   GSSAPIDelegateCredentials
                   GSSAPIRenewalForcesRekey
                   GSSAPITrustDns
                   GSSAPIKexAlgorithms
                   HashKnownHosts
                   Host
                   HostbasedAuthentication
                   HostbasedKeyTypes
                   HostKeyAlgorithms
                   HostKeyAlias
                   HostName
                   IdentitiesOnly
                   IdentityAgent
                   IdentityFile
                   Include
                   IPQoS
                   KbdInteractiveAuthentication
                   KbdInteractiveDevices
                   KexAlgorithms
                   LocalCommand
                   LocalForward
                   LogLevel
                   MACs
                   Match
                   NoHostAuthenticationForLocalhost
                   NumberOfPasswordPrompts
                   PasswordAuthentication
                   PermitLocalCommand
                   PKCS11Provider
                   Port
                   PreferredAuthentications
                   Protocol
                   ProxyCommand
                   ProxyJump
                   ProxyUseFdpass
                   PubkeyAcceptedKeyTypes
                   PubkeyAuthentication
                   RekeyLimit
                   RemoteForward
                   RequestTTY
                   RhostsRSAAuthentication
                   RSAAuthentication
                   SendEnv
                   ServerAliveInterval
                   ServerAliveCountMax
                   StreamLocalBindMask
                   StreamLocalBindUnlink
                   StrictHostKeyChecking
                   TCPKeepAlive
                   Tunnel
                   TunnelDevice
                   UpdateHostKeys
                   UsePrivilegedPort
                   User
                   UserKnownHostsFile
                   VerifyHostKeyDNS
                   VisualHostKey
                   XAuthLocation
**

### Command Format and Options (命令格式和选项)
```
#ssh 
usage: ssh [-1246AaCfgKkMNnqsTtVvXxYy] [-b bind_address] [-c cipher_spec]
           [-D [bind_address:]port] [-E log_file] [-e escape_char]
           [-F configfile] [-I pkcs11] [-i identity_file]
           [-L [bind_address:]port:host:hostport] [-l login_name] [-m mac_spec]
           [-O ctl_cmd] [-o option] [-p port]
           [-Q cipher | cipher-auth | mac | kex | key]
           [-R [bind_address:]port:host:hostport] [-S ctl_path] [-W host:port]
           [-w local_tun[:remote_tun]] [user@]hostname [command]
```
### Command Example (命令范例)
-------------------
**

Secure Shell is a protocol used to securely log onto remote systems.
It can be used for logging or executing commands on a remote server.
**

- Connect to a remote server:

  ` ssh username@remote_host`

- Connect to a remote server with a specific identity (private key):

  ` ssh -i path/to/key_file username@remote_host`

- Connect to a remote server using a specific port:

  ` ssh username@remote_host -p 2222`

- Run a command on a remote server:

  ` ssh remote_host command -with -flags`

- SSH tunneling: Dynamic port forwarding (SOCKS proxy on localhost:9999):

  ` ssh -D 9999 -C username@remote_host`

- SSH tunneling: Forward a specific port (localhost:9999 to slashdot.org:80) along with disabling pseudo-[t]ty allocation and executio[n] of remote commands:

  ` ssh -L 9999:slashdot.org:80 -N -T username@remote_host`

- SSH jumping: Connect through a jumphost to a remote server (Multiple jump hops may be specified separated by comma characters):

  ` ssh -J username@jump_host username@remote_host`

- Agent forwarding: Forward the authentication information to the remote machine (see `man ssh_config` for available options):

  ` ssh -A username@remote_host`
