# Bug 1 Q.18

1. **The incorrect original code or code snippit that you wrote:**

``` cpp
//code with bugs or code snippet with bug goes here

//sample code

// Online C++ compiler to run C++ online.
// Write C++ code in this online editor and run it.

// This program finds the average time spent programming by a student
// each day over a three day period.

// PLACE YOUR NAME HERE

#include <iostream>
using namespace std;

int main()
{
	int numStudents;
	int numdays;
	float numHours, total, average;
	int student, day = 0;	// these are the counters for the loops

	cout << "This program will find the average number of hours a day"
		 << " that a student spent programming over a long weekend\n\n";
	cout << "How many students are there ?" <<endl<<endl;
	cin >> numStudents;

	cout << Enter the number of days in the long weekend <<endl <<endl;
	cin >> numdays;

	for (student = 1; student <= numStudents; student++)
	{
		total = 0;

		for (day = 1; day <= 3; day++)
		{
			cout << "Please enter the number of hours worked by student "
				 << student << " on day " << day << "." << endl;
			cin >> numHours;

			total = total + numHours;
		}

		average = total / 3;

		cout << endl;
		cout << "The average number of hours per day spent programming by "
			 << "student " << student << " is " << average
			 << endl << endl << endl;
	}

	return 0;
}


```

2. **What bug does the original code have?**

  I missed the terminating characters in 21st line.

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

   While writing the code ,I forgot to put the terminating characters.

4. **How to correct the bug?**

   By putting the terminating characters ,the bug can be corrected.

​    5.**The corresponding bug-free code or code snippet is:**

// This program finds the average time spent programming by a student
// each day over a three day period.

// PLACE YOUR NAME HERE

#include <iostream>
using namespace std;

int main()
{
	int numStudents;
	int numdays;
	float numHours, total, average;
	int student, day = 0;	// these are the counters for the loops

	cout << "This program will find the average number of hours a day"
		 << " that a student spent programming over a long weekend\n\n";
	cout << "How many students are there ?" <<endl<<endl;
	cin >> numStudents;
	
	cout << "Enter the number of days in the long weekend" <<endl <<endl;
	cin >> numdays;
	
	for (student = 1; student <= numStudents; student++)
	{
		total = 0;
	
		for (day = 1; day <= 3; day++)
		{
			cout << "Please enter the number of hours worked by student "
				 << student << " on day " << day << "." << endl;
			cin >> numHours;
	
			total = total + numHours;
		}
	
		average = total / 3;
	
		cout << endl;
		cout << "The average number of hours per day spent programming by "
			 << "student " << student << " is " << average
			 << endl << endl << endl;
	}
	
	return 0;
}

```
bug-free code or code snippet goes here

```

6. **What is the take-away message from this bug?**

   Now,I know where to put the terminating characters as I searched that out on google after getting the error of that.

---

# Bug 2 Q.19

1. **The incorrect original code or code snippit that you wrote:**

```
code with bugs or code snippet with bug goes here
// This program finds the average time spent programming by a student
// each day over a three day period.

// PLACE YOUR NAME HERE

#include <iostream>
using namespace std;

int main()
{
	int numStudents;
	int numdays;
	float numhours, total, Average1,Average2;
	int student, day = 0;	// these are the counters for the loops

	cout << "This program will find the average number of hours a day"
		 << " that a student spent programming and biology over a long weekend\n\n";
	cout << "How many students are there ?" <<endl<<endl;
	cin >> numStudents;

	cout <<" Type the number of days in the long weekend" <<endl <<endl;
	cin >> numdays;

	for (student = 1; student <= numStudents; student++)
	{
		total = 0;

		for (day = 1; day <=numdays; day++)
		{
			cout << "Please enter the number of hours worked by student "
				 << student << " on day " << day << " in programming " << endl;
			cin >> numhours;

			total = total + numhours;
		}


		Average1=total/numdays;

		cout << endl;
		cout << "The average number of hours per day spent programming by "
			 << " student " << student << " is " << Average1
			 << endl << endl << endl;




     total=0;
     for(day=1;day<=numdays;day++)
     {
         cout<<" Please enter the number of hours worked by student  "
         << student<<" on day"<<day<<" in biology "<<endl<<endl;
         cin>>numhours;
         total=total+numhours;
     }




     Average2 =total/numdays;
     cout<<endl;
     cout<<"The average number of hours spent per day biology by "
      << " student " << student << " is " << Average2
      <<endl<<endl<<endl;





	if (Average2 > Average1)
    {
        cout<< "Student" <<student<<" utilized more time studying biology as compared to programming "<<endl<<endl;
    }



    if (Average2 < Average1)
    {
        cout<< "Student "<<student<<" utilized more time studying programming as compared to biology "<<endl<<endl;
    }


    else if (Average2=Average1)
    {
     cout<<" Student "<<student<<" utilized the same amount of time studying programming and biology."<<endl<<endl;
    }



	

	return 0;
}


```

