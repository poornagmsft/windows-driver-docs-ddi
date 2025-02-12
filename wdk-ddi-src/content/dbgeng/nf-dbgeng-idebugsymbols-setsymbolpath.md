---
UID: NF:dbgeng.IDebugSymbols.SetSymbolPath
title: IDebugSymbols::SetSymbolPath (dbgeng.h)
description: The IDebugSymbols::SetSymbolPath method sets the symbol path. This method belongs to the IDebugSymbols interface.
old-location: debugger\setsymbolpath.htm
tech.root: debugger
ms.date: 05/03/2018
keywords: ["IDebugSymbols::SetSymbolPath"]
ms.keywords: IDebugSymbols interface [Windows Debugging],SetSymbolPath method, IDebugSymbols.SetSymbolPath, IDebugSymbols2 interface [Windows Debugging],SetSymbolPath method, IDebugSymbols2::SetSymbolPath, IDebugSymbols3 interface [Windows Debugging],SetSymbolPath method, IDebugSymbols3::SetSymbolPath, IDebugSymbols::SetSymbolPath, IDebugSymbols_b699ac62-be52-4f79-9762-8ed1274dfb41.xml, SetSymbolPath, SetSymbolPath method [Windows Debugging], SetSymbolPath method [Windows Debugging],IDebugSymbols interface, SetSymbolPath method [Windows Debugging],IDebugSymbols2 interface, SetSymbolPath method [Windows Debugging],IDebugSymbols3 interface, dbgeng/IDebugSymbols2::SetSymbolPath, dbgeng/IDebugSymbols3::SetSymbolPath, dbgeng/IDebugSymbols::SetSymbolPath, debugger.setsymbolpath
req.header: dbgeng.h
req.include-header: Dbgeng.h
req.target-type: Desktop
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
targetos: Windows
req.typenames: 
f1_keywords:
 - IDebugSymbols::SetSymbolPath
 - dbgeng/IDebugSymbols::SetSymbolPath
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - COM
api_location:
 - dbgeng.h
api_name:
 - IDebugSymbols::SetSymbolPath
---

# IDebugSymbols::SetSymbolPath


## -description

The <b>SetSymbolPath</b>  method sets the symbol path.

## -parameters

### -param Path 

[in]
Specifies the new symbol path.  This is a string that contains symbol path elements separated by semicolons (;).  Each symbol path element can specify either a directory or a symbol server.

## -returns

This method can also return error values.  See <a href="/windows-hardware/drivers/debugger/hresult-values">Return Values</a> for more details.

<table>
<tr>
<th>Return code</th>
<th>Description</th>
</tr>
<tr>
<td width="40%">
<dl>
<dt><b>S_OK</b></dt>
</dl>
</td>
<td width="60%">
The method was successful.

</td>
</tr>
</table>

## -remarks

For more information about manipulating the symbol path, see <a href="/windows-hardware/drivers/debugger/using-symbols">Using Symbols</a>.  For an overview of the symbol path and its syntax, see <a href="/windows-hardware/drivers/debugger/symbol-path">Symbol Path</a>.

## -see-also

<a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugsymbols3-appendsymbolpath">AppendSymbolPath</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nf-dbgeng-idebugsymbols3-getsymbolpath">GetSymbolPath</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols">IDebugSymbols</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols2">IDebugSymbols2</a>



<a href="/windows-hardware/drivers/ddi/dbgeng/nn-dbgeng-idebugsymbols3">IDebugSymbols3</a>

