---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# New-ACMEIdentifier

## SYNOPSIS
Creates and submits a new Identifier to be verified to the ACME CA Server.

## SYNTAX

```
New-ACMEIdentifier [-Dns <String>] [-Alias <String>] [-Label <String>] [-Memo <String>]
 [-VaultProfile <String>]
```

## DESCRIPTION
Currently, the only Identifier type supported is the DNS type.

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -Dns
Specifies the DNS name to be submitted for verification.

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

### -Alias
An optional, unique alias to assign to the Identifier for future reference.

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

### -Label
An optional, human-friendly label to assign to the Identifier for easy recognition.

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

### -Memo
An optional, arbitrary text field to capture any notes or details associated with the Identifier.

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

### -VaultProfile
Specifies a Vault profile name that will resolve to the Vault instance to be used for all related operations and storage/retrieval of all related assets.

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

### ACMESharp.AuthorizationState

## NOTES

## RELATED LINKS

[Get-Identifier]()

[Update-Identifier]()

[Complete-Challenge]()

[Submit-Challenge]()

