---
title: Expression Evaluator Error CXX0036 | Microsoft Docs
ms.custom: 
ms.date: 11/04/2016
ms.reviewer: 
ms.suite: 
ms.technology:
- devlang-cpp
ms.tgt_pltfrm: 
ms.topic: error-reference
f1_keywords:
- CXX0036
dev_langs:
- C++
helpviewer_keywords:
- CXX0036
- CAN0036
ms.assetid: 383404be-df5b-4eec-b113-df21bb5d269d
caps.latest.revision: 6
author: corob-msft
ms.author: corob
manager: ghogen
translation.priority.ht:
- cs-cz
- de-de
- es-es
- fr-fr
- it-it
- ja-jp
- ko-kr
- pl-pl
- pt-br
- ru-ru
- tr-tr
- zh-cn
- zh-tw
translationtype: Human Translation
ms.sourcegitcommit: 3168772cbb7e8127523bc2fc2da5cc9b4f59beb8
ms.openlocfilehash: 81da32ddfdb96efc806cfb1a72ceb89deb97cd43

---
# Expression Evaluator Error CXX0036
bad context {...} specification  
  
 This message can be generated by any of several errors in the use of the context operator (**{}**).  
  
-   The syntax of the context operator (**{}**) was given incorrectly.  
  
     The syntax of the context operator is:  
  
     {*function*,*module*,*dll*}*expression*  
  
     This specifies the context of *expression*. The context operator has the same precedence and usage as a type cast.  
  
     Trailing commas can be omitted. If any of *function*, *module*, or *dll* contains a literal comma, you must enclose the entire name in parentheses.  
  
-   The function name was spelled incorrectly, or does not exist in the specified module or dynamic-link library.  
  
     Because C is a case-sensitive language, *function* must be given in the exact case as it is defined in the source.  
  
-   The module or DLL could not be found.  
  
     Check the full path name of the specified module or DLL.  
  
 This error is identical to CAN0036.


<!--HONumber=Jan17_HO2-->


