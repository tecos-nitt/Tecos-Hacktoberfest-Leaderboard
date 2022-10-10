# Tecos-Hacktoberfest-Leaderboard
The offical leaderboard for TeCOS-Hacktoberfest event.

[Hacktoberfest](https://hacktoberfest.com/) is a yearly event encouraging people to contribute to open source in October. We, the community of TeCOS, will power you up with mentors to guide and assist you in this journey.

Happy Hacking!!

## Configuring the app
Configuration is exclusively done by setting environment variables:
* `PORT` : The port to bind HTTP to. Default port is `8080`
* `GH_TOKEN` : The token to authenticated to github. By default, no token is used, so API calls are not authenticated.
* `EVENT_DATE` : The date to restrict contribution search to. It must follows the github search date format (more details [here](https://help.github.com/articles/understanding-the-search-syntax/#query-for-dates)). Default value is `>=2005` which basically fetch everything without any restriction
* `PARTICIPANTS_FILE` : The URI or file path to the file containing the participants' github usernames.
* **[Deprecated]** `OBJECTIVE` : Number of pull requests to make in order to complete the challenge. Default value is `4`

> If the app is running behind a proxy, you'll need to set both environment variables `HTTP_PROXY` and `HTTPS_PROXY` before running it

## Building & Running the app

Make sure you have [go](http://go.dev) installed and then build the application by running
```bash
    go build .
```

Then run the following command
```bash
    ./leaderboard
    # or
    ./leaderboard.exe
```
then run it locally in http://localhost:8080
