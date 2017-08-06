---
external help file: ACMESharp.POSH.dll-Help.xml
online version: 
schema: 2.0.0
---

# Complete-ACMEChallenge

## SYNOPSIS
Completes a Challenge using a prescribed Handler.

## SYNTAX

### ChallengeHandlerProfile
```
Complete-ACMEChallenge [-IdentifierRef] <String> -HandlerProfileRef <String> [-HandlerParameters <Hashtable>]
 [-CleanUp] [-Regenerate] [-Repeat] [-UseBaseUri] [-VaultProfile <String>] [-Force]
```

### ChallengeHandlerInline
```
Complete-ACMEChallenge [-IdentifierRef] <String> [-ChallengeType] <String> -Handler <String>
 [-HandlerParameters <Hashtable>] [-CleanUp] [-Regenerate] [-Repeat] [-UseBaseUri] [-VaultProfile <String>]
 [-Force]
```

## DESCRIPTION
Use this cmdlet to complete a Challenge associated with an Identifier defined in an ACMESharp Vault that has been submitted for verification to an ACME CA Server.

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

### -HandlerProfileRef
Specifies a reference (ID or alias) to a previously defined Challenge Handler profile in the associated Vault that defines the Handler provider and associated instance parameters that should be used to resolve the Challenge.

```yaml
Type: String
Parameter Sets: ChallengeHandlerProfile
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ChallengeType
Specifies the ACME Challenge type that should be handled.
This type is expected to be found in the list of Challenges returned by the ACME CA Server for the associated Identifier.

```yaml
Type: String
Parameter Sets: ChallengeHandlerInline
Aliases: 

Required: True
Position: 1
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Handler
Specifies the Challenge Handler instance provider that will be used to handle the associated Challenge.

```yaml
Type: String
Parameter Sets: ChallengeHandlerInline
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -HandlerParameters
Specifies the parameters that will be passed to the Challenge Handler instance that will be used to handle the associated Challenge.

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

### -CleanUp
When specified, executes the clean up operation associated with the resolved Challenge Handler.
This is typcially invoked after the challenge has been previously successfully completed and submitted to the ACME server, and is used to remove any residual resources or traces of the steps that were needed during the challenge-handling process.

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

### -Regenerate
When specified, will force the decoding and regeneration of any ACME-defined heuristics and parameters for the given Challenge type.

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

### -Repeat
When specified, forces the resolved Handler to repeat the process of handling the given Challenge, even if the process has already been completed previously.

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
Forces an attempt to complete the challenge even when the state of the current Identifier authorization is in a failed or completed state.

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

[Get-ChallengeHandlerProfile]()

[Set-ChallengeHandlerProfile]()

