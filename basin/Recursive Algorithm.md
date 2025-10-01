```
Form two lines of 32 each, with attendees matched up. Every 30 seconds, have one line shift left one position (with the person on the left end wrapping to right). Once the person that started on the left is back on the left, then have each line split into two matched lines, and repeat until each line has just one person.
```

```
With two lines, 32 * 30 seconds is used. Then the lines split, yielding 4 lines (16 and 16, and another 16 and 16). 16 * 30 seconds is used. Then 8 lines (8 and 8, 8 and 8, 8 and 8, 8 and 8), so 8 * 30 seconds. And so on. Total time is about (32 + 16 + 8 + 4 + 2 + 1) * 30 seconds, or 63 * 30 seconds. This solution is an example of a "recursive" solution (discussed elsewhere).
```

---
#computer-science 