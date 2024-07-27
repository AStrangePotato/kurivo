---
title: C++ Template
weight: 1
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


## DSU
```
int find(int v) {
    if (v == parent[v])
        return v;
    return parent[v] = find_set(parent[v]);
}

void unite(int x, int y) {
    int rootX = find(x); int rootY = find(y);
    parent[rootX] = rootY;
}
```
