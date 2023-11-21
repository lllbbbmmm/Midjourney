
## Midjourney
Connect your project to midjourney | mj contain generate、upsample、variation…

Connect your project to midjourney contain generate、upsample、variation
Support async or query for the generate and action jobs.
More convenient and stable.

## How to use


- If you have any questions, please contact me at 850784744@qq.com and  nb429429@gmail.com
 

```angular2
// php
<?php

$curl = curl_init();

curl_setopt_array($curl, [
	CURLOPT_URL => "https://midjourney-api6.p.rapidapi.com/createImagesFast?prompt=A cat in armor&aspect_ratio=1%3A1&callback_url=https%3A%2F%2Fwww.google.com%2F",
	CURLOPT_RETURNTRANSFER => true,
	CURLOPT_ENCODING => "",
	CURLOPT_MAXREDIRS => 10,
	CURLOPT_TIMEOUT => 30,
	CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
	CURLOPT_CUSTOMREQUEST => "GET",
	CURLOPT_HTTPHEADER => [
		"X-RapidAPI-Host: midjourney-api6.p.rapidapi.com",
		"X-RapidAPI-Key: 8770757a48mshabcf4b117c82442p1fe9c8jsn7665fdf25ced"
	],
]);

$response = curl_exec($curl);
$err = curl_error($curl);

curl_close($curl);

if ($err) {
	echo "cURL Error #:" . $err;
} else {
	echo $response;
}
```

```angular2
// python 
import requests

url = "https://midjourney-api6.p.rapidapi.com/createImagesFast"

querystring = {"prompt":"A cat in armor","aspect_ratio":"1:1","callback_url":"https://www.google.com/"}

headers = {
	"X-RapidAPI-Key": "8770757a48mshabcf4b117c82442p1fe9c8jsn7665fdf25ced",
	"X-RapidAPI-Host": "midjourney-api6.p.rapidapi.com"
}

response = requests.get(url, headers=headers, params=querystring)

print(response.json())
```

```angular2
// respones
{
task_id:"76c2bab7-6d40-42d6-a42d-5773e53295a9"
status:"success"
message:""
}
```  
