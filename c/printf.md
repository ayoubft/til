# `printf`

`printf` is a functions family that produce output according to a format as described below: 

```
%[parameter][flags][width][precision][length]type
```

Example: 
```c
int width = 5;
int num = 1234;
printf("%*d \n", width, num);
printf("%2$*1$d \n", width, num);

// pi
printf("Pi = %.6f \n", 4*atan(1));

// date
char *month = "January";
char *weekday = "Tuesday";
int year = 2023;
int day = 24;
int hour = 11;
int minute = 53;
printf("Now is: %s %dth %s %d, %.2d:%.2d \n", weekday, day, month, year, hour, minute);
```
The above example when executed results in this:
```
 1234
 1234
Pi = 3.141593 
Now is: Tuesday 23th January 2023, 11:53
```

* Note that the first two printfs have the same output with a space padded at the left to make a width of 5 characters.
