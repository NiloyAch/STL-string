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



// String practice probelms with remaining part

/*
#include<bits/stdc++.h>
using namespace std;
int main()
{

    char c = 'A';
    bool f1 = isupper(c);      //1
    cout << f1 << endl;

    char d = 'B';
    bool f2 = islower(d);     //0
    cout << f2 << endl;

    char e = ' ';
    bool f3 = isspace(e);   //1
    cout << f3 << endl;

    char f = 'a';
    f = toupper(f);         //A
    cout << f << endl;

    char g = 'B';
    g = tolower(g);
    cout << g << endl;      //b

    string  h = "asB";
    bool f4 = islower(h[2]);
    cout << f4 << endl;         //0


}
*/

/*
#include<bits/stdc++.h>
using namespace std;

bool isvowel (char c)
{
    return (c=='a' || c=='e' || c=='i' || c=='o' || c=='u' || c=='y');
}
int main()
{
    string s,ans;
    cin >> s;
    for(auto u : s)
    {
        char c = tolower(u);
        if(isvowel(c)==0)
        {
            ans+='.';
            ans+=c;
        }

    }
    cout << ans << endl;
}
*/
/*
#include<bits/stdc++.h>
using namespace std;
int main()
{
    int t;
    cin >> t;
    while(t--)
    {
        string s;
        cin >> s;
        string u = s;
        reverse(u.begin(),u.end());
        if(s==u)
            cout << "Yes" << endl;
        else
            cout << "No" << endl;
    }
}
*/
/*
#include<bits/stdc++.h>
using namespace std;
int main()
{
    string n;
    cin >> n;
    int sum=0;
    for(auto u : n)
    {
        sum+=(u-'0');
    }

    string str = to_string(sum);

    string tmp = str;
    reverse(tmp.begin(),tmp.end());
    if(tmp==str)
        cout << "Yes\n";
    else
        cout << "No\n";

}
*/

/*
#include<bits/stdc++.h>
using namespace std;
int main()
{
    string s1,s2;
    cin >> s1 >> s2;

    for(auto u : s1)
    {
        u = tolower(u);
        for(auto v : s2)
        {
            v = tolower(v);
             if(u==v)
                cout << 0 << "\n";
            else if(u>v)
                cout << 1 << "\n";
            else
                cout << -1 << "\n";
        }
    }

}
*/

/* petya and strings

#include<bits/stdc++.h>
using namespace std;
int main()
{
    ios_base::sync_with_stdio(false);
    cin.tie(NULL);

    string s1,s2;
    cin >> s1 >> s2;
    for(int i=0;i<s1.size();i++) s1[i]=tolower(s1[i]);
    for(int i=0;i<s2.size();i++) s2[i]=tolower(s2[i]);

    if(s1<s2)
        cout << "-1";
    else if(s1>s2)
        cout << "1";
    else
        cout << "0";
}
*/
/*
#include<bits/stdc++.h>
using namespace std;

bool isvowel(char c)
{
    return (c=='a' || c=='e' || c=='i' || c=='o' || c=='u');
}

int main()
{
    vector<string> v;
    int cnt[] = {5,7,5};
    for(int i=0;i<3;i++)
    {
        string s;
        char c;
        cin >> c;
        getline (cin,s);
        s = s+c;
        v.push_back(s);
    }

    for(int i=0;i<3;i++)
    {
        int c=0;
        for(auto u: v[i])
        {
            if(isvowel(u)) c++;
        }
        if(c!=cnt[i]) return cout << "NO\n",0;
    }
    cout << "YES\n";
}
*/

/* hackereart lexogeek

#include<bits/stdc++.h>
using namespace std;
int main()
{
    ios_base::sync_with_stdio(0);
    cin.tie(0);

    int t;
    cin >> t;
    while(t--)
    {
        string s;
        cin >> s;
        if(next_permutation(s.begin(),s.end()))
        {
            cout << s << endl;
        }
        else
        {
            cout << "no answer" << endl;
        }
    }
}

*/


//https://lightoj.com/problem/discovering-permutations

#include<bits/stdc++.h>
using namespace std;
int main()
{
    ios_base::sync_with_stdio(0);
    cin.tie(0);

    int t;
    cin >> t;
    string all = "ABCDEFGHIJKLMNOPSTUVWXYZ";
    while(t--)
    {
        int n,k;
        cin >> n >> k;
        string s,c;
        s = all.substr(0,n);
        c = s;
        cout << "Case " << t << ":" << endl;
        for(int i=1;i<=k;i++)
        {
            cout << s << endl;
            next_permutation(s.begin(),s.end());
            if(s==c) break;
        }
    }
}




