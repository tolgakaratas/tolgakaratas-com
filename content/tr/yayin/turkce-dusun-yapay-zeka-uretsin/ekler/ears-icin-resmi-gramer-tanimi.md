---
title: "Ek D: EARS için Resmi Gramer Tanımı (EBNF)"
weight: 4
type: docs
---

Bu gramer, bir AI sistemine EARS'ın yapısal kurallarını öğretmek için kullanılabilir.

```
requirement      ::= [state_clause], [event_clause], system_name, "shall", system_response, "."
state_clause     ::= "While", condition
event_clause     ::= "When", event
system_name      ::= "the", TEXT
system_response  ::= TEXT
condition        ::= TEXT
event            ::= TEXT

(\* Note: This is a simplified representation. For unwanted behavior \*)
unwanted_req     ::= "If", unwanted_condition, ",", "then", system_name, "shall", system_response, "."
unwanted_condition ::= TEXT
```