2. **What bug does the original code have?**

  I did not put the semicolon in the 83 line.

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

   I used to think like after if else there is no semicolon .

4. **How to correct the bug?**

   By putting the semicolon ,it can be corrected.

5. **The corresponding bug-free code or code snippet is:**

```
bug-free code or code snippet goes here
// This program finds the average time spent programming by a student
// each day over a three day period.

// PLACE YOUR NAME HERE

#include <iostream>
using namespace std;

int main()
{
	int numStudents;
	int numdays;
	float numhours, total, Average1,Average2;
	int student, day = 0;	// these are the counters for the loops

	cout << "This program will find the average number of hours a day"
		 << " that a student spent programming and biology over a long weekend\n\n";
	cout << "How many students are there ?" <<endl<<endl;
	cin >> numStudents;

	cout <<" Type the number of days in the long weekend" <<endl <<endl;
	cin >> numdays;

	for (student = 1; student <= numStudents; student++)
	{
		total = 0;

		for (day = 1; day <=numdays; day++)
		{
			cout << "Please enter the number of hours worked by student "
				 << student << " on day " << day << " in programming " << endl;
			cin >> numhours;

			total = total + numhours;
		}


		Average1=total/numdays;

		cout << endl;
		cout << "The average number of hours per day spent programming by "
			 << " student " << student << " is " << Average1
			 << endl << endl << endl;




     total=0;
     for(day=1;day<=numdays;day++)
     {
         cout<<" Please enter the number of hours worked by student  "
         << student<<" on day"<<day<<" in biology "<<endl<<endl;
         cin>>numhours;
         total=total+numhours;
     }




     Average2 =total/numdays;
     cout<<endl;
     cout<<"The average number of hours spent per day biology by "
      << " student " << student << " is " << Average2
      <<endl<<endl<<endl;





	if (Average2 > Average1)
    {
        cout<< "Student" <<student<<" utilized more time studying biology as compared to programming "<<endl<<endl;
    }



    if (Average2 < Average1)
    {
        cout<< "Student "<<student<<" utilized more time studying programming as compared to biology "<<endl<<endl;
    }


    else if (Average2=Average1);
    {
     cout<<" Student "<<student<<" utilized the same amount of time studying programming and biology."<<endl<<endl;
    }



	}

	return 0;
}


```

6. **What is the take-away message from this bug?**

   After this error,I came to know about where and how to put the semicolon in if else statement.

---

# Bug 3 Q.19

1. **The incorrect original code or code snippit that you wrote:**

