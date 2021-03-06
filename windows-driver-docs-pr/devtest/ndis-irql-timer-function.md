---
title: Irql\_Timer\_Function rule (ndis)
description: The Irql\_Timer\_Function rule specifies that the NDIS timer service functions must be called at correct IRQL levels.
ms.assetid: 4c946f79-7661-4ff6-b2a3-1a5851c9e215
ms.date: 05/21/2018
keywords: ["Irql_Timer_Function rule (ndis)"]
topic_type:
- apiref
api_name:
- Irql_Timer_Function
api_type:
- NA
ms.localizationpriority: medium
---

# Irql\_Timer\_Function rule (ndis)


The Irql\_Timer\_Function rule specifies that the NDIS timer service functions must be called at correct IRQL levels.

This rule verifies the following NDIS functions:

**NdisAllocateTimerObject**
**NdisCancelTimerObject**
**NdisFreeTimerObject**
**NdisSetTimerObject**

|              |      |
|--------------|------|
| Driver model | NDIS |

How to test
-----------

<table>
<colgroup>
<col width="100%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">At compile time</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>Run <a href="https://msdn.microsoft.com/library/windows/hardware/ff552808" data-raw-source="[Static Driver Verifier](https://msdn.microsoft.com/library/windows/hardware/ff552808)">Static Driver Verifier</a> and specify the <strong>Irql_Timer_Function</strong> rule.</p>
Use the following steps to run an analysis of your code:
<ol>
<li><a href="https://msdn.microsoft.com/library/windows/hardware/hh454281#preparing-your-source-code" data-raw-source="[Prepare your code (use role type declarations).](https://msdn.microsoft.com/library/windows/hardware/hh454281#preparing-your-source-code)">Prepare your code (use role type declarations).</a></li>
<li><a href="https://msdn.microsoft.com/library/windows/hardware/hh454281#running-static-driver-verifier" data-raw-source="[Run Static Driver Verifier.](https://msdn.microsoft.com/library/windows/hardware/hh454281#running-static-driver-verifier)">Run Static Driver Verifier.</a></li>
<li><a href="https://msdn.microsoft.com/library/windows/hardware/hh454281#viewing-and-analyzing-the-results" data-raw-source="[View and analyze the results.](https://msdn.microsoft.com/library/windows/hardware/hh454281#viewing-and-analyzing-the-results)">View and analyze the results.</a></li>
</ol>
<p>For more information, see <a href="https://msdn.microsoft.com/library/windows/hardware/hh454281" data-raw-source="[Using Static Driver Verifier to Find Defects in Drivers](https://msdn.microsoft.com/library/windows/hardware/hh454281)">Using Static Driver Verifier to Find Defects in Drivers</a>.</p></td>
</tr>
</tbody>
</table>

Applies to
----------

[**NdisAllocateTimerObject**](https://msdn.microsoft.com/library/windows/hardware/ff561618)
[**NdisCancelTimerObject**](https://msdn.microsoft.com/library/windows/hardware/ff561624)
[**NdisFreeTimerObject**](https://msdn.microsoft.com/library/windows/hardware/ff562605)
[**NdisSetTimerObject**](https://msdn.microsoft.com/library/windows/hardware/ff564563)








