---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Set-ACMEProxy

## SYNOPSIS

## SYNTAX

### UseSystem (Default)
```
Set-ACMEProxy [-UseSystem] [-VaultProfile <String>]
```

### UseNoProxy
```
Set-ACMEProxy [-UseNoProxy] [-VaultProfile <String>]
```

### UseProxyNoCred
```
Set-ACMEProxy -UseProxy <String> [-VaultProfile <String>]
```

### UseProxyDefCred
```
Set-ACMEProxy -UseProxy <String> [-DefaultCredential] [-VaultProfile <String>]
```

### UseProxyWithCred
```
Set-ACMEProxy -UseProxy <String> -Credential <PSCredential> [-VaultProfile <String>]
```

## DESCRIPTION
{{Fill in the Description}}

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -UseSystem
{{Fill UseSystem Description}}

```yaml
Type: SwitchParameter
Parameter Sets: UseSystem
Aliases: 

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseNoProxy
{{Fill UseNoProxy Description}}

```yaml
Type: SwitchParameter
Parameter Sets: UseNoProxy
Aliases: 

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -UseProxy
{{Fill UseProxy Description}}

```yaml
Type: String
Parameter Sets: UseProxyNoCred, UseProxyDefCred, UseProxyWithCred
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -DefaultCredential
{{Fill DefaultCredential Description}}

```yaml
Type: SwitchParameter
Parameter Sets: UseProxyDefCred
Aliases: 

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Credential
{{Fill Credential Description}}

```yaml
Type: PSCredential
Parameter Sets: UseProxyWithCred
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -VaultProfile
{{Fill VaultProfile Description}}

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

