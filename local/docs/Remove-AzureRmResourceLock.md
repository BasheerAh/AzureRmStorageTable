---
external help file: Microsoft.Azure.Commands.ResourceManager.Cmdlets.dll-Help.xml
online version: 
schema: 2.0.0
---

# Remove-AzureRmResourceLock

## SYNOPSIS
{{Fill in the Synopsis}}

## SYNTAX

### A lock, by Id. (Default)
```
Remove-AzureRmResourceLock [-Force] -LockId <String> [-ApiVersion <String>] [-Pre] [-WhatIf] [-Confirm]
```

### A lock at the resource group scope.
```
Remove-AzureRmResourceLock -LockName <String> [-Force] -ResourceGroupName <String> [-ApiVersion <String>]
 [-Pre] [-WhatIf] [-Confirm]
```

### A lock at the resource group resource scope.
```
Remove-AzureRmResourceLock -LockName <String> [-Force] -ResourceName <String> -ResourceType <String>
 -ResourceGroupName <String> [-ApiVersion <String>] [-Pre] [-WhatIf] [-Confirm]
```

### A lock at the specified scope.
```
Remove-AzureRmResourceLock -LockName <String> [-Force] -Scope <String> [-ApiVersion <String>] [-Pre] [-WhatIf]
 [-Confirm]
```

### A lock at the subscription scope.
```
Remove-AzureRmResourceLock -LockName <String> [-Force] [-ApiVersion <String>] [-Pre] [-WhatIf] [-Confirm]
```

### A lock at the subscription resource scope.
```
Remove-AzureRmResourceLock -LockName <String> [-Force] -ResourceName <String> -ResourceType <String>
 [-ApiVersion <String>] [-Pre] [-WhatIf] [-Confirm]
```

### A lock at the tenant resource scope.
```
Remove-AzureRmResourceLock -LockName <String> [-Force] -ResourceName <String> -ResourceType <String>
 [-TenantLevel] [-ApiVersion <String>] [-Pre] [-WhatIf] [-Confirm]
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

### -ApiVersion
When set, indicates the version of the resource provider API to use.
If not specified, the API version is automatically determined as the latest available.

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

### -Confirm
Prompts you for confirmation before running the cmdlet.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: cf

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -Force
Do not ask for confirmation.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -LockId
The Id of the lock.

```yaml
Type: String
Parameter Sets: A lock, by Id.
Aliases: Id, ResourceId

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -LockName
The name of the lock.

```yaml
Type: String
Parameter Sets: A lock at the resource group scope., A lock at the resource group resource scope., A lock at the specified scope., A lock at the subscription scope., A lock at the subscription resource scope., A lock at the tenant resource scope.
Aliases: ExtensionResourceName, Name

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Pre
When set, indicates that the cmdlet should use pre-release API versions when automatically determining which version to use.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: 

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -ResourceGroupName
The resource group name.

```yaml
Type: String
Parameter Sets: A lock at the resource group scope., A lock at the resource group resource scope.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceName
The resource name.
e.g.
to specify a database MyServer/MyDatabase.

```yaml
Type: String
Parameter Sets: A lock at the resource group resource scope., A lock at the subscription resource scope., A lock at the tenant resource scope.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -ResourceType
The resource type.
e.g.
Microsoft.Sql/Servers/Databases.

```yaml
Type: String
Parameter Sets: A lock at the resource group resource scope., A lock at the subscription resource scope., A lock at the tenant resource scope.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -Scope
The scope.
e.g.
to specify a database '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaserName}', to specify a resoruce group: '/subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}'

```yaml
Type: String
Parameter Sets: A lock at the specified scope.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: True (ByPropertyName)
Accept wildcard characters: False
```

### -TenantLevel
Indicates that this is a tenant level operation.

```yaml
Type: SwitchParameter
Parameter Sets: A lock at the tenant resource scope.
Aliases: 

Required: True
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

### -WhatIf
Shows what would happen if the cmdlet runs.
The cmdlet is not run.

```yaml
Type: SwitchParameter
Parameter Sets: (All)
Aliases: wi

Required: False
Position: Named
Default value: None
Accept pipeline input: False
Accept wildcard characters: False
```

## INPUTS

### System.String


## OUTPUTS

### System.Management.Automation.PSObject


## NOTES

## RELATED LINKS
