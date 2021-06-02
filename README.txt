# Crime Status Counter

Crime Status Counter is a Python Web Crawler counting the name of the cities in Washington being written in a local news website, it has redundant check to avoid the same news being add to the status.

## Usage

```python
object1 = crime_data()
userinput=-1
object1.show()
try:
    while (userinput!= '0'):
        print('enter 1 to calculate the count of sities showing up onthe crime news web page')
        print('enter 2 to show the data on console')
        print('enter 3 to clean the data')
        print('enter 0 to exit')
        userinput=input('enter your input \n')
        if(userinput=='1'):
            object1.start()
        elif(userinput=='2'):
            object1.show()
        elif(userinput=='3'):
            object1.clean()
            object1=crime_data()
        else:
            print('invalid input')
        print("Good bye!")
    except:
        print('something went wrong!')
