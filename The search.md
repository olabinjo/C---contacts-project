C---contacts-project
====================

Searching through a string array

     
       cout << "Enter the full name of the contact you want to search"<<endl;
       getline(cin, searchTerm);  

	readFile.open("C:\\Users\\BANJO\\Dropbox\\Valleyview\\book.txt");	


	
	for (int j=0; j< noOfContacts; j++)
	{		
       
	for (int count=0; count < 5; count++)
	{
		switch(count)
		{
			
		case (0): 		
			getline(readFile,name[j]);
			//cout<<"NAME:  "<< name[j]<<endl;break;
		
		case (1):
					getline(readFile,birth[j]);
		//cout<<"BIRTHDAY:     "<< birth[j]<<endl; break;
		case (2):	
			getline(readFile,address[j]);
			//cout<< "ADDRESS:       "<<address[j]<<endl; break;	
		case (3):
			getline(readFile,workplace[j]);
			//cout<< "WORKPLACE:      "<<workplace[j]<<endl; break;			
		case (4):
			getline(readFile,phone[j]);
			//cout<< "PHONE NUMBER:    "<<phone[j]<<endl; 
		
		
       			
		
		if(searchTerm.compare(name[j]) == 0)
		{
			cout << "NAME" << setw(15) << name[j] <<endl;
			cout << "PHONE NUMBER" << setw(10)<<phone[j]<<endl;
			cout << "ADDRESS" << setw(15)<<address[j]<<endl;
			cout << "BIRTHDAY" << setw(10)<<birth[j]<<endl;
			cout << "WORKPLACE" << setw(15)<<workplace[j]<<endl;
			return;
		}
		
		
        }
           
            
		break;
	}
	}
