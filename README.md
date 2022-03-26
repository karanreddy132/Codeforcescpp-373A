# Codeforcescpp-373A
#include <bits/stdc++.h>
using namespace std;

int main() {
	int k;
	cin >> k;
	string s[5];
	for (int i = 0; i < 4; i++) {
		cin >> s[i];
	}
	for (int i = 1; i <= 9; i++) {
		int count(0);
    char ch = '0' + i;
		for (int j = 0; j < 4; j++) {
			for (int k = 0; k < 4; k++) {
				if (s[j][k]==ch){
          count++;
        }
			}
		}
    if(count > 2*k){
      cout << "NO";
      return 0;
    }
	}
  cout << "YES" << endl;
	return 0;
}
