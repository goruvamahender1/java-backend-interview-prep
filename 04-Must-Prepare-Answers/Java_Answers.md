## Java Must Prepare Answers


#### 26.
Think of the coffee in the cup as the data in a variable. ⚡️
One is a copy and one is the original

![alt text](/Images/image-1.png)

#### 43. 
Patterns are reusable solutions to common design problems, resulting in a smoother, more efficient development process. They serve as blueprints for building better software structures. These are some of the most popular patterns:

- Abstract Factory: Family Creator - Makes groups of related items.
- Builder: Lego Master - Builds objects step by step, keeping creation and appearance
- Prototype: Clone Maker - Creates copies of fully prepared examples.
- Singleton: One and Only - A special class with just one instance.
- Adapter: Universal Plug - Connects things with different interfaces.
- Bridge: Function Connector - Links how an object works to what it does.
- Composite: Tree Builder - Forms tree-like structures of simple and complex parts.
- Decorator: Customizer - Adds features to objects without changing their core.
- Facade: One-Stop-Shop - Represents a whole system with a single, simplified interface.
- Flyweight: Space Saver - Shares small, reusable items efficiently.
- Proxy: Stand-In Actor - Represents another object, controlling access or actions.
- Chain of Responsibility: Request Relay - Passes a request through a chain of objects until handled.
- Command: Task Wrapper - Turns a request into an object, ready for action.
- Iterator: Collection Explorer - Accesses elements in a collection one by one.
- Mediator: Communication Hub - Simplifies interactions between different classes.
- Memento: Time Capsule - Captures and restores an object's state.
- Observer: News Broadcaster - Notifies classes about changes in other objects.
- Visitor: Skillful Guest - Adds new operations to a class without altering it.
![alt text](/Images/image-6.png)

#### 67.
🚀 Serialization & Deserialization in Java 💻☕

🔐 Serialization is the process of converting a Java object into a byte stream 🧱 — making it easy to save the object to a file 🗂️ or send it over a network 🌐.

🔓 Deserialization is the reverse process — converting the byte stream back into a Java object 🧬.

📦 Why use it?
✅ Store object state persistently (e.g., in files or DBs)
✅ Transmit objects between JVMs or over networks (e.g., RMI, HTTP)

🛠️ How to serialize in Java?

ObjectOutputStream oos = new ObjectOutputStream(new FileOutputStream("data.ser"));
oos.writeObject(myObject);
oos.close();

🛠️ How to deserialize in Java?

ObjectInputStream ois = new ObjectInputStream(new FileInputStream("data.ser"));
MyClass obj = (MyClass) ois.readObject();
ois.close();

🧾 Note:
 • The class must implement Serializable 🧩
 • Fields marked transient ❌ will not be serialized

💡 Use serialization wisely — it’s powerful, but version control of classes and performance considerations are important! ⚠️

#### 17.

𝗖𝗼𝗻𝘀𝘁𝗿𝘂𝗰𝘁𝗼𝗿𝘀 are essential for 𝗼𝗯𝗷𝗲𝗰𝘁 𝗶𝗻𝗶𝘁𝗶𝗮𝗹𝗶𝘇𝗮𝘁𝗶𝗼𝗻 in Java. 

Here’s a crisp breakdown for interviews & real-world clarity:
🔹 𝗖𝗼𝗿𝗲 𝗖𝗼𝗻𝗰𝗲𝗽𝘁𝘀:
 1. 𝗗𝗲𝗳𝗮𝘂𝗹𝘁 𝗖𝗼𝗻𝘀𝘁𝗿𝘂𝗰𝘁𝗼𝗿 – No-arg constructor that initializes default values.
 2. 𝗣𝗮𝗿𝗮𝗺𝗲𝘁𝗲𝗿𝗶𝘇𝗲𝗱 𝗖𝗼𝗻𝘀𝘁𝗿𝘂𝗰𝘁𝗼𝗿 – Accepts arguments for custom initialization.
 3. 𝗢𝘃𝗲𝗿𝗹𝗼𝗮𝗱𝗶𝗻𝗴 – Multiple constructors in a class with different params.

🔍 𝗧𝗿𝗶𝗰𝗸𝘆 𝗜𝗻𝘁𝗲𝗿𝘃𝗶𝗲𝘄 𝗤𝘂𝗲𝘀𝘁𝗶𝗼𝗻:
🤔 𝗖𝗮𝗻 𝗮 𝗰𝗼𝗻𝘀𝘁𝗿𝘂𝗰𝘁𝗼𝗿 𝗯𝗲 𝘀𝘁𝗮𝘁𝗶𝗰, 𝗳𝗶𝗻𝗮𝗹, 𝗼𝗿 𝗵𝗮𝘃𝗲 𝗮 𝗿𝗲𝘁𝘂𝗿𝗻 𝘁𝘆𝗽𝗲?
 ✖ 𝗡𝗼!
1. static → belongs to class, not object
2. final → constructors aren’t inherited
3. void or return type → becomes a method, not a constructor
4. 𝗕𝘂𝘁 a constructor 𝗰𝗮𝗻 𝘂𝘀𝗲 𝗿𝗲𝘁𝘂𝗿𝗻; 𝘄𝗶𝘁𝗵𝗼𝘂𝘁 𝗮 𝘃𝗮𝗹𝘂𝗲 to 𝗲𝘅𝗶𝘁 𝗲𝗮𝗿𝗹𝘆 when needed.

🔹 𝗥𝘂𝗹𝗲𝘀 𝗧𝗼 𝗥𝗲𝗺𝗲𝗺𝗯𝗲𝗿:
 1.  Constructor name = class name
 2.  No return type allowed
 3. If no constructor → Java provides default
 4. If any constructor exists → no default provided
 5. Constructors can’t be static, final, abstract
 6. Use this() to call another constructor in the same class
 7. Use super() to call superclass constructor
 8. First line must be this() or super() (if used)