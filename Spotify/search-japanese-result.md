Spotify search API on curl command doesn't returns same artist name's characters as Spotify developer console.
If you want to get same result, you shuld apply Accept-Language header on the command 

```
curl -X "GET" "https://api.spotify.com/v1/search?q=Kendrick%20Lamar&type=artist&market=JP" -H "Accept: application/json" -H "Content-Type: application/json" -H "Authorization: Bearer  <Token>" -H "Accept-Language: ja;q=1"
```

https://github.com/spotify/web-api/issues/1023#issuecomment-452638826
