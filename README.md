<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>Ordenador de Serie</title>
</head>
<body>
	
<script>

var a, b, c;

a = parseInt(prompt('Ingresar numero:',''));
b = parseInt(prompt('Ingresar numero:',''));
c = parseInt(prompt('Ingresar numero:',''));

if(a==b){
    if(b==c)
        document.write('Los números son iguales');
    else if(b>c)
        document.write('Los dos primeros son iguales y el orden es: ',a,'=',b,'>',c);
    else
        document.write('Los dos primeros son iguales y el orden es: ',c,'>',a,'=',b);
}

else if(a==c){
    if(a>b)
        document.write('El primero y tercero son iguales y el orden es: ',a,'=',c,'>',b);
    else
        document.write('El primero y tercero son iguales y el orden es: ',b,'>',a,'=',c);
}

else if(b==c){
    if(b>a)
        document.write('El segundo y tercero son iguales y el orden es: ',b,'=',c,'>',a);
    else
        document.write('El primero y tercero son iguales y el orden es: ',a,'>',b,'=',c);
}

else if((a>b)&&(b>c))
    document.write('El orden es: ',a,'>',b,'>',c);
else if((a>c)&&(c>b)) 
    document.write('El orden es: ',a,'>',c,'>',b);
else if((b>a)&&(a>c))
    document.write('El orden es: ',b,'>',a,'>',c);
else if((b>c)&&(c>a))
    document.write('El orden es: ',b,'>',c,'>',a);
else if((c>a)&&(a>b))
    document.write('El orden es: ',c,'>',a,'>',b);
else if((c>b)&&(b>a))
    document.write('El orden es: ',c,'>',b,'>',a);

</script>

</body>
</html>
