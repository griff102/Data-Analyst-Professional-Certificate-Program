# Module 4 - Working with Data in Python



# Reading Files with Open

### To open a file:

* Use the **open** function see below

  ![](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729184901385.png)

  

* The first argument show below is the file path

  ![image-20210729185044666](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729185044666.png)

  

* This is made up of the 'File name' as seen below

  ![image-20210729185145464](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729185145464.png)

  * And the File Directory

    ![image-20210729185319113](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729185319113.png) 

* The second parameter is the mode:

  * Common values used include 'r' for reading,

  * 'w' for writing, and 'a' for appending.

  * We will use 'r' for reading

    ![image-20210729185501897](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729185501897.png) 

* Finally is the file 'object'
* ![image-20210729185645385](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729185645385.png)

### **We can now use the file object to obtain information about the file**

* We can use the data attribute name to get the name of the file.
* The result is a string that contains the name of the file.
  * We can see what mode the object is in using the data attribute mode, and 'r' is shown representing read.
    * You should always close the file object using the method close.

![image-20210729190200173](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729190200173.png)

### Using the with statement to close the file

* Using a "with" statement to open a file is better practice because it automatically closes the file.

* The code will run everything in the indent block, then closes the file.

  ![image-20210729190839908](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729190839908.png)

  * This code reads the file, Example1.txt.
  * We can use the file object, "File1."
  * The code will perform all operations in the indent block then close the file at the end of the indent.
  * The method "read" stores the values of the file in the variable "file_stuff" as a string.
  * You can print the file content.

#### File object:

![image-20210729191326025](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729191326025-16275572072611.png)

#### Indented Block: The code will preform all of the functions in the indent block:

![image-20210729191434425](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729191434425.png)

#### And then close the file at the end of the indent:

![image-20210729191605256](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729191605256.png)



#### The method read stores all of the values of the file in the variable "file_stuff" as a string

![image-20210729191639484](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729191639484.png)

#### You can print the file content. You can check if the file content is closed, but you cannot read from it outside the indent. But you can print it outside the indent as well. You can print the file content.



![image-20210729191838281](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729191838281.png)



#### We can print the raw content. When we look at the raw string we see '\n', this is so Python knows to start a new line.

![image-20210729192412129](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729192412129.png)



#### We can output every line as an element in a list using the method "readlines" (Frist line corresponds to the first element in the list, etc..)

![image-20210729192637035](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729192637035.png)

#### We can use the method "readline" to read the first line of the file.

* If we run this command, it will store the first line in the variable "file_stuff" then print the first line.
* We can use the method "readline" twice. 
* The first time it's called it will save the first line in the variable "file_stuff", and then print the first line
* The second time its called, it will save the second line in the variable "file_stuff" and then print the second line. 

![image-20210729193509761](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729193509761.png)

#### We can use a loop:

* This will print out each line individually as follows:

  ![image-20210729194043323](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729194043323.png)

* ![image-20210729194304722](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729194304722.png)

#### We can specify the number of characters we would like to read from the string as an argument to the method "readlines"(in this example we used (16)) 'as see above'



#### From Lab1 "Reading Files with Open"



![image-20210729200108343](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729200108343.png)



![image-20210729200039344](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729200039344.png)

#### Reading the first four characters syntax: (or a certain number of Characters)

![image-20210729200234379](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729200234379.png)

![image-20210729200333053](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729200333053.png)

![image-20210729200451785](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729200451785.png)



#### Syntax for reading one line at a time:

![image-20210729200615930](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729200615930.png)



#### We can also pass an argument to readline() to specify the number of characters we want to read. However, unlike read(), readline() can only read one line at most:

![image-20210729201010407](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729201010407.png)



#### We can use a Loop to iterate through each line: 

![image-20210729201128390](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729201128390.png)



#### We can use the method readlines() to save the text file to a list:

![image-20210729201337108](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729201337108.png)

#### Each element of the list corresponds to a line of text:

![image-20210729201443198](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729201443198-16275608843402.png)

#### Weather Exercise:

![image-20210729210030417](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729210030417.png)





#### See Below for solution:

![image-20210729211914974](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729211914974.png)

![image-20210729212153286](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210729212153286.png)



Solutions for importing in matplot

![image-20210730203714617](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210730203714617.png)

![image-20210730204034532](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210730204034532.png)



# Writing Files with Open:



#### We can also write to files using the open function:

1. We will use Python's open function to get a file object to create a text file.
2. We can apply method write **"w'"** to write data to that file.
3. As a result, text will be written to the file.
4. We can create the file **Example2.txt** as follows.
   * We use the **open** function.
5. The first argument is the **file path**. ("/resources/data/
6. This is made up of the file name. **/Example2.txt,**
7. If you have that f**ile in your directory,**
8. **it will be overwritten**, and the file directory.
9. Finally we have the file object **as File1:**

![image-20210731112431050](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731112431050.png)



​                                                  

**We use the open function.**

1. This creates a file Example2.txt in your directory.

2. We use the method write, to write data into the file.

3. The argument is the text we would like input into the file.

4. If we use the write method successively,

5. each time it is called, it will write to the file.

   

![image-20210731113613320](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731113613320.png)



**This is called write the file:**

1. "This is line A " to represent a new line.
2. The second time we call the method, it will write,
3. "this is line B " then it will close the file.
4. We can write each element in a list to a file.



#### As before we use the with command and open function to create a file:

* The list, Lines, has three elements consisting of text.
* We use a **for loop** to read each element of the first lines and pass it to the variable line.
* The first iteration of the loop writes
* the first element of the list to the file Example2.
* The second iteration writes the second element of the list and so on.
* At the end of the loop, the file will be closed.



![image-20210731114132583](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731114132583.png)

#### We use the for loop to read each element in the lines



#### We can set the mode to appended using the ,"a"

* This will not create a new file but just use the existing file:
* ![image-20210731114939278](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731114939278.png)



#### We can copy on file to a new file as follows:



![image-20210731115158783](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731115158783.png)





### Lab 2: Writing files with open:

![image-20210731120717806](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731120717806.png)



#### You can check the file to see if you are correct

![image-20210731120817508](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731120817508.png)

#### Next

![image-20210731120914212](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731120914212.png)

#### Note the the setting 'w' overwrites all of the text in the file

![image-20210731121254067](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731121254067.png)

![image-20210731121504830](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731121504830.png)

![image-20210731121533908](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731121533908.png)

#### Additional Modes:

![image-20210731121636325](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731121636325.png)

![image-20210731122015172](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731122015172.png)

![image-20210731122109085](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731122109085.png)

New locations:

![image-20210731123410907](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731123410907.png)

![image-20210731130150659](C:\Users\Christopher\OneDrive\6-Edx Materials & Assignments\IBM Data Analytics\4-Python Basics for Data Science\Module 4 - Working with Data in Python\Module 4 - Working with Data in Python.assets\image-20210731130150659.png)

