# cocos2d_network

For cocos2d-x-2.1.5, HttpClient & HttpRequest, it doesn't support upload file via FORM.

So I add FORM uploading file function into it via curl. You can just merge these files into cocos2d-x-2.1.5\extensionsnetwork.

For better test your uploading file feature, you can upload file to below online http server:
http://posttestserver.com/
http://posttestserver.com/post.php

post file only:
curl -v -F file=@main.h http://posttestserver.com/post.php

post file and params:
curl -v -F skey=123456 -F file=@text.txt http://posttestserver.com/post.php
