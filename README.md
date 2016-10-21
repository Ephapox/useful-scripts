# useful-scripts

#### Delete multiple github repositories based on a repos.txt file where each repo is one its own line and in the format \<user_name>/\<repo_name>
```
while read repo; do curl -X DELETE -H "Authorization: token UR_TOKEN" "https://api.github.com/repos/$repo"; done < repos.txt
```
