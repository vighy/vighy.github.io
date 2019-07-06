<h2>A primer on Design Patterns</h2>
Wikipedia defines a design pattern as a general reusable solution to a commonly occurring problem within a given context in software design.

More importantly, Design patterns help developers communicate effectively.

It is easy to get lost among all the terms and patterns. This post will try to classify and explain the different design patterns and terms involved while designing good software and clean code.
<br><br>
<u><b>Types of Design Patterns</b></u>
<ol type="1">
	<li>Gang of Four (GoF) Design Patterns</li>
	<ul>
	  <li>Creational</li>
	  	<ul>
	  		<li>Abstract Factory - Creates an instance of several families of classes</li>
			<li>Builder - Separates object construction from its representation</li>
			<li>Factory Method - Creates an instance of several derived classes</li>
			<li>Object Pool - Avoid expensive acquisition and release of resources by recycling objects that are no longer in use</li>
			<li>Prototype - A fully initialized instance to be copied or cloned</li>
			<li>Singleton - A class of which only a single instance can exist</li>
	    </ul>
	  <li>Structural</li>
	  	<ul>
	  		<li>Adapter - Match interfaces of different classes</li>
			<li>Bridge - Separates an object's interface from its implementation</li>
			<li>Composite - A tree structure of simple and composite objects</li>
			<li>Decorator - Add responsibilities to objects dynamically</li>
			<li>Facade - A single class that represents an entire subsystem</li>
			<li>Flyweight - A fine-grained instance used for efficient sharing</li>
			<li>Private Class Data - Restricts accessor/mutator access</li>
			<li>Proxy - An object representing another object</li>
		</ul>
	  <li>Behavioral</li>
	  <ul>
	  		<li>Chain of responsibility - A way of passing a request between a chain of objects</li>
			<li>Command - Encapsulate a command request as an object</li>
			<li>Interpreter - A way to include language elements in a program</li>
			<li>Iterator - Sequentially access the elements of a collection</li>
			<li>Mediator - Defines simplified communication between classes</li>
			<li>Memento - Capture and restore an object's internal state</li>
			<li>Null Object - Designed to act as a default value of an object</li>
			<li>Observer - A way of notifying change to a number of classes</li>
			<li>State - Alter an object's behavior when its state changes</li>
			<li>Strategy - Encapsulates an algorithm inside a class</li>
			<li>Template method - Defer the exact steps of an algorithm to a subclass</li>
			<li>Visitor - Defines a new operation to a class without change</li>
	  </ul>
	</ul>
	<li>Enterprise integration patterns</li>
	<li>Enterprise Application patterns - Marting fowlers patterns book</li>
</ol>
<br>
There are other terms like GRASP, SOLID when you speak about Object Oriented Design.
<br>
I will touch upon all these and with examples in future posts. Till then treat this post as a placeholder.
