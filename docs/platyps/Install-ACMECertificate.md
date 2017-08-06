---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Install-ACMECertificate

## SYNOPSIS
Invokes an Installer to install a PKI certificate.

## SYNTAX

### InstallerProfile
```
Install-ACMECertificate [-CertificateRef] <String> -InstallerProfileRef <String>
 [-InstallerParameters <Hashtable>] [-VaultProfile <String>]
```

### InstallerInline
```
Install-ACMECertificate [-CertificateRef] <String> -Installer <String> [-InstallerParameters <Hashtable>]
 [-VaultProfile <String>]
```

## DESCRIPTION
Use this cmdlet to invoke an instance of an Installer Provider defined by a profile stored in an ACMESharp Vault.
The profile will specify the provider name as well as any parameters that will be applied during the instance creation and invocation.
Alternatively, you can specify all the details captured in a profile "inline" during this cmdlet's invocation.

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -CertificateRef
A reference (ID or alias) to a previously retrieved and resolved Certificated provided by an ACME CA Server.

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

### -InstallerProfileRef
Specifies a reference (ID or alias) to a previously defined Installer profile in the associated Vault that defines the Installer provider and associated instance parameters that should be used to install the certificate.

```yaml
Type: String
Parameter Sets: InstallerProfile
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Installer
Specifies the Installer instance provider that will be used to install the associated certificate.

```yaml
Type: String
Parameter Sets: InstallerInline
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -InstallerParameters
Specifies the parameters that will be passed to the Installer instance that will be used to install the associated certificate.

If this cmdlet is invoked *in-line*, then these are the only parameters that will be passed to the handler.
If this cmdlet is invoked with a handler profile reference, then these parameters are merged with, and override, whatever parameters are already defined within the profile.

```yaml
Type: Hashtable
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

## NOTES

## RELATED LINKS

[Get-InstallerProfile]()

[Set-InstallerProfile]()

