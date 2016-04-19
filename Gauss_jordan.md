# Numerical-method-Codes
# Gauss Jordan Method
function [x]= gjordan(a)
printf("Roopam Bhardwaj,14150138\n");
[m,n]=size(a)
display('a=')
display(a)

for j=1:m
  for i=1:m
    if(i!=j)
      c=a(i,j)/a(j,j);
      for k=1:m+1
      a(i,k)=a(i,k)-(c*a(j,k));
      end
    end
  end
end
display('diagnol form')
display(a)
for i=1:m
x(i)=a(i,m+1)/a(i,i);
fprintf(1,'x(%d)=%e \n',i,x(i));
end  
