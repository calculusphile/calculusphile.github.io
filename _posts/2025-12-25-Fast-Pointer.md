---
layout: post
title: "Slow and Fast Pointer"
date: 2025-12-25
---

Slow and Fast pointer are very useful in Linked List.

## Concept



## Problems

1. [Leetcode 876. Middle of the Linked List](https://leetcode.com/problems/middle-of-the-linked-list/description/)


```cpp
class Solution {
public:
    ListNode* middleNode(ListNode* head) {
        ListNode* slow = head;
        ListNode* fast = head;
        while(fast != nullptr && fast->next != nullptr) {
            slow = slow->next;
            fast = fast->next->next;
        }
        return slow;
    }
};
```

For Full Solution [CLICK HERE](../learning/data-structures/LinkedList/leetcode-876.cpp)

---

Enjoy blogging!
