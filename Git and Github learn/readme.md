this is a readme file.
........................................
U = Untracked
A = Added
C = committed

...........................................
git config --global user.name "Rajan Bhandari"

git config --global user.email "rajanbhandari4541@gmail.com"


//////yedi kei edit garnu pare default code editor vs code ho vaneko aani wait ko matlab terminal maa ma wait garirako xu jabasamma user ley tyo code end gardaina taba samma wait garxu vaneko(code lekhako matlab tei ho)
git config --global core.editor "code --wait"



//////////////////The command git config --global core.autocrlf "input" tells Git to convert line endings to LF (Unix-style) when committing, but leave them unchanged when checking out files. This helps keep line endings consistent across different systems.////////////////////


git config --global core.autocrlf "input"



//to edit the configuration.

git config --global -e 

...............................................
git log tells about all the commit histories.

to see each and every details about files:
git log run garni terminal maa. 

to check the checkpoint:
git log --oneline ---in terminal
........................................
to go in previous checkpoint:
git reset --hard HEAD~1  ---one step back

.............................................
to check the current status:
git status -s

note: git status only tells the status about the files which are not committed OR changed or modified after the commitment.

.............................................
to make a branch:
git branch "branch_name"
and
to see all the branch:
- git branch.
to switch between branches:
- git switch "branch_name"

yedi main bahek aaru branch baneko xaina bhane, ekipalta create pani ra branch switch garna ko lagi::
- git switch -C feature/addfooter
.........................................
to merge branches:
- git merge "branch_name"
-note::: to merge a branch we have to come to main branch first
..........................................
- merging techniques:
- fast forward merge::::: the first real file, the copy of real file 
and the changes made in that copy wala file. these three file are in used.
the first real file basically known as head is transferred to the file which was a changed copy of that real file. (the last file). tyo last file maa head transfer hunxa. this is called fast forward merging...
fast forward merge maa basically merge chai hudaina tara head ko location change matra hunxa(from first real to last the changed of the copied file)

- three way merge:::the real file, duplicate of real file and the real  file which was changed are three files. These 3 files give a new file by merging all of three is three way merge.
- squash merge
- recursive strategy merge
- rebase and merge

...........................................................
to delete a branch:
- git branch -d feature/navbar
...........................................................
stashing:
jab aap kisi branch mein kaam kar rahe ho and aapne kuchh code likha hai and aapne us code ko commit nahi kiya hai; aur aap doosri branch mein jaane ki kosis karte ho to git aako bolta hai ki bhai saved nahi hey changes delete ho jayenge. hum chhahe toh un changes ko delete honey dey yaa fir changes ko draft kar sakte hey. jab hum draft karengey, wo changes naa hi delete hongey naa hi add hongey. woo kahi bich mey dale rahengey fir aap us branch ko jaab chahe wo changes ko wapis se apply kar sakte hey.
now to stash:
- git stash...... garni aani jun branch maa jata pani switch huna paiyo ra feri back tei branch maa aayera stash garnu parxa by:
- git stash apply
aani commit garera feri
- git stash clear garni

>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>..
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>..
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>..
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

COMMON STEPS TO WORK IN GROUP AS A COLLABORATOR IN GITHUB::::
>>>>>>
1. main banda folder and initial files banaayegaa.
2. ab usse github par daal degaa
3. collaborators add karegaa
4.saare bande us repo se cloning karengey
5. [VERY IMP.]= aapni branch create karengey saare bandey.
6. apni code usi branch mey likhengey
7. jab apni code complete ho jaye to usko commit karengey and push karengey
8. inform karengey teammates ko about commit
9. merger banda fetch karegaa and merge karegaa and repush/merge karegaa..
>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
1. main banda boiler plate code yeta uti files banayera github maa repo banauxa:
2. aani usle vs code ko terminal maa following code run garni::::::
- echo "# testing test" >> README.MD
- git init
- git add README.MD
- git add .
- git commit -m "first commit by captain of group"
- git branch -M main
- git remote add origin "github_repo_ko_link"
- git push -u origin main


then aarko team member ley github repo ko link copy garera clone repository garxa vs code maa.

then, add collaborator and the email confirmation is sent
then, aapni branch create garxan: git switch -C "feature/navbar".
then, pahile make sure cd current folder maa hos.
then, git branch
then, main bahek aarko branch maa lekhnu paryo main lai chalauna vayena

then, code main bahek aarko branch maa lekhera jaba complete hunxa,
taba in terminal:::
- git add .
- git commit -m "added .... feature (basically a commit message)"
///////////////////yaha samma member ley saved checkpoint banako /////////////////////////////////

aaba, github maa push garna ko lagi::
- git push -u origin feature/navbar
aaba github maa check garda naya branch baneko hunxa

then, aaha samma main code disturb vako xaina

then, member ley captain lai maile commit and push gare vanxa


then, captain ley.....git fetch garxa terminal maa vs code ko
then, git branch to check...
then, git switch branchname.
then, captain check the whole code,
thenn, git switch main garxa captain ley
then, git merge branch name
then, adding code in main branch:::: git push origin main


code main branch maa ni vayo captain sanga pani vayo.. aba captain ley member lai vanxa a
then, member ley :: git switch main
then, git fetch
then, git pull,, fetch yaa pull j garepani tara pull better
note:: pull garepaxi merge garna pardaina, fetch garepaxi merge garna paryo






