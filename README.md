# Assignment-1
# 1) Using a for loop, print each job posting in a readable format.
To read the number of jobs i am using len function.
Now initializing the loop in 0 and printing all the values till it reaches the maximum number of jobs by incremneting with for loop 
# 2) Add New Job Postings (interactive)
 With a Input statement assigning to n i am getting number of postings from user.keeping n value in 
 for loop job_id gets maximum +1,
 job role we are getting from user,
 company we are getting from user,
 skills we are getting from user.later appending everything to the kist in the dictionary                                 
 # 3)  Clean & Normalize Skills (text processing)
 Defined an function clean_skills(skillstr). using lower to convert all skills in lowercase letter.Replace is removing , and replaces with some space " ".Split function Splits all the words in an sentence with join we are adding all skills into job_Data["skills"].
 # 4)Skill Extraction & Frequency
 Created Empty dictionary Skill_count.With Cleaned and Split skills into tokens.Checking skill exists or not. if skills exists
 increase count by 1 else add skill with count 1.By using lamda Sorts skills from highest frequency to lowest.with min of 5 prints top 5 skills
 # 5)Basic Statistics & Insights
 Using len to print total number of jobs with job_id.We are extracting skills from 1st job by split and also extracting skills from all the other jobs too. Converting the skills into Set to get only Unique values and finding its total by len . using if to find whether the given skill is there in which role.
# 6)Skill Search Function (functions & conditional logic)
 Defining a function called find_jobs_by_skill().To normalize the function input using lower and strip.Using for loop in range of total number of jobs we are creating a list with all the skills.Using if to print the job role where the given skill is present in created list.
# 7)  Lambda Filtering & List Comprehension
Split skills into Tokens,count skill frequencies by using get(j.lower(), 0).if skill not present it returns 0 /adds 1.using list comprehension to Store roles having at least one common skill(>=2).
# 8) Unique Skill Set
Create empty list skills.Splited skills into tokens.Added tokens to skills list.Cenverted list to Set to remove Duplicate values.Used Sort() to Sort skills alphabetically
# 9) Save Cleaned Data to File (file handling & exceptions)
Creates two files using file handling inside a try block. It writes all job details into job_skills.csv and stores the top 5 skills with their frequencies in top_skills.txt.
If any error occurs while creating or writing files, the except block displays the error message; otherwise, the else block prints "Files created"
