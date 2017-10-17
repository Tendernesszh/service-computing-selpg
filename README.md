# service-computing-selpg
## 测试部分
First, generate three files, inputFile.txt, outputfile.txt and errorfile.txt<br>
inputFile.txt file has 10 pages, each page has 10 lines, of course, I specified selpg each line is also 10 pages (default is 72)<br>
Test:<br>
1.<br>
input: $ ./selpg -s 1 -e 1 inputfile.txt<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test1.png)<br>
As Figure, the success of the first page of the 10 lines of text output to the screen.<br>

2.<br>
input: $ ./selpg -s 1 -e 1 < inputfile.txt<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test2.png)<br>

3.<br>
input: $ python testout.py | ./selpg -s 1 -e 1 < inputfile.txt<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test3.png)<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test3(1).png)<br>

4.<br>
input: $ ./selpg -s 5 -e 10 inputfile.txt >outputfile.txt<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test4(1).png)<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test4(2).png)<br>

5.<br>
input: $ ./selpg -s 1 -e 8 inputfile.txt 2>errorfile.txt<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test5(1).png)<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test5(2).png)<br>

6.<br>
input: $ ./selpg -s 4 -e 6 inputfile.txt >outputfile.txt 2>errorfile.txt<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test6(1).png)<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test6(2).png)<br>

7.<br>
input: $ ./selpg -s 2 -e 4 inputfile.txt >outputfile.txt 2>/dev/null<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test7.png)<br>

8.<br>
input: $ ./selpg -s 1 -e 3 inputfile.txt >/dev/null<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test8.png)<br>

9.<br>
input: $ ./selpg -s 2 -e 5 -l 7 inputfile.txt<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test11.png)<br>
10.<br>
input: $ ./selpg -s 1 -e 4 -f inputfile.txt<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test12.png)<br>

11.<br>
input: $ ./selpg -s 1 -e 3 inputfile.txt > outputfile.txt 2>errorfile.txt &<br>
output:<br>
![image](https://github.com/Tendernesszh/service-computing-selpg/blob/master/testpicture/test14.png)<br>
