---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Submit-ACMEChallenge

## SYNOPSIS
Submits a completed Challenge for verification by ACME CA Server.

## SYNTAX

```
Submit-ACMEChallenge [-IdentifierRef] <String> [-ChallengeType] <String> [-UseBaseUri] [-VaultProfile <String>]
 [-Force]
```

## DESCRIPTION
After a Challenge has been handled and completed, it needs to be submitted to the ACME CA Server that issued the Challenge.
This cmdlet submits the Challenge of a particular type to the ACME Server to be verified.
If the ACME Server issued multiple Challenges and combinations that will satisfy the validation of ownership of an Identifier, you can use this cmdlet to submit each Challenge type completed.

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
Parameter Sets: (All)
Aliases: Ref

Required: True
Position: 0
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChallengeType
Specifies the ACME Challenge type that should be submitted.
This type is expected to be found in the list of Challenges returned by the ACME CA Server for the associated Identifier and it should already have been handled previously, either externally to the ACMESharp operations or via the Handler mechanisms within.

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

### -UseBaseUri
Overrides the base URI associated with the target Registration and used for subsequent communication with the associated ACME CA Server.

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

### -Force
Forces an attempt to submit the challenge even when the state of the current Identifier authorization is in a failed or completed state.

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

## INPUTS

## OUTPUTS

## NOTES

## RELATED LINKS

[New-Identifier]()

[Complete-Challenge]()

