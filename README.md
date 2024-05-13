# Data_Final_project

FAST NATIONAL UNIVERISTY OF COMPUTER AND EMERGING SCIENCES


 
Introduction: The GitHub simulation project in C++ presents a comprehensive platform emulating core functionalities of the real GitHub system. Designed to facilitate user account management, repository creation, file management, and user interactions, this project offers a hands-on experience in understanding version control, collaborative development, and social networking aspects akin to GitHub. Through this simulation, users delve into creating, managing, and collaborating on repositories, enhancing their skills in software development practices and fostering a deeper understanding of modern version control systems.Our  project include “Social network .cpp” , “Repository.cpp” , “Hash- Table.cpp” and “Project.cpp” and their Header files respectively. 

Social network.cpp: 
 

 

Got it! Here's the structured information about the Social Network Management System as described in your document:
1. Adding new users to the system.
2. Loading user data from a CSV file.
3. Saving user data to a CSV file.
4. Retrieving the total number of users and user lists.

 Connection Management:
1. Following other users.
2. Unfollowing users.
3. Checking if a user is following another user.
4. Retrieving following lists and followers count.

 Implementation Details
**Class Structure**
- **SocialNetwork:** Represents the core functionality of the social network system.

**Data Members:**
- **users_count:** Total number of users in the system.
- **UsersList:** Array to store user names.
- **UserFollowing:** Array of vectors to store the following lists for each user.

**Constructor:**
- Initializes data members and dynamically allocates memory for user data.

**Member Functions:**
- **getTotalUsers():** Returns the total number of users.
- **getUserIndex(string usr):** Returns the index of a user in the UsersList array.
- **loadData():** Loads user data from a CSV file.
- **getFollowingList(string usr):** Retrieves the following list for a user.
- **getFollowersCount(string user):** Returns the count of followers for a user.
- **saveData():** Saves user data to a CSV file.
- **addNewUsr(string usr):** Adds a new user to the system.
- **IsFollowing(string usr, string follow_user):** Checks if a user is following another user.
- **AddToFollowingList(string usr, string follow_user_name):** Adds a user to the following list.
- **UnfollowUser(string usr, string following_user_name):** Removes a user from the following list.
- **getUserList():** Retrieves the list of all users.

**Destructor:**
- Frees memory allocated for user data.

This structure outlines the functionalities and class design of the Social Network Management System as described in your document.

Hash_table.cpp:
 
Constructor
- Initializes the hash table with a specified maximum length.

Member Functions
1. **getUserCount()**
   - Returns the total number of user accounts in the hash table.
   
2. **getLength()**
   - Returns the maximum length of the hash table.
   
3. **getUserAtIndex(int i)**
   - Returns the user account at a specified index in the hash table.
   
4. **checkDataExists(UserAcc data)**
   - Checks if a given user account data exists in the hash table.
   
5. **checkUserExists(string usr_name)**
   - Checks if a user with a specified username exists in the hash table.
   
6. **RegisterNewUser(UserAcc usr)**
   - Registers a new user account in the hash table.
   
7. **InsertData(UserAcc data)**
   - Inserts user account data into the hash table.
   
8. **DeleteData(UserAcc data)**
   - Deletes user account data from the hash table.
   
9. **LoadData()**
   - Loads user account data from a CSV file into the hash table.
   
10. **SaveData()**
    - Saves user account data from the hash table to a CSV file.
    
11. **IsNearFull()**
    - Checks if the hash table is nearing full capacity and extends its size if necessary.
    
12. **hashKey(UserAcc data)**
    - Calculates the hash key based on a user account's username.
    
13. **DisplayUserName(int index)**
    - Displays the username of a user account at a specified index in the hash table.
    
 Destructor
- Deallocates memory for the hash table.

Repository.cpp:
 

 
Class: LinkedList

**Purpose:** Represents a simple linked list used for storing file names and commit messages.

**Member Variables:**
- **ListNode:** Represents a node in the linked list containing a string data and a pointer to the next node.
- **head:** Pointer to the first node in the linked list.
- **listSize:** Stores the number of nodes in the linked list.

**Member Functions:**
1. `Insert(string str):` Inserts a new node with the given string data into the linked list.
2. `Delete(string str):` Deletes a node with the given string data from the linked list.
3. `getSize():` Returns the size of the linked list.
4. `getDataAt(int index):` Returns the data at the specified index in the linked list.

 Class: Repository

**Purpose:** Represents a repository within the management system.

**Member Variables:**
- **root:** Pointer to the root node of the repository's binary search tree.
- **OwnerName:** Stores the owner's name of the repository.

