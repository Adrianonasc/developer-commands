how check ip

```console
ipconfig
```

Inclusão de regra no firewall
```console
New-NetFirewallRule -DisplayName "WSL" -Direction Inbound  -InterfaceAlias "vEthernet (WSL (Hyper-V firewall))"  -Action Allow
```

