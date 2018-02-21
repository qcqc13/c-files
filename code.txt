#include iostream
#include fstream
#include string
using namespace std;

const int N = 2;  number of strings in the file

struct album
{
    for example
   string nickname;
   string role;
     free space for your things
};


int main()
{
ifstream count(album.txt);  values file
int k = 0;	 string counter

	if (count)
	{
    while (!count.eof())  reads from file while it not ended
        {
        string buff;
        count  buff;
        k++;  adding string
        }
	}
        else
        {cout  File not found!  endl; return 0;}  don't forget to upload your file

	if (k % N == 0)
        {k = k  N;}
            else
            {k = (k - (k % N))  N;}

	album  WhatEver = new album[k];

	ifstream fileb(album.txt);
	for (int i = 0; i  k; i++)
        {
		fileb  WhatEver[i].nickname;			 inputing to struct
		fileb  WhatEver[i].role;
        }
        fileb.close();

	string key;
	while (key!= stop)
    {
		cout  Type the name (if you want to finish, write stop)----;
		getline(cin,key);  getting keyword


        bool match = false;  boll value for infinity reading cycle
		for (int i = 0; i  k; i++)
        {
			if (key == WhatEver[i].nickname)
                {
                cout  endl;
                cout  WhatEver[i].nickname   is a  WhatEver[i].role  endl;

				cout  endl;
				match = true;
                }
		}
		if (match == false && key!= stop)  the end of the cycle
        {cout  Not found  endl;}
	}
	delete[] WhatEver;
    return 0;
}

