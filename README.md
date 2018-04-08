## MyWallPaper
A project on Android 3D wallpaper （OpenGL ES）,the IDE is Android Studio2.4.1,the version is old,you can open this project with a higher version Android Studio.

There are  some Swimming fish,these fish are divided into a single fish and fish school,the bule fish is single,the red fish and the orange is fish school .it use one AI(Artificial intellgence ) algorithm ,it is improtant  in this project.The background uses a texture rectangle,the fish model and the shell uses skeletal animation,i don't uses the FBX,use a custom bone animation.The project  involve some physics and 3D math.

## Run Result

This gif is compressed,so it may not be very clear.

![1](./result/result.gif)

## AI Fish algorithm

it simulate the real world,for example,speed,force and other Details,the picture can only vaguely introduce this algorithm,i omitted some details,can read the class from the folder--fish and fishschool.
#### single fish algorithm
![singlefish](./result/singlefish1.png)![singlefish](./result/singlefish2.png)

Use two fish to illustrate,fish A and fish B.Each fish has two attributes,speed and force.At first,the two fish are far away,the force is small,the distance between the two narrows,The force between the two becomes larger,it does not cause two fish to collide.

So,at the beginning of the program,you should set the initial speed and the force is ok,when the fish encounter the wall,give the fish opposite force is ok.These parameters need to be experienced .

####  fish school algorithm
![fischool](./result/fishschool.png)

The algorithm is similar to the single fish algorithm.the four fish are affected by the force of center fish ,you can think the center fish as a single fish .Of course ,the greater the  distance ,the greater the force .