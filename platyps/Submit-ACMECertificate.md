---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Submit-ACMECertificate

## SYNOPSIS

## SYNTAX

```
Submit-ACMECertificate [-CertificateRef] <String> [-Force] [-VaultProfile <String>] [-PkiTool <String>]
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

### -CertificateRef
A reference (ID or alias) to a previously defined Certificate request.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Ref

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
{{Fill Force Description}}

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: False
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

### -PkiTool
Specifies a PKI tool provider (i.e.
CertificateProvider) to be used in all PKI related operations such as private key generation, CSR generation and certificate importing and exporting.
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

## INPUTS

## OUTPUTS

### ACMESharp.Vault.Model.CertificateInfo

## NOTES

## RELATED LINKS

