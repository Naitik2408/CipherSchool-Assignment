  Linked list->

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

    // Constructor to initialize the head node with a value
    public LinkedList(int data) {
        head = new Node(data);
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
        list.display(); 
    }
}

output->
 // Output: 1 -> 4 -> 3 -> 2 -> null
