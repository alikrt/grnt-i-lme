[m,n] = size(template);
[x,y] = size(image);
xFound = 0;
yFound = 0;
for i=1:(x-m)
for j=1:(y-n)
difference=0;
for k=1:m
for t=1:n
template_pixel = template(k,t);
image_pixel = image(k+i,t+j);
difference = difference + abs(image_pixel-template_pixel);
end
end
if (minDifference>difference)
minDifference=difference;
xFound = i;
yFound = j;
end
end
end
