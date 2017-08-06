---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Get-ACMECertificate

## SYNOPSIS
Gets the status and details of a Certificate stored in the Vault.

## SYNTAX

### List (Default)
```
Get-ACMECertificate [-VaultProfile <String>] [-PkiTool <String>]
```

### Get
```
Get-ACMECertificate [-CertificateRef] <String> [-ExportKeyPEM <String>] [-ExportCsrPEM <String>]
 [-ExportCertificatePEM <String>] [-ExportCertificateDER <String>] [-ExportIssuerPEM <String>]
 [-ExportIssuerDER <String>] [-ExportPkcs12 <String>] [-CertificatePassword <String>] [-Overwrite]
 [-VaultProfile <String>] [-PkiTool <String>]
```

## DESCRIPTION
This cmdlet retrieves the details of a Certificate defined in the Vault.
It is also used to export various artificates associated with the Certificate to various formats.

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
Parameter Sets: Get
Aliases: Ref

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportKeyPEM
Optionally, specifies a file path where the private key associated with the referenced Certificate will be saved in PEM format.

```yaml
Type: String
Parameter Sets: Get
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportCsrPEM
Optionally, specifies a file path where the CSR associated with the referenced Certificate will be saved in PEM format.

```yaml
Type: String
Parameter Sets: Get
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportCertificatePEM
Optionally, specifies a file path where the referenced Certificate will be saved in PEM format.

```yaml
Type: String
Parameter Sets: Get
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportCertificateDER
Optionally, specifies a file path where the referenced Certificate will be saved in DER format.

```yaml
Type: String
Parameter Sets: Get
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportIssuerPEM
Optionally, specifies a file path where the referenced Issuer Certificate will be saved in PEM format.

```yaml
Type: String
Parameter Sets: Get
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportIssuerDER
Optionally, specifies a file path where the referenced Issuer Certificate will be saved in DER format.

```yaml
Type: String
Parameter Sets: Get
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ExportPkcs12
Optionally, specifies a file path where the referenced Certificate and related artifacts will be saved into a PKCS#12 archive format.

```yaml
Type: String
Parameter Sets: Get
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CertificatePassword
Optionally, specifies a password to use to secure an exported PKCS#12 archive file.

```yaml
Type: String
Parameter Sets: Get
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Overwrite
This flag indicates that any existing files matching any of the requested export parameter paths will be overwritten.
If not specified, existing files will cause this cmdlet to error.

```yaml
Type: SwitchParameter
Parameter Sets: Get
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

[New-Certificate]()

[Submit-Certificate]()

[Update-Certificate]()

