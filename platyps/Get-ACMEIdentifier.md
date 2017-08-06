---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-ACMEIdentifier

## SYNOPSIS
Lists all, or retrieves details for, Identifiers submitted for verification.

## SYNTAX

### List (Default)
```
Get-ACMEIdentifier [-VaultProfile <String>]
```

### Get
```
Get-ACMEIdentifier [-IdentifierRef] <String> [-VaultProfile <String>]
```

## DESCRIPTION
Use this cmdlet to list all of the Identifier that have been previously defined and submitted to the ACME CA Server of the current Vault.
You also use this cmdlet to specify specific Identifier references (ID or alias) to retrieve more specific details as they are captured in the Vault.

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -IdentifierRef
A reference (ID or alias) to a previously defined Identifier submitted to the ACME CA Server for verification.

```yaml
Type: String
Parameter Sets: Get
Aliases: Ref

Required: True
Position: 0
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

[New-Identifier]()

[Update-Identifier]()

