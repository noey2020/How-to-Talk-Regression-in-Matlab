# How-to-Talk-Regression-in-Matlab

September 16, 2020

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!

Hire me! 😊

% First generate a vector of x points, equally spaced in the interval [0,2.5], and then evaluate erf(x) at those points.

x = (0:0.1:2.5)';

y = erf(x);

% Determine the coefficients of the approximating polynomial of degree 6.

p = polyfit(x,y,6)

% To see how good the fit is, evaluate the polynomial at the data points and generate a table showing the data, fit, and error.

f = polyval(p,x);

T = table(x,y,f,y-f,'VariableNames',{'X','Y','Fit','FitError'})

% In this interval, the interpolated values and the actual values agree fairly closely. Create a plot to show how outside this interval, the extrapolated values quickly diverge from the actual data.

x1 = (0:0.1:5)';

y1 = erf(x1);

f1 = polyval(p,x1);

figure

plot(x,y,'o')

hold on

plot(x1,y1,'-')

plot(x1,f1,'r--')

axis([0  5  0  2])

hold off

I included some posts for reference.

https://github.com/noey2020/How-to-Get-Started-in-Matlab

https://github.com/noey2020/How-to-Convert-Data-from-Web-Service-Using-Matlab

https://github.com/noey2020/Quote-for-the-Day

https://github.com/noey2020/How-to-Talk-Good-Investment-Strategy

https://github.com/noey2020/How-to-Talk-of-Good-Plan

https://github.com/noey2020/Thought-for-the-Day

https://github.com/noey2020/How-to-Talk-Stock-Watch-of-the-Day

https://github.com/noey2020/How-to-Talk-Data-Science

https://github.com/noey2020/How-to-Talk-Fundamental-Analysis

https://github.com/noey2020/How-to-Read-Company-Profiles

https://github.com/noey2020/How-to-Import-Data-from-Spreadsheets-and-Text-Files-Matlab-Without-Coding

https://github.com/noey2020/How-to-Talk-Model-of-Stock-Market-Prices-

https://github.com/noey2020/How-to-Talk-Digital-Wallets

https://github.com/noey2020/How-to-Talk-Investing

https://github.com/noey2020/How-to-Double-Your-Money-in-5years

https://github.com/noey2020/How-to-Talk-Matlab

I appreciate comments. Shoot me an email at noel_s_cruz@yahoo.com!

Thanks for reading, and happy coding.

Hire me!

Noel