```
code with bugs or code snippet with bug goes here

code with bugs or code snippet with bug goes here
// This program finds the average time spent programming by a student
// each day over a three day period.

// PLACE YOUR NAME HERE

#include <iostream>
using namespace std;

int main()
{
	int numStudents;
	int numdays;
	float numhours, total, Average1,Average2;
	int student, day = 0;	// these are the counters for the loops

	cout << "This program will find the average number of hours a day"
		 << " that a student spent programming and biology over a long weekend\n\n";
	cout << "How many students are there ?" <<endl<<endl;
	cin >> numStudents;

	cout <<" Type the number of days in the long weekend" <<endl <<endl;
	cin >> numdays;

	for (student = 1; student <= numStudents; student++)
	{
		total = 0;

		for (day = 1; day <=numdays; day++)
		{
			cout << "Please enter the number of hours worked by student "
				 << student << " on day " << day << " in programming " << endl;
			cin >> numhours;

			total = total + numhours;
		}


		Average1=total/numdays;

		cout << endl;
		cout << "The average number of hours per day spent programming by "
			 << " student " << student << " is " << Average1
			 << endl << endl << endl;




     total=0;
     for(day=1;day<=numdays;day++)
     {
         cout<<" Please enter the number of hours worked by student  "
         << student<<" on day"<<day<<" in biology "<<endl<<endl;
         cin>>numhours;
         total=total+numhours;
     }




     Average2 =total/numdays;
     cout<<endl;
     cout<<"The average number of hours spent per day biology by "
      << " student " << student << " is " << Average2
      <<endl<<endl<<endl;





	if (Average2 > Average1)
    {
        cout<< "Student" <<student<<" utilized more time studying biology as compared to programming "<<endl<<endl;
    }



    if (Average2 < Average1)
    {
        cout<< "Student "<<student<<" utilized more time studying programming as compared to biology "<<endl<<endl;
    }


    else if (Average2=Average1)
    {
     cout<<" Student "<<student<<" utilized the same amount of time studying programming and biology."<<endl<<endl;
    }



	

	return 0;
}


```

2. **What bug does the original code have?**

   I did not close the bracket in the 90th line which(bracket) I started in the 26th line.

  

3. **What misunderstanding of C++ concepts lead you to this incorrect code?**

   I was not clear with the information to put the bracket before return 0 of  93rd line .

4. **How to correct the bug?**

   By closing the bracket the bug can be corrected.

5. **The corresponding bug-free code or code snippet is:**

```
bug-free code or code snippet goes here
code with bugs or code snippet with bug goes here
// This program finds the average time spent programming by a student
// each day over a three day period.

// PLACE YOUR NAME HERE

#include <iostream>
using namespace std;

int main()
{
	int numStudents;
	int numdays;
	float numhours, total, Average1,Average2;
	int student, day = 0;	// these are the counters for the loops

	cout << "This program will find the average number of hours a day"
		 << " that a student spent programming and biology over a long weekend\n\n";
	cout << "How many students are there ?" <<endl<<endl;
	cin >> numStudents;

	cout <<" Type the number of days in the long weekend" <<endl <<endl;
	cin >> numdays;

	for (student = 1; student <= numStudents; student++)
	{
		total = 0;

		for (day = 1; day <=numdays; day++)
		{
			cout << "Please enter the number of hours worked by student "
				 << student << " on day " << day << " in programming " << endl;
			cin >> numhours;

			total = total + numhours;
		}


		Average1=total/numdays;

		cout << endl;
		cout << "The average number of hours per day spent programming by "
			 << " student " << student << " is " << Average1
			 << endl << endl << endl;




     total=0;
     for(day=1;day<=numdays;day++)
     {
         cout<<" Please enter the number of hours worked by student  "
         << student<<" on day"<<day<<" in biology "<<endl<<endl;
         cin>>numhours;
         total=total+numhours;
     }




     Average2 =total/numdays;
     cout<<endl;
     cout<<"The average number of hours spent per day biology by "
      << " student " << student << " is " << Average2
      <<endl<<endl<<endl;





	if (Average2 > Average1)
    {
        cout<< "Student" <<student<<" utilized more time studying biology as compared to programming "<<endl<<endl;
    }



    if (Average2 < Average1)
    {
        cout<< "Student "<<student<<" utilized more time studying programming as compared to biology "<<endl<<endl;
    }


    else if (Average2=Average1)
    {
     cout<<" Student "<<student<<" utilized the same amount of time studying programming and biology."<<endl<<endl;
    }



	}

	return 0;
}


```

6. **What is the take-away message from this bug?**

After making this mistake,now I came to know about usage of brackets as I searched on google about that and I got my answer from www.quora.com .