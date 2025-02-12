IN ELKSTACK ubuntu vm
Go to 
http://localhost:5601 in web browser

Login with this username and password
```
username: 
elastic
pass: 
0olw6pqS78Su53xPwU*0
```

In WEBSERVER ubuntu vm
Go to http://localhost/DVWA
login: 
admin
password

output {
  elasticsearch {
    hosts => ["https://localhost:9200"]
    user => "elastic"
    password => "0olw6pqS78Su53xPwU*0"
    ssl => true
    ssl_certificate_verification => false
  }
}

elastic:0olw6pqS78Su53xPwU*0

https://tap.group-ib.com/api/v2/attacks/phishing_group

ps -ef | grep logstash
sudo kill -9 <pid from prevoius command>
