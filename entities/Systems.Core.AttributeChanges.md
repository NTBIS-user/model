---
uid: Systems.Core.AttributeChanges
---
# Systems.Core.AttributeChanges View

**Namespace:** [Systems.Core](Systems.Core.md)  

Attribute values of an object change. Entity: Sys_Attribute_Changes_View

## Default Visualization
Default Display Text Format:  
_{ObjectChangeId}: {AttributeName}_  
Default Search Member:  
__  

## Aggregate
An [aggregate](https://docs.erp.net/tech/advanced/concepts/aggregates.html) is a cluster of domain objects that can be treated as a single unit.  

Aggregate Parent:  
[Systems.Core.ObjectChanges](Systems.Core.ObjectChanges.md)  
Aggregate Root:  
[Systems.Core.ObjectChangesets](Systems.Core.ObjectChangesets.md)  

## Attributes

| Name | Type | Description |
| ---- | ---- | --- |
| [AttributeName](Systems.Core.AttributeChanges.md#attributename) | string (64) | The attribute name. `Required` `Filter(eq)` `Inherited from Sys_Attribute_<br />Changes_Table.Attribute_Name` 
| [NewValue](Systems.Core.AttributeChanges.md#newvalue) | string (max) __nullable__ | The new value. `Filter(eq;like)` `Inherited from Sys_Attribute_<br />Changes_Table.New_Value` 

## References

| Name | Type | Description |
| ---- | ---- | --- |
| [ObjectChange](Systems.Core.AttributeChanges.md#objectchange) | [ObjectChanges](Systems.Core.ObjectChanges.md) | The object change. `Required` `Filter(multi eq)` `Inherited from Sys_Attribute_<br />Changes_Table.Object_Change_Id` `Owner` |


## Attribute Details

### AttributeName

The attribute name. `Required` `Filter(eq)` `Inherited from Sys_Attribute_Changes_Table.Attribute_Name`

_Type_: **string (64)**  
_Inherited From_: **Sys_Attribute_Changes_Table.Attribute_Name**  
_Supported Filters_: **Equals**  
_Supports Order By_: **False**  
_Maximum Length_: **64**  

### NewValue

The new value. `Filter(eq;like)` `Inherited from Sys_Attribute_Changes_Table.New_Value`

_Type_: **string (max) __nullable__**  
_Inherited From_: **Sys_Attribute_Changes_Table.New_Value**  
_Supported Filters_: **Equals, Like**  
_Supports Order By_: **False**  
_Maximum Length_: **2147483647**  


## Reference Details

### ObjectChange

The object change. `Required` `Filter(multi eq)` `Inherited from Sys_Attribute_Changes_Table.Object_Change_Id` `Owner`

_Type_: **[ObjectChanges](Systems.Core.ObjectChanges.md)**  
_Inherited From_: **Sys_Attribute_Changes_Table.Object_Change_Id**  
_Supported Filters_: **Equals, EqualsIn**  
_[Filterable Reference](https://docs.erp.net/dev/domain-api/filterable-references.html)_: **True**  


## API

Domain API Query:
<https://demodb.my.erp.net/api/domain/odata/Systems_Core_AttributeChanges?$top=10>

Domain API Query Builder:
<https://demodb.my.erp.net/api/domain/querybuilder#Systems_Core_AttributeChanges?$top=10>

