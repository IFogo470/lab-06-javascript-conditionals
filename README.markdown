v314-ent-011:~ student$ cd ~/Desktop
v314-ent-011:Desktop student$ mkdir Ian
v314-ent-011:Desktop student$ cd Ian
v314-ent-011:Ian student$ mkdir lab-06-javascript-conditionals
v314-ent-011:Ian student$ cd lab-06-javascript-conditionals
v314-ent-011:lab-06-javascript-conditionals student$ pwd
/Users/student/Desktop/Ian/lab-06-javascript-conditionals
v314-ent-011:lab-06-javascript-conditionals student$ ls -al
total 0
drwxr-xr-x  2 student  staff   68 Oct 21 15:01 .
drwxr-xr-x  3 student  staff  102 Oct 21 15:01 ..
v314-ent-011:lab-06-javascript-conditionals student$ git init
Initialized empty Git repository in /Users/student/Desktop/Ian/lab-06-javascript-conditionals/.git/
v314-ent-011:lab-06-javascript-conditionals student$ la -al
-bash: la: command not found
v314-ent-011:lab-06-javascript-conditionals student$ ls -al
total 0
drwxr-xr-x  3 student  staff  102 Oct 21 15:03 .
drwxr-xr-x  3 student  staff  102 Oct 21 15:01 ..
drwxr-xr-x  9 student  staff  306 Oct 21 15:03 .git
v314-ent-011:lab-06-javascript-conditionals student$ ls .git
HEAD		config		description	hooks		info		objects		refs
v314-ent-011:lab-06-javascript-conditionals student$ git config user.name "IFogo470"
v314-ent-011:lab-06-javascript-conditionals student$ git config user.email "ian.fogo@mail.citytech.cuny.edu"
v314-ent-011:lab-06-javascript-conditionals student$ git config -l
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
core.ignorecase=true
core.precomposeunicode=true
user.name=IFogo470
user.email=ian.fogo@mail.citytech.cuny.edu
v314-ent-011:lab-06-javascript-conditionals student$ curl -u 'IFogo470' https://api.guthub.com/com/user/repos -d '{"name":"lab-06-javascript-conditionals"}'
Enter host password for user 'IFogo470':
curl: (6) Could not resolve host: api.guthub.com
v314-ent-011:lab-06-javascript-conditionals student$ curl -u 'IFogo470' https://api.github.com/user/repos -d '{"name":"lab-06-javascript-conditionals"}'
Enter host password for user 'IFogo470':
{
  "message": "Repository creation failed.",
  "errors": [
    {
      "resource": "Repository",
      "code": "custom",
      "field": "name",
      "message": "name already exists on this account"
    }
  ],
  "documentation_url": "https://developer.github.com/v3/repos/#create"
}
v314-ent-011:lab-06-javascript-conditionals student$ git remote -v
v314-ent-011:lab-06-javascript-conditionals student$ git remote add origin https://github.com/IFogo470/lab-06-javascript-conditionals.git
v314-ent-011:lab-06-javascript-conditionals student$ git remote -v
origin	https://github.com/IFogo470/lab-06-javascript-conditionals.git (fetch)
origin	https://github.com/IFogo470/lab-06-javascript-conditionals.git (push)
v314-ent-011:lab-06-javascript-conditionals student$ git status
On branch master

No commits yet

nothing to commit (create/copy files and use "git add" to track)
v314-ent-011:lab-06-javascript-conditionals student$
