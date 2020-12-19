
HTML File:

<html>
<body>
<center>
<h1><b>hello world... </b></h1>
<p>today is {{today}} </p>
</center>
</body>
</html>

Django File:

def hello(request):

today = datetime.datetime.now().date() 
return render(request,"hello.html", {"today" : today}) 
