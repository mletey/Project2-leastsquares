# Project2-leastsquares
PSI 2023 Numerical Methods Course - Project 2

All answers contained in Project 2 ipynb file, which should run without any additional fuss so long as the user has WGLMakie and LinearAlgebra downloaded. To do so, add two additional block at the beginning of the notebook and write in them
"]add WGLMakie"
and
"]add LinearAlgebra"

This notebook fits a function, namely sine(x), by using a finite polynomial approximation of various degree. The polynomial is fit using a least squares interpolation, and we measure the error in our approximation using the L2 norm. The code is adjustable to fit a different function of the user's choice, by modifying Block 3, targetfunc(x) value. 
<img width="1054" alt="Screenshot 2023-04-12 at 12 34 34" src="https://user-images.githubusercontent.com/118086545/231523576-94e061e4-e36e-4a34-af4b-9cc8c4a12d2e.png">

Other modifiable parameters are seen in the above image, which the user can specify as desired. "pmax" gives the degree of the polynomial, i.e. the largest x^n term in the approximation. "npoints" gives the number of points used to divide the x-axis during the least squares interpolation process. "rangestart" and "rangeend" specify the range over which the function is fit to the polynomial, and in this range, error will be low. Outside this range, error will diverge. Both of these phenomena are demonstrated in blochs 5 and 6 on ranges 0 to pi, and 0 to 2pi for targetfunc(x) = sine(x) fit on the range 0 to pi/2.

<img width="424" alt="Screenshot 2023-04-12 at 12 41 42" src="https://user-images.githubusercontent.com/118086545/231525413-98d1c9e9-9ffa-4352-8c65-56734e1f7b75.png">
<img width="409" alt="Screenshot 2023-04-12 at 12 41 50" src="https://user-images.githubusercontent.com/118086545/231525415-53b8ee9e-cae2-4028-86d5-20ca9cb7c425.png">



