---
title: base64_decode_toarray() - Azure Data Explorer
description: Learn how to use the base64_decode_toarray() function to decode a base64 string into an array of long values.
ms.reviewer: alexans
ms.topic: reference
ms.date: 11/03/2022
---
# base64_decode_toarray()

Decodes a base64 string to an array of long values.

## Syntax

`base64_decode_toarray(`*String*`)`

## Arguments

* *String*: Input base64 string to be decoded from base64 to an array of long values.

## Returns

Returns an array of long values decoded from a base64 string.

* To decode base64 strings to a UTF-8 string, see [base64_decode_tostring()](base64_decode_tostringfunction.md)
* To encode strings to a base64 string, see [base64_encode_tostring()](base64_encode_tostringfunction.md)

## Example

<!-- csl: https://help.kusto.windows.net/Samples -->
```kusto
print Quine=base64_decode_toarray("S3VzdG8=")  
// 'K', 'u', 's', 't', 'o'
```

|Quine|
|-----|
|[75,117,115,116,111]|
