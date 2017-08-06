---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Update-ACMERegistration

## SYNOPSIS

## SYNTAX

### Default (Default)
```
Update-ACMERegistration [-UseBaseUri] [-Contacts <String[]>] [-AcceptTos] [-NewAlias <String>]
 [-Label <String>] [-Memo <String>] [-VaultProfile <String>]
```

### LocalOnly
```
Update-ACMERegistration [-LocalOnly] [-NewAlias <String>] [-Label <String>] [-Memo <String>]
 [-VaultProfile <String>]
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

### -UseBaseUri
{{Fill UseBaseUri Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Default
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -LocalOnly
{{Fill LocalOnly Description}}

```yaml
Type: SwitchParameter
Parameter Sets: LocalOnly
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Contacts
{{Fill Contacts Description}}

```yaml
Type: String[]
Parameter Sets: Default
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AcceptTos
{{Fill AcceptTos Description}}

```yaml
Type: SwitchParameter
Parameter Sets: Default
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -NewAlias
Optionaly, set or update the unique alias assigned to the Certificate for future reference.
To remove the alias, use the empty string.

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
{{Fill Label Description}}

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
{{Fill Memo Description}}

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

### ACMESharp.AcmeRegistration

## NOTES

## RELATED LINKS

