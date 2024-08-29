
> Problem: [LCP 44. 开幕式焰火](https://leetcode.cn/problems/sZ59z6/description/)

[TOC]

# 思路

dfs前序遍历 + 哈希表

# 复杂度

- 时间复杂度: $O(n)$
- 空间复杂度: $O(n)$

# Code

```Rust []
use std::rc::Rc;
use std::cell::RefCell;
use std::collections::HashSet;
impl Solution {
    pub fn num_color(root: Option<Rc<RefCell<TreeNode>>>) -> i32 {
        fn dfs(root: &Option<Rc<RefCell<TreeNode>>>, hashset: &mut HashSet<i32>, res: &mut i32) {
            if root.is_none() {
                return;
            }
            let node = root.as_ref().unwrap().borrow();
            if !hashset.contains(&node.val) {
                *res += 1;
                hashset.insert(node.val);
            }
            dfs(&node.left, hashset, res);
            dfs(&node.right, hashset, res)
        }
        let mut hashset = HashSet::new();
        let mut res = 0;
        dfs(&root, &mut hashset, &mut res);
        res
    }
}
```
