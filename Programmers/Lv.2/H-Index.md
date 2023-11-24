# Python

```python
def solution(citations):
    for h in range(len(citations), 1, -1):
        count = 0
        for i in citations:
            if h <= i:
                count += 1
        if len(citations) - count <= h and count >= h:
            return h

    return 0
```
