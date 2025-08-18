Delegates 
-----------

⦁	type-safe function pointer.
⦁	holds the reference to the method (or multiple methods).
⦁	allows methods to be passed as parameters.
⦁	signature of method must match with signature of the delegates.


Types
------
⦁	Single-cast Delegate
⦁	Multi-cast Delegate
⦁	Built-in Delegate

Single-cast Delegate (with example)
-----------------------------------

// access modifier
// delegate keyword
// return type of the method.
// delegate name.
// signature must match with method signature.
public delegate int MathOperation(int x, int y);

public class calculator
{
 	public static int Add(int x, int y) => x + y;
 
 	public static int Multiply(int x, int y)
 	{
 		return x * y;
 	}
}

MathOperation op1 = Calculator.Add;
MathOperation op2 = Calculator.Multiply;

Console.WriteLine(op1(5,10)); // output 15
Console.WriteLine(op2(5,10)); // output 50

Multi-cast Delegate (with example)
-----------------------------------
public delegate void Notify(string message);

public class NotificationService
{
	public void SendEmail(string message)
	{
		Console.WriteLine('Mail sent' + message);
	}
	
	public void SendSms(string message)
 	{
 		Console.WriteLine('SMS sent' + message);
 	}
	
	public void SendPushNotification(string message)
 	{
 		Console.WriteLine('Push notification' + message);
 	}

}

public class TransactionProcessor
{
	public void ProcessTransaction(Notify notify)
	{
		Console.WriteLine('Transaction Completed');
		
		notify('Your transaction successfully');
	}
}

TransactionProcessor transaction = new TransactionProcessor();
NotificationService service = new NotificationService();

Notify nofify = service.SendEmail;
notify += service.SendSms;
notify += service.SendPushNotification;

transaction.ProcessTransaction(notify);

Built-in Delegates
------------------
Action<T>
--------
⦁	No return type.
Action<string> print = msg => Console.WriteLine(msg);
print("Hello From Action");

Func<T, TResult>
----------------
⦁	Return type must.
Func<int, int, int> add(a,b) => a + b;
Console.WriteLine(add(10,5); // 15

Predicate<T>
----------------
⦁	Return type boolean.
Predicate<int> isEven = num => num % 2 == 0;
Console.WriteLine(isEven(10)); // true

Events
------

⦁	specal delegate mechanism used for publish and subscribe communication.
⦁	allows one object to notify to another object when something happens.
⦁	foundation of GUI frameworks (WinForms/WPF), .NET events, and many real-time apps.

// Step 1: Define a delegate type
public delegate void NotifyHandler(string message);

// Step 2: Define an event in a class (Publisher)
public class Process
{
    public event NotifyHandler ProcessCompleted;  // Event declaration

    public void Start()
    {
        Console.WriteLine("Process Started...");
        // Raise event
        ProcessCompleted?.Invoke("Process finished successfully!");
    }
}

// Step 3: Subscriber
Process process = new Process();

// Subscribe to event
process.ProcessCompleted += (msg) => Console.WriteLine(msg);

// Trigger
process.Start();