**Member Functions:**
1. `getHeight(Node* node):` Returns the height of a given node in the repository's binary search tree.
2. `getBalance(Node* node):` Returns the balance factor of a given node in the repository's AVL tree.
3. `setPrivateStatus(Node* node, string repo_name, bool status):` Sets the private status of a repository.
4. `rightRotate(Node* y):` Performs a right rotation on a given node in the repository's AVL tree.
5. `leftRotate(Node* x):` Performs a left rotation on a given node in the repository's AVL tree.
6. `Add_File(Node* node, string repName, string fileName, string commit_msg):` Adds a file or commit message to a repository.
7. `minValueNode(Node* node):` Finds the node with the minimum value in a given subtree of the repository's AVL tree.
8. `ForkRepository(Node* node, string repo_name, Repository& repo):` Forks a repository into a new repository.
9. `deleteRepo(Node* root, string repoName):` Deletes a repository from the management system.
10. `deleteFileFromRepo(Node* node, string repoName, string fileName, string commit_msg):` Deletes a file from a repository.
11. `saveData(Node*& node):` Saves repository data to a file.
12. `inorderTraversalSave(Node* node):` Performs an inorder traversal of the repository's AVL tree and saves data to a file.
13. `inorderTraversalRepoGrab(Node* node, vector<string>& vect):` Performs an inorder traversal of the repository's AVL tree and collects repository names.
14. `getRepoRecurr(Node* node, string name):` Recursively searches for a repository by name.
15. `CreateANewRepo(string repoName):` Creates a new repository.
16. `Add_File(string repoName, string fileName):` Adds a file to a repository.
17. `Add_Commit_Msg(string repoName, string commitMsg):` Adds a commit message to a repository.
18. `ForkARepository(string repo_name, Repository& repo):` Forks a repository.
19. `LoadData(string Owner):` Loads data from a file into the management system.
20. `SaveData():` Saves data from the management system to a file.
21. `getRepo(string name):` Retrieves a repository by name.
22. `getRepoList():` Retrieves a list of repository names.

This structured breakdown outlines the purpose, member variables, and member functions of the `LinkedList` and `Repository` classes as described in your provided information.


Project.cpp:

 
 Introduction
The program is a command-line social network with GitHub-like features, allowing users to register accounts, log in, manage repositories, follow/unfollow users, and more.
 Global Variables
- **AccountsList:** Hash table storing user account information.
- **socialnetwork:** Manages social network functionalities.
- **repository:** Array of repositories for each user.

 Functions
1. **InitialLoading()**
   - **Purpose:** Loads initial data from files into memory.
   - **Operations:**
     - Loads user accounts from a file into `AccountsList`.
     - Loads social network data from a file into `socialnetwork`.
     - Creates repositories for each user in the social network.

2. **DisplayUsersList(vector<string> userslist)**
   - **Purpose:** Displays a list of users.
   - **Parameters:**
     - `userslist`: A vector containing usernames to be displayed.

3. **ViewMenu()**
   - **Purpose:** Displays the main menu and handles user input.
   - **Operations:**
     - Provides options to register a new account, login, or exit the program.

4. **RegisterAnAccount()**
   - **Purpose:** Allows users to register a new account.
   - **Operations:**
     - Takes user input for username and password.
     - Checks for username uniqueness and registers the new account if valid.

5. **LoginIntoAnAccount()**
   - **Purpose:** Allows users to log in to an existing account.
   - **Operations:**
     - Takes user input for username and password.
     - Validates the credentials against existing accounts.

6. **LoggedInUserOptions()**
   - **Purpose:** Handles options available to a logged-in user.
   - **Operations:**
     - Displays options to view profiles, manage GitHub-like functionalities, or log out.

7. **ManageGitHub()**
   - **Purpose:** Manages GitHub-like functionalities for a logged-in user.
   - **Operations:**
     - Allows viewing, creating, editing repositories, viewing following users, etc.

8. **ViewRepository(vector<string> repo_list, int index)**
   - **Purpose:** Displays details of a user's repository.
   - **Parameters:**
     - `repo_list`: A vector containing repository names.
     - `index`: Index of the user in the repository array.

9. **ShowUserGitHub(string user)**
   - **Purpose:** Displays GitHub-like functionalities for a user.
   - **Parameters:**
     - `user`: Username of the user.

Main Functionality
- **Registration/Login:** Users can register new accounts or log in with existing credentials.
- **Profile Management:** Logged-in users can view other profiles and perform related actions.
- **GitHub-like Features:** Users can manage repositories, view, add, remove files, change repository status, follow/unfollow other users, and view their GitHub profiles.

This breakdown outlines the core functionalities and operations of your command-line social network program with GitHub-like features.

















