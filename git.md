 Learn git

 Installation  

1 :-> git config --global user.name "name"
2 :-> git config --global user.email"email@male.com"
3 --> git config --global core.editor "code --wait"
4 --> git config --global core.autocrlf

stages :-
     U --> Untracked 
     A --> added or staged
     C --> Commited

---------------------------------------------------

---->   here are 3 types of goback and check the pervious and reset the previous datav
          -- > git reset --hard 
          --> git reset --SOFT
          --> git reset --MIXEd 

---------------------------------------------------

git status -s --> check kr skte h konsi file kis stage m hai 

git status -s sirf unka status btata h jo files committed nhi h ya fir commit hone k bad change ho gyi h jese commit krne k bad delete kr di ya modify

git status btata h file k changes k bare m and uske chages k bare m before commit or after commit 

--------------------------------------------------

git log --oneline --graph --> check kr skte h kitni saved checkpoints hai 

git log btata h sare commit history 

------------------------------------------------------------------------------------

# branching  --> git branch feature/textandbranchlearning

branching means work on the copy of main file and after completition and check the work we can add main file 


 git switch main


--------------------------------------------------------------------------------------

 get merge file branch name

 branch merge krna 

 merging techniqies ---> fastforward merge(ff) , three way , squash merging, recursice strategy merge , rebase and merge

--------------------------------------------------------------------------------------

How to delete the Branch ---> git branch -d here write branch name 

-----------------------------------------------------------------------------------------

# Stashing ----------> jab aap kisi branch mein kam kr rhe ho and apne kuch code likha hai and aapne us code ko commit nhi kiya hai , aur aaap dusri branch mein jane ki koshisb krte ho to got aapko bolta hai ki saved nhi change delete ho jaenge hm chahe to un changes ko delete hone de yaa fir un changes ko draft kr skte hai , jab bhi draft krenge to wo changes naa hi delte honge na hi add honge but beech mein khi dale rahenge fir aap us branch mein jab wappas aaye to wo changes waapas se apply kr skte ho

# kese stash krenge----> git stash 


Git Stashing is a process of temporarily saving your uncommitted changes so that you can work on something else without committing those changes.

1. Real-life example

Maan lo tum Java project par kaam kar rahe ho.

Step 1: Coding kar rahe ho

Student.java me changes kiye, lekin code complete nahi hua.

Step 2: Urgent task aa gaya

Tumhe dusri branch par jaakar bug fix karna hai.

Step 3: Changes stash kar do

Incomplete changes temporarily save ho jayenge aur working directory clean ho jayegi.

Step 4: Changes wapas lao

Bug fix karne ke baad apne previous changes restore kar lo.


# 1. Current changes check karo
git status

# 2. Changes temporarily save karo
git stash push -m "My incomplete Java work"

# 3. Ab dusra task complete karo
git switch main

# 4. Jab original branch par wapas aana ho
git switch feature-branch

# 5. Changes restore karo
git stash pop