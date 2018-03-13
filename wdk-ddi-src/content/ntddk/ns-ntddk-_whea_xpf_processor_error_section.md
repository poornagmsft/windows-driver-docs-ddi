---
UID: NS:ntddk._WHEA_XPF_PROCESSOR_ERROR_SECTION
title: "_WHEA_XPF_PROCESSOR_ERROR_SECTION"
author: windows-driver-content
description: The WHEA_XPF_PROCESSOR_ERROR_SECTION structure describes processor error data that is specific to the x86/x64 processor architecture.
old-location: whea\whea_xpf_processor_error_section.htm
old-project: whea
ms.assetid: e994c778-4a1b-4c7d-a9fb-4481d9edda0d
ms.author: windowsdriverdev
ms.date: 2/20/2018
ms.keywords: "*PWHEA_XPF_PROCESSOR_ERROR_SECTION, PWHEA_XPF_PROCESSOR_ERROR_SECTION, PWHEA_XPF_PROCESSOR_ERROR_SECTION structure pointer [WHEA Drivers and Applications], WHEA_XPF_PROCESSOR_ERROR_SECTION, WHEA_XPF_PROCESSOR_ERROR_SECTION structure [WHEA Drivers and Applications], _WHEA_XPF_PROCESSOR_ERROR_SECTION, ntddk/PWHEA_XPF_PROCESSOR_ERROR_SECTION, ntddk/WHEA_XPF_PROCESSOR_ERROR_SECTION, whea.whea_xpf_processor_error_section, whearef_e3338334-dc16-4242-9c30-0daaab2df957.xml"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: ntddk.h
req.include-header: Ntddk.h
req.target-type: Windows
req.target-min-winverclnt: Supported in Windows Server 2008, Windows Vista SP1, and later versions of Windows.
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
req.irql: PASSIVE_LEVEL
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	ntddk.h
api_name:
-	WHEA_XPF_PROCESSOR_ERROR_SECTION
product: Windows
targetos: Windows
req.typenames: WHEA_XPF_PROCESSOR_ERROR_SECTION, *PWHEA_XPF_PROCESSOR_ERROR_SECTION
---

# _WHEA_XPF_PROCESSOR_ERROR_SECTION structure


## -description


The WHEA_XPF_PROCESSOR_ERROR_SECTION structure describes processor error data that is specific to the x86/x64 processor architecture.


## -syntax


````
typedef struct _WHEA_XPF_PROCESSOR_ERROR_SECTION {
  WHEA_XPF_PROCESSOR_ERROR_SECTION_VALIDBITS ValidBits;
  ULONGLONG                                  LocalAPICId;
  UCHAR                                      CpuId[48];
  UCHAR                                      VariableInfo[ANYSIZE_ARRAY];
} WHEA_XPF_PROCESSOR_ERROR_SECTION, *PWHEA_XPF_PROCESSOR_ERROR_SECTION;
````


## -struct-fields




### -field ValidBits

A <a href="..\ntddk\ns-ntddk-_whea_xpf_processor_error_section_validbits.md">WHEA_XPF_PROCESSOR_ERROR_SECTION_VALIDBITS</a> union that specifies which members of this structure contain valid data and the number of structures that are contained in the <b>VariableInfo</b> member.


### -field LocalAPICId

The value programmed into the local APIC ID register.

This member contains valid data only if the <b>ValidBits.LocalAPICId</b> bit is set.


### -field CpuId

A 48-byte buffer that contains the results of executing the CPUID instruction. For more information about the CPUID instruction, see the <a href="http://go.microsoft.com/fwlink/p/?linkid=78804">Intel 64 and IA-32 Architectures Software Developer's Manual</a>.

This member contains valid data only if the <b>ValidBits.CpuId </b>bit is set.


### -field VariableInfo

A variable length buffer that contains zero or more <a href="..\ntddk\ns-ntddk-_whea_xpf_procinfo.md">WHEA_XPF_PROCINFO</a> structures followed by zero or more <a href="..\ntddk\ns-ntddk-_whea_xpf_context_info.md">WHEA_XPF_CONTEXT_INFO</a> structures. The number of WHEA_XPF_PROCINFO structures is specified in <b>ValidBits.ProcInfoCount</b>. The number of WHEA_XPF_CONTEXT_INFO structures is specified in <b>ValidBits.ContextInfoCount</b>. For a diagram that shows how these data structures are stored in the buffer, see the Remarks section.


## -remarks



The WHEA_XPF_PROCESSOR_ERROR_SECTION structure describes the error data that is contained in an x86/x64 processor error section of an <a href="https://msdn.microsoft.com/080da29a-b5cb-45a5-848d-048d9612ee2a">error record</a>. An error record contains an x86/x64 processor error section only if the <b>SectionType </b>member of one of the <a href="..\ntddk\ns-ntddk-_whea_error_record_section_descriptor.md">WHEA_ERROR_RECORD_SECTION_DESCRIPTOR</a> structures that describes the error record sections for that error record contains XPF_PROCESSOR_ERROR_SECTION_GUID.




## -see-also

<a href="..\ntddk\ns-ntddk-_whea_xpf_processor_error_section_validbits.md">WHEA_XPF_PROCESSOR_ERROR_SECTION_VALIDBITS</a>



<a href="..\ntddk\ns-ntddk-_whea_xpf_procinfo.md">WHEA_XPF_PROCINFO</a>



<a href="..\ntddk\ns-ntddk-_whea_error_record_section_descriptor.md">WHEA_ERROR_RECORD_SECTION_DESCRIPTOR</a>



<a href="..\ntddk\ns-ntddk-_whea_xpf_context_info.md">WHEA_XPF_CONTEXT_INFO</a>



 

 

<a href="mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback [whea\whea]:%20WHEA_XPF_PROCESSOR_ERROR_SECTION structure%20 RELEASE:%20(2/20/2018)&amp;body=%0A%0APRIVACY STATEMENT%0A%0AWe use your feedback to improve the documentation. We don't use your email address for any other purpose, and we'll remove your email address from our system after the issue that you're reporting is fixed. While we're working to fix this issue, we might send you an email message to ask for more info. Later, we might also send you an email message to let you know that we've addressed your feedback.%0A%0AFor more info about Microsoft's privacy policy, see http://privacy.microsoft.com/en-us/default.aspx." title="Send comments about this topic to Microsoft">Send comments about this topic to Microsoft</a>
