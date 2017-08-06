---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# New-ACMECertificate

## SYNOPSIS
Initiates a request to issue a request for previously authorized Identifier.

## SYNTAX

### Default (Default)
```
New-ACMECertificate [-IdentifierRef] <String> -KeyPemFile <String> -CsrPemFile <String> [-Alias <String>]
 [-Label <String>] [-Memo <String>] [-VaultProfile <String>]
```

### Generate
```
New-ACMECertificate [-IdentifierRef] <String> [-Generate] [-CsrDetails <Hashtable>]
 [-AlternativeIdentifierRefs <System.Collections.Generic.IEnumerable`1[System.Object]>] [-Alias <String>]
 [-Label <String>] [-Memo <String>] [-VaultProfile <String>]
```

## DESCRIPTION
This cmdlet is used to request a new certificate for a DNS Identifier that has already been verified by the ACME CA Server.
It is also used to import, generate or define the certificate parameters and artifacts needed for the request, such as the private key and CSR details.

## EXAMPLES

### Example 1
```
PS C:\> {{ Add example code here }}
```

{{ Add example description here }}

## PARAMETERS

### -IdentifierRef
A reference (ID or alias) to a previously defined and authorized Identifier verified by the ACME CA Server.

```yaml
Type: String
Parameter Sets: (All)
Aliases: Identifier, Ref

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -KeyPemFile
Specifies an existing private key in PEM file format that should be used to generate the Certificate Request.

```yaml
Type: String
Parameter Sets: Default
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -CsrPemFile
Specifies an existing CSR in PEM file format containing all the details of the Certificate that should be used to generate the Certificate Request.

```yaml
Type: String
Parameter Sets: Default
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Generate
Indicates that new Certificate Request parameters and artificats should be generated.

```yaml
Type: SwitchParameter
Parameter Sets: Generate
Aliases: 

Required: True
Position: Named
Default value: False
Accept pipeline input: False
Accept wildcard characters: False
```

### -CsrDetails
An optional set of certificate details to be included in the generated CSR.

The common name will be set based on the DNS name of the associated Identifier, however all other details will be specified as set in this parameter.
The following elements are defined, however not all of these may be supported or honored by the target ACME CA Server: * Country; // C; * StateOrProvince; // ST; * Locality; // L; * Organization; // O; * OrganizationUnit; // OU; * Description; // D; * Surname; // S; * GivenName; // G; * Initials; // I; * Title; // T; * SerialNumber; // SN; * UniqueIdentifier; // UID; * AlternativeNames; // X509 SAN Extension (manually overridden)

For any elements that except multiple values (such as SAN), specify a string of values separated by space, comma or semicolon

```yaml
Type: Hashtable
Parameter Sets: Generate
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -AlternativeIdentifierRefs
A collection of one or more references (ID or alias) to previously defined and authorized Identifiers verified by the ACME CA Server which will be included in the X509 extension for the list of Subject Alternative Names (SAN).

There is no need to repeat the reference to the primary common name Identifier as it will be automatically included at the start of this list.

```yaml
Type: System.Collections.Generic.IEnumerable`1[System.Object]
Parameter Sets: Generate
Aliases: AltIdentifiers, AltRefs

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Alias
An optional, unique alias to assign to the Certificate for future reference.

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
An optional, human-friendly label to assign to the Certificate for easy recognition.

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
An optional, arbitrary text field to capture any notes or details associated with the Certificate.

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

### ACMESharp.Vault.Model.CertificateInfo

## NOTES

## RELATED LINKS

[New-Identifier]()

[Complete-Challenge]()

