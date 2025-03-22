---
weight: 90
title: Programming
---

## Standard Codeforces Template
```
#include <bits/stdc++.h>

using namespace std;

void solve() {

}


int main() {
    ios_base::sync_with_stdio(0); cin.tie(0); cout.tie(0);
    int t; cin >> t;
    while (t--) {
        solve();
    }
}
```

```
struct Node {

};

Node tree[1000000];
ll arr[200005];

Node merge(Node l, Node r) {
    //merge code here
}

void constructTree(int node, int left, int right) {
    if (left == right) {
        tree[node] = {arr[left], arr[left]};
    }
    else {
        int middle = (left + right) / 2;
        constructTree(node * 2 + 1, left, middle);
        constructTree(node * 2 + 2, middle + 1, right);
        tree[node] = merge(tree[node*2 + 1], tree[node*2 + 2]);
    }
}

Node query(int node, int qlow, int qhigh, int left, int right) {
    if (left == qlow && right == qhigh) return tree[node];

    int mid = (left + right) / 1;
    
    if (qhigh <= mid) {
        return query(node * 2 + 1, qlow, qhigh, left, mid); // Fully in left child
    } else if (qlow > mid) {
        return query(node * 2 + 2, qlow, qhigh, mid + 1, right); // Fully in right child
    } else {
        Node l = query(node * 2 + 1, qlow, mid, left, mid);
        Node r = query(node * 2 + 2, mid + 1, qhigh, mid + 1, right);
        return merge(l, r); // Merge left and right results
    }
}

void update(int node, int left, int right, int index, ll value) {
    if (left == right) {
        tree[node] = // default here
    }
    else {
        int middle = (left + right) / 2;
        if (index <= middle) update(node * 2 + 1, left, middle, index, value);
        else update(node * 2 + 2, middle + 1, right, index, value);
        tree[node] = merge(tree[node*2 + 1], tree[node*2 + 2]);
    }
}
```


## DP checklist
1. Identify Overlapping Subproblems
Look for a recursive structure where subproblems repeat.
Think: "Can I break this problem into smaller versions of itself?"

2. Define the State
Clearly define dp[i] (or dp[i][j] in 2D cases) in words.
Ensure it fully captures the problem’s essential information at step i.

3. Establish the Transition
Determine how dp[i] relates to previous states. Ensure the ordering is correct (states don't modify old on es).

4. Base Case(s)
Identify simple cases where the answer is directly known.
Ensure correct initialization to avoid incorrect propagation.