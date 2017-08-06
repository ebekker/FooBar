---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Set-ACMEVault

## SYNOPSIS

## SYNTAX

### BaseService (Default)
```
Set-ACMEVault [-BaseService <String>] [-Signer <String>] [-PkiTool <String>] [-Force <Boolean>]
 [-Alias <String>] [-Label <String>] [-Memo <String>] [-VaultProfile <String>]
```

### BaseUri
```
Set-ACMEVault -BaseUri <String> [-Signer <String>] [-PkiTool <String>] [-Force <Boolean>] [-Alias <String>]
 [-Label <String>] [-Memo <String>] [-VaultProfile <String>]
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

### -BaseService
{{Fill BaseService Description}}

```yaml
Type: String
Parameter Sets: BaseService
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -BaseUri
{{Fill BaseUri Description}}

```yaml
Type: String
Parameter Sets: BaseUri
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Signer
{{Fill Signer Description}}

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

### -PkiTool
Specifies a PKI tool provider (i.e.
CertificateProvider) to be used by default in all subsequent operations against this vault.
In most cases this can be overridden on a call-by-call basis but typically, all PKI-related operations should be performed by a single PKI Tool provider because of the internal workings of the provider and interdependencies of the operations.
Such operations include private key generation, CSR generation and certificate importing and exporting.
If left unspecified a default PKI tool provider will be used.

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

### -Force
{{Fill Force Description}}

```yaml
Type: Boolean
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -Alias
{{Fill Alias Description}}

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

## NOTES

## RELATED LINKS

