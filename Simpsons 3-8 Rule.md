# Numerical-method-Codes
# Simpsons 3/8 rule
function  x=simpsons38( a, b, n)
  printf("Roopam Bhardwaj,14150138\n");
  h = (b - a)/ n;
  s = f(a) + f(a + n*h)+3*(f(a+h)+f(a+2*h));
  for i = 3: 3: n-3
    s = s + 3*f(a+(i+1)*h)+2*f(a + (i)*h);
  end
  fprintf("The value of a is:%d \n",a);
  fprintf("The value of b is:%d \n",b);
  fprintf("The value of n is:%d \n",n);
  fprintf("The value of the function is:%f\n", 3*s*h/8);
end

function f = f(x)
  f = (sqrt(sin(x)))/((sqrt(sin(x)))+(sqrt(cos(x))));
end
