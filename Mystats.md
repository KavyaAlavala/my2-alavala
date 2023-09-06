# Kavya Alavala
 I have recently  completed my bachelors.From my childhood, my aim is to do masters in USA and now i acheived it.Present my aim after completion of my masters to return back India and to start my own startup company and wanted to settle with my family and friends.


![myimage](image/my_image.jpg)

****

# Sports
A human activity involving physical exertion and skill as the primary focus of the activity, with elements of competition or social participation where rules and patterns of behaviour governing the activity exist formally through organisations and is generally recognised as a sport.It reduces mental stress.

|Sport Name|Reason|Hours|
|----------|------|-----|
|Golf|focus,entertainment|2|
|Kabbadi|Stress Relief,body stretch|3|
|Badminton|Improves Flexibilty and mobility|2|
|Hockey|hepls to burn fat|4|


****

# Quotes

>“Everything is theoretically impossible until it is done.” – Robert A. Heinlein

>"The important thing is not to stop questioning." - Albert Einstein

>"The more I learn, the more I realize how much I don't know." - Isaac Newton


# Code Fencing:

___Link to the Stack Overflow:___
https://stackoverflow.com/questions/39730856/symfony-php-template-custom-error-page

htaccess code:
```
<?php

$status=$_SERVER['REDIRECT_STATUS'];
$codes=array(
      400 => array('400 Bad Request', 'The request cannot be fulfilled due to bad syntax.'),
      401 => array('401 Login Error', 'It appears that the password and/or user-name you entered was incorrect.'),
      403 => array('403 Forbidden', 'Sorry, employees and staff only.'),
      404 => array('404 Missing', 'We\'re sorry, but the page you\'re looking for is missing, hiding, or maybe it moved somewhere else and forgot to tell you.'),
      405 => array('405 Method Not Allowed', 'The method specified in the Request-Line is not allowed for the specified resource.'),
      408 => array('408 Request Timeout', 'Your browser failed to send a request in the time allowed by the server.'),
      414 => array('414 URL To Long', 'The URL you entered is longer than the maximum length.'),
      500 => array('500 Internal Server Error', 'The request was unsuccessful due to an unexpected condition encountered by the server.'),
      502 => array('502 Bad Gateway', 'The server received an invalid response from the upstream server while trying to fulfill the request.'),
      504 => array('504 Gateway Timeout', 'The upstream server failed to send a request in the time allowed by the server.'),
);

$errortitle=$codes[$status][0];
$message=$codes[$status][1];

if($errortitle==false){
       $errortitle="Unknown Error";
       $message="An unknown error has occurred.";
}

?>
<!doctype html>
<html>
<head>
<title><?php echo("$errortitle");?></title>
<meta charset="utf-8">
</head>
<body>

<!-- Insert headers here. -->

<?php
echo('<h1>'.$errortitle.'</h1>');
echo('<p>'.$message.'</p>');
?>

<!-- Insert footers here. -->

</body>
</html>