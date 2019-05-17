<h1> Performance Lab Keegan Mullins

<h3> The purpose of this lab was to create code that would apply filters to an image as optimally (time-wise) as possible.

<h3> This code utilizes many different techniques in order to most optimally perform the calculations for the filter on the image. The filters themselves can be found as the files labeled "x.filter" where x is some filter name. Each is a 3 by 3 matrix with various numbers in it along with some other image information. The code can be found in the "FilterMain.cpp" file.

<h3> There are two images titled "boats.bmp" and "blocks-small.bmp" for which these filters are applied to. The boats image is smaller than the blocks image in order to test the optimization of the code for various image sizes. The filtered images can be found in the folder titled "filtered-..." for each image/filter combo.

<h3> My code works by minimizing memory calls/using cache storage as much as possible, limiting cache collisions, loop unrolling 8 times (attempting to use as many registers as possible), using as small a data size for calculations as possible (such as division to decrease cpu clock cycles per item), and storing as many local function variables inside of the registers instead of memory as possible. Note that the highest level of optimization is turned on in the compiler with the flag -O3.

<h3> Most of the code in this project is my own, however the basic shell of the project itself was provided by my computer systems class. Other than small changes to some files, the majority of my work is located in the "FilterMain.cpp" file for which almost all of the code excluding most of the code in the "main" function is my own.
