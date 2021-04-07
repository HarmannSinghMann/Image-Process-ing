Hey

I am hands on with python and due to my tight job(present) contraints , I have formulated my submission in python only.
Hoping this wont hurt my candidature .

My submission - 'solution.py'.

This code runs by default - if you have the following dependencies installed just run it through your editor . 
Press any key to kill the code or the display windows 

Please pip install the following dependencies to run my submission :
1.Python 
2.opencv

After installation: Run the code ( by cmd or in editor ) 

About 'writeup.html':
    Run it to see my results of the tasks.

    Note:
    I have saved the outputs of the tasks folder-wise thus have changed the <img src''> from 'output/'(default) to 'output/function_name/' in wrtiteup html 
    You can refer to output folder or <img> element in html for more understanding.


Description Of Code - 'solution.py' :
    1. Nature :
        This code takes in an image as input and gives output of all the functions (image processing operations) defined by me .
        NOTE: Composite function - It gives the composite output of the 3 input images(background,foreground,mask) given in the problem set 
       
        Output from code :
        1 Original-image 
        2 Brightness-Image
        3 Blurr-Image
        4 EdgeDetection-Image
        5 Sharpen-Image
        6 Contrast-Image
        7 Composite Image

        NOTE: All outputs will be seperate windows , kindly access them using your taskbar (as Shown in video - princeton_small )
        
    2. This code contains the following functions :
        Normalize Data - This function Normalizes the data in the range [0,1]                                - Parameter : (Image)
        brightness     - This Function changes the brighness of the image by the given factor                - Parameter : (Image,Brightness Factor)
        convolution    - This Function changes the brighness of the image by the given factor                - Parameter : (Image , kernel to convolute)
        Blur           - This function performs the blurr operation on the image by the factor of sigma      - Parameter : (Image , Blur factor-Sigma)
        contrast       - This operations changes the contrast of the image by the given factor               - Parameter : (Image , Contrast factor)
        composite      - This function Produces the composite of images provided all 3 parameters are given  - Parameter : (Image)
        ReadImage      - This function is used to read the image from the given path                         - Parameter : (background image,foreground image,mask image)
        
    3. To test the code you need to define the following in main function:
       path ='Path to image' (default path = 'input/princeton_small.jpg')
       
       OPTIONAL:
       You can change the following parameters to the desired number to test the function operations:
           factor_b: brighness factor   ( Default : 2 )
           Sigma : Blur factor          ( Default : 1 )
           factor_c : Contrast factor   ( Default : 1 )
           edge_kernel                  ( Default : [[-1, -1, -1], [-1, 8, -1], [-1, -1, -1]])
           sharp_kernel                 ( Default : [[-1, -1, -1], [-1, 9, -1], [-1, -1, -1]])         
