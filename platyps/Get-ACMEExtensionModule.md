---
external help file: ACMESharp.POSH.dll-help.xml
online version: 
schema: 2.0.0
---

# Get-ACMEExtensionModule

## SYNOPSIS

## SYNTAX

```
Get-ACMEExtensionModule [[-ModuleName] <String>] [[-AcmeVersion] <String>]
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

### -ModuleName
Optional, the name of the PowerShell module that is an enabled ACMESharp Extension Module. 
If unspecified, then all enabled Extension Modules will be returned.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AcmeVersion
An optional version spec, useful if multiple versions of the core ACMESharp module is installed,
this will specify which module installation will be targeted for inspecting for enabled modules.

The spec can be an exact version string or a \`-like\` pattern to be matched.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 2
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

