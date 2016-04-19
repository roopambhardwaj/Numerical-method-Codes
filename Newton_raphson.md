# Numerical-method-Codes
# Newton raphson method

functionx=newton
printf("Roopam Bhardwaj,14150138\n");
x=0.5;
t=1;
while(abs(t-x)<0.001)
y=x-f(x)/df(x);
t=x;
x=y;
end
printf("Answer is %.3f\n",x);
end
function a=f(x)
a=x^3-4*x-9;
end
function b=df(x)
b=3*(x^2)-4;
end
