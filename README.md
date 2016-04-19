# Numerical-method-Codes
#Program for Bisection:-

function x=bisection(a,b)
printf("Roopam Bhardwaj , 14150138 \n"); 
tol=0.001
fa=fun(a)
fb=fun(b)
i=0;
while(abs(a-b))>tol
    x=(a+b)/2;
i++;
if fun(a)*fun(x)<0
      b=x;
else
      a=x;
end
printf(" %d iteration= %f \n", i, x);

end
end
function f=fun(x)
  f=x^3-4*x-9;
end
