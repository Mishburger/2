# 2
#2

#include <algorithm>
#include <vector>
#include <iostream>
using namespace std;

int main() {
    vector<int> a = {1, 4, 6};
    vector<int> b = {11, 33, 22};

    sort(a.begin(), a.end(),
        [b](int i, int j) { return b[i] < b[j]; });

    for (auto x : a) {
        cout << x << " ";
    }
    cout << endl;
   
    return 0;
}
