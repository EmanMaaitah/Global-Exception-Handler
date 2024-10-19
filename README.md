# OBJECTIVE 
The [Global-Exception-Handler](https://docs.uipath.com/studio/standalone/2023.4/user-guide/global-exception-handler) used when you receive a project from another coworker in the same team and want to make sure that the project is correct.

# PROCEDURES
How to insert a Global-Exception-handler scope
In the Design tab part of the Ribbon, select New > Global Handler
You can unpack and link the Global-Exception-handler through Project Panel > Right click > Set as Global Handler or Remove Handler


<img src="https://github.com/user-attachments/assets/a041f1a5-7807-419d-8e5a-1866d1ede8e9" width="500">

You can confirm through the Project file.json from the global-Exception-handler scope link to the project

![image](https://github.com/user-attachments/assets/8b358d2f-7477-48a3-867f-587d3198caf3)


The number of attempts will be entered in the condition box > The number of attempts will be printed at each round

# Results

To watch the robot run and the results, [click here](https://drive.google.com/file/d/1Od5widPQyt08J11YDIY6XNUHxAxdzkLv/view?usp=sharing)



# CONCLUSION
The activities that are located inside Global-Exception-Handler by default are: 
1) Log Error
2) If Condition /Choose Next Behaviour inside the do scope there are three options of commands:
-Continue - The exception is re-thrown.
-Ignore - The exception is ignored, and the execution continues from the next activity.
-Retry - The activity which threw the exception is retried. Use the RetryCount method for errorInfo to count the number of times the activity is retried.
-Abort - The execution stops after running the current Global Exception Handler.

The condition is by defult three roundings

<img src="https://github.com/user-attachments/assets/9cb5b6b4-2f2c-4aca-99b5-854483846340" width="500">

