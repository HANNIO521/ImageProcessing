#include <b11035021.jpg>
#include <b11035021 2.jpg>
#include <b11035021 3.jpg> 

int main()
{
    char FileName[10]="rain.jpg";

    IplImage *Image1 = cvLoadImage(FileName,1);

    cvNamedWindow("Show Image",0);

    cvResizeWindow("Show Image",300,400);

    cvShowImage("Show Image",Image1);

    cvWaitKey(0); 

    cvDestroyWindow("Show Image");

    cvReleaseImage(&Image1);
}
