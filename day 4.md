# Execute CPP file using Linux Command Line:

>  + First check whether you are having g++ tool in your linux system or not by using \
**g++ --version**
> + If you are not having it then follow below instructions:
 >   + Enter following command in your linux terminal\
**yum group install 'Development tools'**
>    +	You will get response then enter **Y** and hit enter
>    + To check whether g++ tool install successful or not enter following command\
**g++ --version**

## Create a directory:

> We are creating a directory to save our cpp code in particular directory.
> + To create directory name as my_cpp_codes enter following command in linux terminal\
**mkdir my_cpp_codes**
> + To check whether our directory created or not enter following command\
**ls**
Which will list all files and directory of current working directory 
> + Now change current path to my_cpp_codes by using following command\
**cd my_cpp_codes**

## Compile and Execute CPP Codes:

> + First create cpp file using vi tool by using following command\
**vi HelloWorld.cpp**
> + Then enter **i** to enter in insert mode
> + Now write you cpp code 
> + Once done press esp key and enter following command to save your code into .cpp file\
**:w**
> + Now to exist from current file press esp key and following command\
**:q**
> + Check whether  .cpp file created successfully or not enter following command\
**ls**
> + Now compile your file using g++ tool, to compile enter following command\
**g++ HelloWorld.cpp -o HelloWorld** (it is name of your output after compilation process)
> + Now Execute your output file using following command\
**./HelloWorld**




