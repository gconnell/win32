---
title: CimMofDeserializer.DeserializeClasses method (Byte[], UInt32, IEnumerable(CimClass)) (Microsoft.Management.Infrastructure.Serialization)
TOCTitle: CimMofDeserializer.DeserializeClasses method (Byte[], UInt32, IEnumerable(CimClass)) (Microsoft.Management.Infrastructure.Serialization)
ms:assetid: M:Microsoft.Management.Infrastructure.Serialization.CimMofDeserializer.DeserializeClasses(System.Byte[],System.UInt32@,System.Collections.Generic.IEnumerable{Microsoft.Management.Infrastructure.CimClass})
ms.date: 11/13/2019
mtps_version: v=VS.85
dev_langs:
- csharp
- c++
- fsharp
- vb
api_location:
- Microsoft.Management.Infrastructure.dll
api_name:
- Microsoft.Management.Infrastructure.Serialization.CimMofDeserializer.DeserializeClasses
api_type:
- Assembly
topic_type:
- apiref
product_family_name: VS
ms.topic: reference
---

# CimMofDeserializer.DeserializeClasses method (Byte\[\], UInt32, IEnumerable\<CimClass\>)

Deserializes CIM classes based on serialized data, and a collection of parent CIM classes.

**Namespace:**   [Microsoft.Management.Infrastructure.Serialization](hh832966\(v=vs.85\).md)  
**Assembly:**  Microsoft.Management.Infrastructure (in Microsoft.Management.Infrastructure.dll)  

## Syntax

``` csharp
public IEnumerable<CimClass> DeserializeClasses(
    byte[] serializedData,
    ref uint offset,
    IEnumerable<CimClass> classes
)
```

``` c++
public:
IEnumerable<CimClass^>^ DeserializeClasses(
    array<unsigned char>^ serializedData,
    unsigned int% offset,
    IEnumerable<CimClass^>^ classes
)
```

``` fsharp
member DeserializeClasses : 
        serializedData:byte[] *
        offset:uint32 byref *
        classes:IEnumerable<CimClass> -> IEnumerable<CimClass>
```

``` vb
Public Function DeserializeClasses (
    serializedData As Byte(),
    ByRef offset As UInteger,
    classes As IEnumerable(Of CimClass)
) As IEnumerable(CimClass)
```

#### Parameters

  - serializedData  
    Type: [System.Byte](/dotnet/api/system.byte?view=netframework-4.8)\[\]
    
    A buffer that contains the serialized data.

<!-- end list -->

  - offset  
    Type: [System.UInt32](/dotnet/api/system.uint32?view=netframework-4.8)
    
    The byte offset to the location at which to begin reading the data. When the method returns, the offset will be pointing to the next byte after the deserialized classes.

<!-- end list -->

  - classes  
    Type: [System.Collections.Generic.IEnumerable](/dotnet/api/system.collections.generic.ienumerable-1?view=netframework-4.8)\<[CimClass](hh832269\(v=vs.85\).md)\>
    
    An optional cache of parent CIM classes.

#### Return value

Type: [System.Collections.Generic.IEnumerable](/dotnet/api/system.collections.generic.ienumerable-1?view=netframework-4.8)\<[CimClass](hh832269\(v=vs.85\).md)\>

An [IEnumerable\<T\>](/dotnet/api/system.collections.generic.ienumerable-1?view=netframework-4.8) interface that can be used to enumerate the CIM classes.

## See also

[CimClass class](hh832269\(v=vs.85\).md)  
[Microsoft.Management.Infrastructure.Serialization namespace](hh832966\(v=vs.85\).md)