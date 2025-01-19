#include<bits/stdc++.h>
using namespace std;
int main()
{

    string s = "Niloy acharjee";

	cout << s.back() << endl;

	cout << *s.begin() << endl;

	s.pop_back();  //AB

	for(int i=0;i<s.size();i++)
    {
        cout << s[i] << endl;
    }

    //for each loop
    for(auto c : s)
    {
        cout << c << endl;
    }


	string :: iterator it ;
	for(it = s.begin(); it!=s.end(); it++)
	{
		cout << *it << endl;
	}




/*

#include <bits/stdc++.h>
using namespace std;

int main()
{
	string s = "nily acharjee";

	cout << s.back() << endl;

	cout << *s.begin() << endl;


	for(int i = s.size()-1; i>=0; i--)
	{
		cout << s[i];
	}

	string :: iterator it ;
	for(auto it = s.begin(); it!=s.end(); it++)
	{
		cout << *it << endl;
	}


	for(auto it = s.rbegin(); it!=s.rend(); it++ )
	{
		cout << *it;
	}


	s.erase(s.begin());
	cout << s << endl;

	reverse(s.begin(), s.begin()+5);
	cout << s << endl;

	string t =s ;

	reverse(it.begin(),t.end());

}
*/


	string s = "abcde";
	string t = s.substr(1,3);     //bcd
	cout << t << endl;

    string a = "abcsfdhg"
    sort(a.begin(),a.end());      //abcdfghs
    cout << a << endl;

    int t;
    cin >> t;

    string tmp;
    getline (cin ,tmp);

    while(t--)
    {
        string s;
        getline(cin ,s);     // full line input
        cout << s << endl;
    }


    string s = "Ab\"cd";    \ indicating another strings
    cout << s << endl;          //Ab"cd

    ios:: sync_with_stdio(false);
    cin.tie(nullptr);

    for(int i=0;i<3;i++)
    {
        string s;
        cin >> s;
        cout << s << "\n";
    }

    vector<string> v;
    v.push_back("Toky");
    v.push_back("Adnan");

    sort(v.begin(),v.end());
    for(auto p : v)
    {
        cout << p << endl;     //Adnan Toky
    }


    string q = "ab5x89";
    int cnt = 0;
    for(char c : s)
    {
        if(c>='0' && c<='9')
        {
            cnt++;
        }
    }

    cout << cnt << endl;    // value 3 ta



    string y = "abcaacdef";
    vector<int> v(26,0);

    for(char c:s )
    {
        v[c-'a']++;
    }
    for(int i=0;i<26;i++)
    {
        cout << (char) ('a'+i) << "->" << v[i] << endl;       //kon alphabett koto bar ase print korbe
    }
    return 0;



    //anagram string

    string s1 = "listen";
    string s2 = "silent";

    sort(s1.begin(),s1.end());
    sort(s2.begin(),s2.end());
    if(s1==s2)
        cout << "anagram" << endl;
    else
        cout << "not anagram" << endl;
 }



