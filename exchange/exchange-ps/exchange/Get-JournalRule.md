---
applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online
schema: 2.0.0
---

# Get-JournalRule

## SYNOPSIS
!!! Exchange Server 2010

Use the Get-JournalRule cmdlet to view the journal configuration on a Hub Transport server.

!!! Exchange Server 2013, Exchange Server 2016, Exchange Online

This cmdlet is available in on-premises Exchange and in the cloud-based service. Some parameters and settings may be exclusive to one environment or the other.

Use the Get-JournalRule cmdlet to view the journal rules in your organization.

For information about the parameter sets in the Syntax section below, see Exchange cmdlet syntax (https://technet.microsoft.com/library/bb123552.aspx).

## SYNTAX

```
Get-JournalRule [[-Identity] <RuleIdParameter>] [-DomainController <Fqdn>] [-LawfulInterception]
 [-Organization <OrganizationIdParameter>] [<CommonParameters>]
```

## DESCRIPTION
!!! Exchange Server 2010

The Get-JournalRule cmdlet displays all rules configured for use with the Journaling agent.

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Journaling" entry in the Messaging Policy and Compliance Permissions topic.

!!! Exchange Server 2013

The Get-JournalRule cmdlet displays journal rules configured in your organization.

You need to be assigned permissions before you can run this cmdlet. Although all parameters for this cmdlet are listed in this topic, you may not have access to some parameters if they're not included in the permissions assigned to you. To see what permissions you need, see the "Journaling" entry in the Messaging policy and compliance permissions topic.

!!! Exchange Server 2016, Exchange Online

The Get-JournalRule cmdlet displays journal rules configured in your organization.

You need to be assigned permissions before you can run this cmdlet. Although this topic lists all parameters for the cmdlet, you may not have access to some parameters if they're not included in the permissions assigned to you. To find the permissions required to run any cmdlet or parameter in your organization, see Find the permissions required to run any Exchange cmdlet (https://technet.microsoft.com/library/mt432940.aspx).

## EXAMPLES

### Example 1 -------------------------- (Exchange Server 2010)
```
Get-JournalRule
```

This example retrieves all journal rules configured on a Hub Transport server.

### Example 1 -------------------------- (Exchange Server 2013)
```
Get-JournalRule
```

This example retrieves all journal rules configured in your organization.

### Example 1 -------------------------- (Exchange Server 2016)
```
Get-JournalRule
```

This example retrieves all journal rules configured in your organization.

### Example 1 -------------------------- (Exchange Online)
```
Get-JournalRule
```

This example retrieves all journal rules configured in your organization.

### Example 2 -------------------------- (Exchange Server 2010)
```
Get-JournalRule "Brokerage Communications" | Format-List
```

This example retrieves the specific journal rule Brokerage Communications and pipes the output to the Format-List cmdlet to view all the parameters of the rule.

### Example 2 -------------------------- (Exchange Server 2013)
```
Get-JournalRule "Brokerage Communications" | Format-List
```

This example retrieves the specific journal rule Brokerage Communications and pipes the output to the Format-List cmdlet to view all the parameters of the rule.

### Example 2 -------------------------- (Exchange Server 2016)
```
Get-JournalRule "Brokerage Communications" | Format-List
```

This example retrieves the specific journal rule Brokerage Communications and pipes the output to the Format-List cmdlet to view all the parameters of the rule.

### Example 2 -------------------------- (Exchange Online)
```
Get-JournalRule "Brokerage Communications" | Format-List
```

This example retrieves the specific journal rule Brokerage Communications and pipes the output to the Format-List cmdlet to view all the parameters of the rule.

## PARAMETERS

### -DomainController
!!! Exchange Server 2010

The DomainController parameter specifies the domain controller that's used by this cmdlet to read data from or write data to Active Directory. You identify the domain controller by its fully qualified domain name (FQDN). For example, dc01.contoso.com.



!!! Exchange Server 2013, Exchange Server 2016, Exchange Online

This parameter is available only in on-premises Exchange.

The DomainController parameter specifies the domain controller that's used by this cmdlet to read data from or write data to Active Directory. You identify the domain controller by its fully qualified domain name (FQDN). For example, dc01.contoso.com.



```yaml
Type: Fqdn
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Identity
!!! Exchange Server 2010

The Identity parameter specifies the rule to be viewed. Enter either the GUID or the name of the journal rule. You can omit the parameter label.



!!! Exchange Server 2013, Exchange Server 2016, Exchange Online

The Identity parameter specifies the rule you want to view. Enter either the name or the GUID of the journal rule. You can omit the parameter label.



```yaml
Type: RuleIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010, Exchange Server 2013, Exchange Server 2016, Exchange Online

Required: False
Position: 1
Default value: None
Accept pipeline input: True
Accept wildcard characters: False
```

### -LawfulInterception
This parameter is available for multi-tenant deployments. It isn't available for on-premises deployments. For more information about multi-tenant deployments, see Multi-Tenant Support.

The LawfulInterception parameter returns journal rules for the specified organization in which mailbox content is being lawfully intercepted.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Organization
This parameter is available for multi-tenant deployments. It isn't available for on-premises deployments. For more information about multi-tenant deployments, see Multi-Tenant Support.

The Organization parameter specifies the organization in which you'll perform this action. This parameter doesn't accept wildcard characters, and you must use the exact name of the organization.

```yaml
Type: OrganizationIdParameter
Parameter Sets: (All)
Aliases:
Applicable: Exchange Server 2010

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### CommonParameters
This cmdlet supports the common parameters: -Debug, -ErrorAction, -ErrorVariable, -InformationAction, -InformationVariable, -OutVariable, -OutBuffer, -PipelineVariable, -Verbose, -WarningAction, and -WarningVariable. For more information, see about_CommonParameters (https://go.microsoft.com/fwlink/p/?LinkID=113216).

## INPUTS

###  
To see the input types that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Input Type field for a cmdlet is blank, the cmdlet doesn't accept input data.

## OUTPUTS

###  
To see the return types, which are also known as output types, that this cmdlet accepts, see Cmdlet Input and Output Types (https://go.microsoft.com/fwlink/p/?LinkId=616387). If the Output Type field is blank, the cmdlet doesn't return data.

## NOTES

## RELATED LINKS

[Online Version](https://technet.microsoft.com/library/7620913f-cf28-4e82-983f-61a79f0b6e5a.aspx)
