---
external help file: ACMESharp.POSH.dll-help.xml
online version: 
schema: 2.0.0
---

# Disable-ACMEExtensionModule

## SYNOPSIS

## SYNTAX

```
Disable-ACMEExtensionModule [-ModuleName] <String> [[-ModuleVersion] <String>] [[-AcmeVersion] <String>]
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
Required, the name of the PowerShell module that is an ACMESharp Extension Module.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ModuleVersion
An optional version spec, useful if multiple version of the target Extension Module
are installed.

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

### -AcmeVersion
An optional version spec, useful if multiple versions of the core ACMESharp module is installed,
this will specify which module installation will be targeted for enabling the module.

The spec can be an exact version string or a \`-like\` pattern to be matched.

```yaml
Type: String
Parameter Sets: (All)
Aliases: 

Required: False
Position: 3
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

