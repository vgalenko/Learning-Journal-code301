# LJ Code 301 - Day 13

Yesterday we learned about REST API's. We accessed our personal GitHub API by using a jQuery ajax request. It retrieved all of the data about my repos. Here is a pretty simple but yet, one of the most common ways to retrieve API's into local server. 

```
GitHub API request Example: 
$.ajax({
	url: 'https://api.github.com/user/repos',
	method:'GET',
	headers: {
		Authorization: 'token ecbf050fa6ce22046c1e4028c4a0199ca034af92'
	} 
}).then(data => console.log(data.name)); //that will retrieve all of the names of my repos 

If we are deploying a website and want to retrieve this data, we would have to use .get() like so:

$.get('/github/user/repos')
    .then(data => repos.all = data, err => console.error(err)) //
    .then(callback);

function proxyGitHub(request, response) {
  (requestProxy({
    url: `https://api.github.com/${request.params[0]}`,
    headers: {Authorization: `token ${process.env.GITHUB_TOKEN}`} //add GITHUB_TOKEN in Heroku 
  }))(request, response);
}
```

Today we learned how to deploy our websites with Heroku. It was extremely simple and it took only a few command lines.  
```
Example:
heroku create (desired app name) // that creates the name of the app 
git push heroku master // that will push your repo to Heroku website
```
Note: Its very important that your package.json file is exposed and anchored in the root of the file path because when Heroku receives your files through "git push" it will look for a package.json and if it can't find it because its buried in other files then unfortunately it won't deploy. 

Make sure that you merge your Github Repo into your master, as well as your local branches into master branch. You will always want to push from your master branch. 
