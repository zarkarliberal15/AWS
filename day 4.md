# Execute CPP file using Linux Command Line:

>  + First check whether you are having g++ tool in your linux system or not by using \
**g++ --version**
> + If you are not having it then follow below instructions:
 >   + Enter following command in your linux terminal\
**yum group install 'Development tools'**\

 >  ![](images/day%204%20images/1.JPG)
>    +	You will get response then enter **Y** and hit enter\
>  ![](images/day%204%20images/2.JPG) 
>    + To check whether g++ tool install successful or not enter following command\
**g++ --version**\
>  ![](images/day%204%20images/3.JPG)

## Create a directory:

> We are creating a directory to save our cpp code in particular directory.
> + To create directory name as my_cpp_codes enter following command in linux terminal\
**mkdir my_cpp_codes**\
>  ![](images/day%204%20images/4.JPG)
> + To check whether our directory created or not enter following command\
**ls**\
Which will list all files and directory of current working directory \
>  ![](images/day%204%20images/5.JPG)
> + Now change current path to my_cpp_codes by using following command\
**cd my_cpp_codes**\
>  ![](images/day%204%20images/6.JPG)

## Compile and Execute CPP Codes:

> + First create cpp file using vi tool by using following command\
**vi HelloWorld.cpp**
\
>  ![](images/day%204%20images/7.JPG)\
>  ![](images/day%204%20images/8.JPG) 
> + Then enter **i** to enter in insert mode\
>  ![](images/day%204%20images/9.JPG)
> + Now write you cpp code\
>  ![](images/day%204%20images/10.JPG)

> + Once done press esp key and enter following command to save your code into .cpp file\
**:w**\
>  ![](images/day%204%20images/11.JPG)\
>  ![](images/day%204%20images/12.JPG)
> + Now to exit from current file press esp key and following command\
**:q**\
>  ![](images/day%204%20images/13.JPG)\
>  ![](images/day%204%20images/14.JPG)
> + Check whether  .cpp file created successfully or not enter following command\
**ls**\
>  ![](images/day%204%20images/15.JPG)
> + Now compile your file using g++ tool, to compile enter following command\
**g++ HelloWorld.cpp -o HelloWorld** (it is name of your output after compilation process)\
>  ![](images/day%204%20images/16.JPG)
> + Now Execute your output file using following command\
**./HelloWorld**\
>  ![](images/day%204%20images/17.JPG)




