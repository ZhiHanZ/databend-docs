---
title: BITMAP_HAS_ANY
---

检查第一个位图是否存在与第二个位图匹配的位。

## 语法

```sql
BITMAP_HAS_ANY( <bitmap1>, <bitmap2> )
```

## 示例

```sql
SELECT BITMAP_HAS_ANY(BUILD_BITMAP([1,4,5]), BUILD_BITMAP([1,2]));

┌───────────────────────────────────────────────────────────────┐
│ bitmap_has_any(build_bitmap([1, 4, 5]), build_bitmap([1, 2])) │
├───────────────────────────────────────────────────────────────┤
│ true                                                          │
└───────────────────────────────────────────────────────────────┘
```