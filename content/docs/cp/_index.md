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