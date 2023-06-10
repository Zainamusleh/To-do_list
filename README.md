# To-do list

### goal! 

Being able to oragnize your tasks and time is a pretty diffecult thing to a lot of people , so this program is going to help you list down you tasks for you to  be able to manage your time and use it the right way!

<p align="center">
<picture>
  <img alt="An overwhelming man" src="https://th.bing.com/th/id/OIP.eZagGTx71Y5Ar5GhJLtNnQHaE7?pid=ImgDet&rs=1" width="50%" hight="50%" >
</picture>
</p>


###  code 

```
tasks =[]

#the options of the to-do list

def options():
    print("1.Add a task")
    print("2.delete a task")
    print("3.view tasks")
    print("4.Marking tasks as completed")


#function of adding a task
def Add():
    task = input("A task :")
    tasks.append(task) #to add the input of task in tasks
    print("task added successfully")

#function : delete a task
def delete():
    task = input("Enter the task you want to delete: ")  

    tasks.remove(task)
  
    print("please write the exact task you added")
    print("task deleted successfully")

#Function : view tasks 
def view_tasks():
    print(tasks)

#completed tasks
def completed():
        task = input("Enter the task to mark as completed: ")
        if task in tasks:
            tasks.remove(task)
            print("Task marked as completed!")
        else:
            print("Task not found, please write the correct task")



#the to do list

while True:
     options()
     user = int(input("Choose an option from 1-4: "))
     if user == 1:
          Add()
     elif user == 2:
          delete()
     elif user == 3:
          view_tasks()
     elif user ==4:
          completed()
     else:
          break
```
