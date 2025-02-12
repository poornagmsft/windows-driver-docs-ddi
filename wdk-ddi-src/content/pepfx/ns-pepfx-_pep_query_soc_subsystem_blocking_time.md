---
UID: NS:pepfx._PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
title: _PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME (pepfx.h)
description: The PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME structure (pepfx.h) is used by the PEP_DPM_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME notification to collect details about the blocking duration for a particular system on a chip (SoC) subsystem.
old-location: kernel\pep_query_soc_subsystem_blocking_time.htm
tech.root: kernel
ms.date: 07/30/2021
keywords: ["PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME structure"]
ms.keywords: "*PPEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME, PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME, PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME structure [Kernel-Mode Driver Architecture], PPEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME, PPEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME structure pointer [Kernel-Mode Driver Architecture], _PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME, kernel.pep_query_soc_subsystem_blocking_time, pepfx/PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME, pepfx/PPEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME"
req.header: pepfx.h
req.include-header: Pep_x.h
req.target-type: Windows
req.target-min-winverclnt: Supported starting with Windows 10.
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
req.typenames: PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME, *PPEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
f1_keywords:
 - _PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
 - pepfx/_PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
 - PPEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
 - pepfx/PPEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
 - PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
 - pepfx/PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
topic_type:
 - APIRef
 - kbSyntax
api_type:
 - HeaderDef
api_location:
 - pepfx.h
api_name:
 - _PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
 - PPEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
 - PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME
---

# _PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME structure (pepfx.h)

## -description

The **PEP_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME** structure is used by the [PEP_DPM_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME notification](../index.yml) to collect details about the blocking duration for a particular system on a chip (SoC) subsystem.

## -struct-fields

### -field PlatformIdleStateIndex

[in] The platform idle state index for the SoC subsystem that the OS is querying.

### -field SubsystemHandle

[in] A context pointer that the PEP previously provided on subsystem initialization. The context pointer is optional, so if none was provided then the value will be zero. The PEP is free to ignore this field.

### -field SubsystemName

[in] The name of the subsystem whose blocking time is being queried.  This name was provided by the PEP on subsystem initialization.

### -field BlockingTime

[out] The blocking time tallied for this subsystem in 100 nanosecond units since the previous [PEP_DPM_RESET_SOC_SUBSYSTEM_ACCOUNTING notification](../index.yml).

### -field Flags

This member is reserved and should be set to zero.

## -see-also

[PEP_DPM_QUERY_SOC_SUBSYSTEM_BLOCKING_TIME notification](../index.yml)

[PEP_DPM_RESET_SOC_SUBSYSTEM_ACCOUNTING notification](../index.yml)