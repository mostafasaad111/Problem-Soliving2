# Problem-Soliving2

## 1 - برنامج بيشوف القيمه اللي انت كاتبها لو رقم يطبعها لو لا بيرجع تاني يقولك اكتب الرقم مره اخري 

                    #include <iostream>
                    
                    using namespace std;
                    
                    int ReadNumber() {
                        int number;
                        cout << "Please enter number" << endl;
                        cin >> number;
                        while (cin.fail()) {
                    
                            cin.clear();
                            cin.ignore(std::numeric_limits<std::streamsize>::max(), '\n');
                            cout << "Invalid Number, Enter a valid one:" << endl;
                            cin >> number;
                    
                        }
                        return number;
                    
                    }
                     
                    int main()
                    {
                        
                        cout << "yes number is " << ReadNumber();
                         return 0;
                    }

                    
## 2 - مثال علي ال Range Loop 

        #include <iostream>
        
        using namespace std;
        
        
         
        int main()
        {
            
            int arr[] = { 1,2,3,4,34,4,3,5,3,4 };
            for (int n : arr) {
                cout << n << endl;
            }
             return 0;
        }

## 3 - مثال علي الجمع بال AND , OR 

        #include <iostream>
        
        using namespace std;
        
        int main()
        {
            cout << (12 & 25) << endl; // AND
            cout << (12 | 25) << endl; // OR
        
        }


        
## 4 -  Declaration Vs Definition

          #include <iostream>
          
          using namespace std;
          
          int sum(int a, int b); //function declaration
          
          int main()
          {
             
          	cout << sum(10, 20);
          
          }
          int sum(int a, int b) {  ////function definition
          	int c = a + b;
          	return c;
          }

## 5 - default parameters

          #include <iostream>
          
          using namespace std;
          
          int sum(int a, int b, int c = 0, int d = 0) {  // default parameters
          	
          	return (a + b + c + d);
          }
          
          int main()
          {
          	cout << sum(10, 20) << endl; 
          	cout << sum(10, 20, 3) << endl;
          	cout << sum(10, 20, 3, 23) << endl;
          
          	return 0;
          }

## 6 - 














