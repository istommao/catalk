# 栈与队列

## 栈 LIFO

```python
class Stack(object):

    def __init__(self):
        self._items = []

    def push(self, val):
        self._items.append(val)

    def pop(self):
        return self._items.pop()

    def top(self):
        return self._items[0]

```

## 队列 FIFO

```python
class Queue(object):

    def __init__(self):
        self._items = []

    def enqueue(self, val):
        self._items.insert(0, val)

    def dequeue(self):
        return self._items.pop()
```
