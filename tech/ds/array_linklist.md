# 数组与链表

## 数组

```python
lst = []
lst.append(1)
lst.append(2)
print(lst)
```

## 链表

```python
class Node(object):

    def __init__(self, val=None):
        self.val = val
        self.next = None

class LinkedList(object):

    def __init__(self, root=None):
        self.root = root or Node()
        self._current_node = self.root

    def add(self, val):
        node = Node(val)
        self._current_node.next = node
        self._current_node = node

    def traverse(self):
        node = self.root.next
        lst = []
        while node:
            lst.append(str(node.val))
            node = node.next

        print(*lst, sep=' -> ')
```
