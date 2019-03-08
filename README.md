INTRODUCTION

We implemented android studio features such as; activities and fragments using viewpager, android graphics and material design, to develop an appointment mobile application for a medical doctor. The motivation for this project is to assist medical doctors to keep up with their busy schedule efficiently and effectively. Our project design made use of graphics, fragment, viewpager and material customize our user interface. The application contains activities that allows the doctor to enter patients’ data and also patients’ treatment schedule. SQLite was used for data persistence and also broadcast service was used to send alarm to doctor to remind him of an appointment with patient. A background service of along patient data has been entered or any editing is been performed on the stored data was also set using service in android studio.
Activities, fragment, viewpager, material design and android graphics are very important to our concept because they are important part of an android application and also allows users’ flexibility in android application design. These android features are very essential when designing an attractive and a customized user interface for a medical or health application.


ACTIVITY
	It is one screen of an android users’ interface, it is similar to window in desktop application. 
	An android may have more than one activity, i.e. more than screen. The android app starts by showing the main activity. One activity is capable of implementing another in an application or invoking(calling) another activity in another app, in order to perform different actions.
	It is an entry point for users’ interaction with the application
	All activities in android apps are represented by an activity class which is a subset of android.app.Activity.
Activity Life cycle
To implement activity, information must be registered in the app’s manifest and the activity life cycle must be well managed
Methods in Activity Class;
onCreate ()
onStarted ()
onResumed ()
onPaused ()
onStopped ()
onDestroyed ()


FRAGMENT
•	It represents a behavior or a portion of user interface in a Fragment Activity
•	Its aims at enhancing users experience when designing an app. It helps to create more logical layout that users can understand.
•	It provides additional information and control without leaving the activity
•	To create a fragment, you must create a subclass of Fragment (or an existing subclass of it).
•	It is easier to pass data between screens with Fragments than it is with Activities. 
•	It can be easily display at different positions on screen (drop-downs, pop-ups, slide menus, etc.) and can be change depending on the current screen size or orientation.
A fragment contains callback methods similar to an activity, such as onCreate(), onStart(),  onPause()  and  onStop().
 

VIEWPAGER
•	It is a class that allows the user to flip left and right through pages of an app.
•	It is most often used along with fragment which is convenient way to manage the life cycle of each page.
•	It is a widget found in the support library
•	Its implementation requires putting the elements in XML layout.
•	It works with PagerAdapter which manages the pages
•	To display sliding fragments two FragmentPagerAdapter methods are used; getCount() and getItem().



ANDROID GRAPHICS (Graphics API, 2D Graphics, Android.Graphics.Canvas)
Graphics are important in designing an appealing application and it determine user demand for application. Android Graphics provides API that enables user to draw and animate shapes and images to   enhance user interface design of an application. This is very useful in designing an application that can be used for taking medical statistics, where shapes and images are needed for    description of data. This project made used of Android Graphics 2D to design  UI of a simple application for medical statistics and also draw an analog clock.
Android 2D Graphic: Android provides a custom 2D graphics library/API for drawing and animating shapes and images. Common classes for animating and drawing in two dimensions can be found in android graphic.drawable and android.view.animation. 2D can be approached in two ways;
1.	Using a View object: Graphics drawing is handled by the system’s normal view hierarchy drawin process. It is suitable for simple graphics that do not need to change dynamically. It is also used to draw background of a view to an image View in layout.
2.	Using Canvas: It uses appropriate class draw () methods and passing them the canvas. It is good for application that frequently draw the screen.

2D With Drawables
i.	It makes use of Drawables for drawing shapes and images to View. 
ii.	Its resources are usually stored in res/drawable folder of an android project
iii.	It can be defined and instantiated in three ways;using an image saved in a project resources, using an XML file that defines Drawable properties, using normal class constructors in code
iv.	It contains Drawable class and Subclass;BitmapDrawable, ShapeDrawable, LayerDrawable
v.	It is in different forms; Bitmap, Nine Patch, Shape, Layer, State, Levels and Scale.

2D Drawing with Canvas
i.	It is suitable for application that requires specialized drawing and control of the animation graphics
ii.	It provides the interface to the actual surface upon which graphics can be drawn
iii.	It offers a set of drawing methods; drawBitmap(), drawRect(), drawText(), etc.
iv.	It works on View class, by extending View and defining on Draw () callback method
v.	It also works on SurfaceView which is a special subclass of View that offers a dedicated drawing surface within the View hierarchy


MATERIAL DESIGN
It is a visual language that combine the classic principles of good design with the innovation of technology and science. Its goals are; to unify, create and customize. It has diverse features such as; Material Theme, new widgets, custom shadows, vector drawables and custom animations.
Principles Guiding Material Design
Material Design is inspired by the physical world and its textures, including how they reflect light and cast shadows.
i.	Bold, graphic, intentional
Material Design is guided by print design methods — typography, grids, space, scale, color, and imagery — to create hierarchy, meaning, and focus that immerse viewers in the experience.   
ii.	Cross-platform
Material Design maintains the same UI across platforms, using shared components across Android, iOS, Flutter, and the web.
iii.	Motion provides meaning
As elements appear on screen, they transform and reorganize the environment, with interactions generating new transformations.
iv.	Flexible foundation
It’s integrated with a custom code based that allows the seamless implementation of components, plug-ins, and design elements


Other Features used in our application are;
Data persistence using SQLite: This was used to store data without changing even when the activity is closed.
Service: This runs at the background to provide information on how long data has been stored or edited by user.
Broadcast Receiver: This was used to send alarm to the doctor to remind him of appointment with patient.
