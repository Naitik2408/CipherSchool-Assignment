insertion at head->
code->
class Node {
    int data;
    Node next;

    // Constructor
    Node(int data) {
        this.data = data;
        this.next = null;
    }
}

public class LinkedList {
    Node head;

    // Constructor to initialize the linked list with a head node
    public LinkedList(int data) {
        head = new Node(data);
    }

    // Method to add a new element at the beginning of the list
    public void addFirst(int data) {
        Node newNode = new Node(data);
        newNode.next = head;
        head = newNode;
    }

    // Method to add a new element directly after the head node
    public void addAfterHead(int data) {
        Node newNode = new Node(data);
        newNode.next = head.next;
        head.next = newNode;
    }

    // Method to display the list
    public void display() {
        Node current = head;
        while (current != null) {
            System.out.print(current.data + " -> ");
            current = current.next;
        }
        System.out.println("null");
    }

    public static void main(String[] args) {
        // Create a LinkedList with the initial head node value 1
        LinkedList list = new LinkedList(1);
        
        // Add new elements directly after the head node
        list.addAfterHead(2);
        list.addAfterHead(3);
        list.addAfterHead(4);
        
        // Display the linked list
        System.out.println("List after adding elements after the head:");
        list.display();  // Output: 1 -> 4 -> 3 -> 2 -> null

        // Add a new element at the beginning of the list
        list.addFirst(0);

        // Display the linked list
        System.out.println("List after adding element at the beginning:");
        list.display();  // 
    }
}

Output: 0 -> 1 -> 4 -> 3 -> 2 -> null

insertion at end of list
code->


class Node {
    int data;
    Node next;

    // Constructor
    Node(int data) {
        this.data = data;
        this.next = null;
    }
}
public class LinkedList {
    Node head;

    // Constructor to initialize the linked list with a head node
    public LinkedList(int data) {
        head = new Node(data);
    }

    // Method to insert a new element at the end of the list
    public void insertAtEnd(int data) {
        Node newNode = new Node(data);
        
        if (head == null) {
            head = newNode;
            return;
        }

        Node current = head;
        while (current.next != null) {
            current = current.next;
        }

        current.next = newNode;
    }

    // Method to display the list
    public void display() {
        Node current = head;
        while (current != null) {
            System.out.print(current.data + " -> ");
            current = current.next;
        }
        System.out.println("null");
    }

    public static void main(String[] args) {
        // Create a LinkedList with the initial head node value 1
        LinkedList list = new LinkedList(1);

        // Insert new elements at the end of the list
        list.insertAtEnd(2);
        list.insertAtEnd(3);
        list.insertAtEnd(4);

        // Display the linked list
        list.display();  \
    }
}
 Output: 1 -> 2 -> 3 -> 4 -> null
