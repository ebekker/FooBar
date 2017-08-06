---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Update-ACMECertificate

## SYNOPSIS
Updates the status and details of a Certificate stored in the Vault.

## SYNTAX

### Default (Default)
```
Update-ACMECertificate [-CertificateRef] <String> [-UseBaseUri] [-Repeat] [-NewAlias <String>]
 [-Label <String>] [-Memo <String>] [-VaultProfile <String>] [-PkiTool <String>]
```

### LocalOnly
```
Update-ACMECertificate [-CertificateRef] <String> [-LocalOnly] [-NewAlias <String>] [-Label <String>]
 [-Memo <String>] [-VaultProfile <String>] [-PkiTool <String>]
```

## DESCRIPTION
Use this cmdlet to update characteristics of an Identifier that are defined locally, such as the Alias or Label.

Also use this cmdlet to refresh the state and status of a Certificate including retrieving the certificate and intermediate signing certificate from the associated ACME CA Server.

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

### -UseBaseUri
Overrides the base URI associated with the target Registration and used for subsequent communication with the associated ACME CA Server.

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

### -Repeat
When specified, this flag instructs the cmdlet to repeat the retrieval of the issued certificate and related artifacts (e.g.
intermediate signing cert).

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
Indicates that updates should be performed locally only, and no attempt should be made to retrieve the current status from the ACME CA Server.

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
Optionally, set or update the human-friendly label to assigned to the Certificate for easy recognition.

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
Optionall, set or update the arbitrary text field used to capture any notes or details associated with the Certificate.

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

[New-Certificate]()

[Get-Certificate]()

[Submit-Certificate]()

