![http://www.fao.org/fi/figis/org/data/assets/images/logos/ColombiaFlag.gif](http://www.fao.org/fi/figis/org/data/assets/images/logos/ColombiaFlag.gif)
![http://img717.imageshack.us/img717/7084/logouz.png](http://img717.imageshack.us/img717/7084/logouz.png)
<br><br>

<h1>Welcome to Gplad</h1>
In this page you'll know more about what is <b>Gplad</b>, This is a Project Developed for Jonathan Ray Cardenas (Student) and Fabian Giraldo (Teacher) of the <a href='http://www.sanmartin.edu.co/'>Fundacion Universitaria San Martin</a>.<br>
Please note that <b>Gplad</b>, and this GoogleCode website are currently in alpha development stage. We will Add More information and the code of the project as soon is ready to be launched. Let's start!<br>
<br>
<a href='http://translate.google.com.co/translate?sl=en&tl=es&js=n&prev=_t&hl=es&ie=UTF-8&layout=2&eotf=1&u=http%3A%2F%2Fcode.google.com%2Fp%2Fgplad%2F'>Version en Español</a>

<li><a href='http://code.google.com/p/gplad/#What_is_Gplad?'>What is Gplad</a><br>
<li><a href='http://code.google.com/p/gplad/#What_it_Does'>What it Does</a><br>
<li><a href='http://code.google.com/p/gplad/#Used_Technologies:'>Used Technologies</a><br>
<li><a href='http://code.google.com/p/gplad/#Why?'>Why?</a><br>
<li><a href='http://code.google.com/p/gplad/#Why?'>Videos?</a><br>

<h2>What is Gplad?</h2>
This project implements <b>Gplad</b> (Graphical Programming Language for Android Devices) an on-device graphical programming language for Android devices that is inspired by <a href='http://education.mit.edu/projects/starlogo-tng'>the Starlogo TNG</a> programming language developed by the MIT Scheller Teacher Education Program at the MIT.<br>
<br>
This application allows the construction of solutions to simple programming problems in a blocks-based programming interface that contains all the main structures of programming languages, like Conditionals (if,else), Variable definitions(strings,integers), and loops(for,while).<br>
<br>
Also, after create your solution you can obtain the code of the solution in a common Programming Language as <a href='http://en.wikipedia.org/wiki/Java_(programming_language)'>Java</a> or  <a href='http://www.cnc.una.py/sl/'>SL</a>. , this can be possible through the use of Intelligent Agents as <a href='http://jade.tilab.com/doc/tutorials/JADE_ANDROID_Guide.pdf'>JadeAndroid</a>.<br>
<br>
<h2>What it Does</h2>

As we said before, based in a blocks programming interface, The main screen of the application will contain the workspace, where the shapes will be dragged to start creating our solution to the problem. This Screen will contain a Menu that will Hold all the possible shapes to start, in this case, the main structures of a language.<br>
<br>
This is how is the menu developed at this time<br>
<img src='http://img844.imageshack.us/img844/7217/menuin.png' /><br>

After this the User will have some Idea of how to start creating the solution, based in the labels of each shape, Let's see a basic example of how this will work <b>Actually the project is in alpha phase, so the translation process of getting the specific language to SL and Java is not implemented yet</b>

Let's create a basic program example that give us the sum of all the Even numbers from 1 to 20, So We start Designing in our head the solution and then put it in the application, this is how should be created: <br>
<img src='http://img89.imageshack.us/img89/9544/examplepk.png' /><br>
The app will have a scroll view so we won't have this problem (in this case i put 2 images so we can see all the blocks)<br>

After we generate the solution in the blocks, it will be a button that will send the information through an agent to a server that will contain the Translator (JavaCC) and it will return the information to the Android Screen of the selected language (SL or Java).<br>
<br>
This will obtain the following Code in SL:<br>
<pre><code><br>
programa EvenNumbers<br>
var<br>
n, suma, k : numerico<br>
inicio<br>
n=20<br>
suma = 0<br>
k=2<br>
desde k hasta n paso 2<br>
{<br>
suma = suma + k<br>
}<br>
imprimir (“La suma es “, suma)<br>
fin<br>
<br>
</code></pre>

And the Following Java code:<br>
<pre><code><br>
public class EvenNumbers {<br>
	public static void main(String args[]){<br>
		int n=20;<br>
		int suma=0;<br>
		int k=2;<br>
		for(k=2;k&lt;n;k+=2){<br>
			suma=suma+k;<br>
		}<br>
		System.out.println("la suma es: "+ suma);<br>
	}<br>
}<br>
</code></pre>


<h3>Used Technologies:</h3>
<br>
<a href='http://jade.tilab.com/doc/index.html'><img src='http://jade.tilab.com/doc/logo.jpg' /></a>
<a href='http://source.android.com/'><img src='http://www.supernifty.com.au/images/android-logo.png' /></a>
<a href='http://javacc.java.net/'><img src='http://3.bp.blogspot.com/-0oeIdbBsl00/Tkh97QxrCtI/AAAAAAAAAbI/_zgHqVkam4o/s200/beans_javacc.gif' /></a>

<h2>Why?</h2>
This project was though to solve the problems that people have when they're getting started in the areas of programming language, most of them usually forget to put a semicolon or sometimes they omit a parenthesis, Users waste a lot of time correcting this kind of mistakes, so we decrease the time they use to correct this. Also, we're thinking in persons that have excellent logic (like physics or mathematics) but they don't know any programming lenguage, so if they want to solve a problem they don't must to learn a programming language just with their logic is enough.<br>
<br>
<br>
<h2>Videos</h2>
<a href='http://www.youtube.com/watch?feature=player_embedded&v=gn6EEE3W7Ig' target='_blank'><img src='http://img.youtube.com/vi/gn6EEE3W7Ig/0.jpg' width='425' height=344 /></a><br>
<br>
<a href='http://www.youtube.com/watch?feature=player_embedded&v=BZ4INB0Agjk' target='_blank'><img src='http://img.youtube.com/vi/BZ4INB0Agjk/0.jpg' width='425' height=344 /></a><br>
<br>
<br>
Mobile devices, especially those that handle Android operating system have been well received in recent years and are used to solve problems in real time. Nowadays some applications are being developed to support visual programming within these devices and mobile applications have been developed to accomplish this approach as Catroid and Scratch, since it has been proven through studies that allows graphical programming to gain more interest in software development and has supported applications for computers with Scratch, StarLogo and Alice. For these reasons is presented the design and analysis of an application that lets you to program using blocks from Android devices and allows the generation and execution of code in the Java language on a remote server<br>
<br>
<br>
<h2>Oriented Object Programming Videos</h2>
<a href='http://www.youtube.com/watch?feature=player_embedded&v=u17Pf2wicPk' target='_blank'><img src='http://img.youtube.com/vi/u17Pf2wicPk/0.jpg' width='425' height=344 /></a><br>
<br>
<a href='http://www.youtube.com/watch?feature=player_embedded&v=SF2KcFW5hW0' target='_blank'><img src='http://img.youtube.com/vi/SF2KcFW5hW0/0.jpg' width='425' height=344 /></a><br>
<br>
<br>
If you Have any Question About this project please contact us at: raycitoc@gmail.com<br>
Version 1.0 of Application and Page