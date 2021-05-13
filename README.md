# LoL Mastery Grinder

A web app that takes in your League of Legends summoner name, region, and position and returns which champion in that role you have the lowest mastery score with.

# Running the Project

## Riot Games API
To run this project with your own key, add a file called `riot-api-key.txt` at the root of this repo and paste your api key in it.

Limitations on requests enforced by Riot:
- 20 requests every 1 seconds(s)
- 100 requests every 2 minutes(s)

## Startup

From the root of the repository, build the docker image:

```
 docker build -t mastery-grinder .
```

Then run the image with
```
docker run -dp 3000:3000 mastery-grinder
```

The app can be accessed locally at http://localhost:3000/.
